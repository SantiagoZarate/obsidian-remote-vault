---
title: "Mocking Drizzle instance - Drizzle Team"
source: "https://www.answeroverflow.com/m/1135298272248995850"
author:
  - "[[fermentfan]]"
created: 2024-11-13
published: 2023-07-30
description: "Hey there, I am currently trying to find a good way to mock our drizzle instance for our unit test suite, but the nature of the usage of it makes it kinda hard. Is there somebody who is running a code base with a mocked drizzle?"
tags:
  - "clippings"
---
Hey there, I am currently trying to find a good way to mock our drizzle instance for our unit test suite, but the nature of the usage of it makes it kinda hard. Is there somebody who is running a code base with a mocked drizzle?

Just sharing this if any helpful to anyone: I ended up using in-memory db from @electric-sql/pglite instead of mocking. So even if I am using "drizzle-orm/node-postgres" in my actual application, tests are working as expected with "Pglite"

```javascript
import { PGlite } from "@electric-sql/pglite";
import { drizzle } from "drizzle-orm/pglite";
import { migrate } from "drizzle-orm/pglite/migrator";
import path from "path";
import * as clientSchema from "../src/drizzle/schema/clients";
import * as usersSchema from "../src/drizzle/schema/users";

export const testDB = async () => {  const sqlite = new PGlite();

const db = drizzle(sqlite, { schema: { ...clientSchema, ...usersSchema } });
const migrationPath = path.join(process.cwd(),"src/drizzle/migrations");  await migrate(db, { migrationsFolder: migrationPath });
return { dblite: db };};
```