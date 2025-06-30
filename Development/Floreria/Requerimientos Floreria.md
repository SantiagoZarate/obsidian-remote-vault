## 📄 Documento De Requisitos Del Proyecto De Software

### 1. Información General
- **Nombre del Proyecto:** Plataforma Digital - Las Flores De La Imprenta
- **Fecha:** 16/05/2025
- **Versión del Documento:** 1.0
- **Responsable del relevamiento:** Santiago Zarate y Felipe García

---

### 2. Objetivo Del Proyecto

El objetivo del proyecto es desarrollar una plataforma digital que permita a la florería automatizar procesos clave como la compra de ramos de flores, Además, se implementará un sistema de membresías personalizadas, en el cual los clientes podrán suscribirse a distintos niveles de membresía, cada uno con beneficios exclusivos como descuentos o productos especiales. La plataforma busca mejorar la eficiencia operativa del negocio y ofrecer una experiencia de compra más simple, ágil y atractiva para sus clientes.

Además, se implementará un sistema de referidos exclusivo para las membresías más premium. Los usuarios que adquieran estos planes podrán generar un enlace único de referido. Cuando una persona nueva se registre y adquiera una membresía a través de dicho enlace, el usuario que refirió recibirá un porcentaje de la transacción como beneficio acumulable en su cuenta.

---

### 3. Alcance Del Proyecto

El proyecto incluirá el desarrollo de un sistema web que permita a los clientes de la florería:

**Incluye**

- Explorar y seleccionar diferentes tipos de ramos de flores y productos disponibles
- Realizar compras en línea mediante una interfaz intuitiva y segura.
- Personalizar pedidos, como la selección de flores específicas o mensajes para incluir en el ramo.
- Acceder a un sistema de membresías, con distintos planes y beneficios asociados (como descuentos, acceso prioritario a productos exclusivos o promociones especiales).
- Administrar su cuenta, historial de pedidos y detalles de membresía desde un panel de usuario.
- Ver reportes acerca de los usuarios que obtuvieron ingresos a partir de los links de referidos

**No Incluye**

- funcionalidades relacionadas con la logística o el envío de entregas. Las entregas deberán gestionarse por otros medios fuera del alcance de este proyecto.

---

### 4. Público Objetivo

El sistema está dirigido a un público amplio que incluye:

- **Clientes particulares**, que desean comprar ramos o arreglos florales de forma puntual o suscribirse a una membresía para recibir beneficios exclusivos.

- **Pequeñas y medianas empresas (PyMEs)**, interesadas en servicios recurrentes como decoración floral para oficinas, eventos corporativos o regalos empresariales.

- **Grandes empresas**, que requieren soluciones personalizadas y automatizadas para pedidos a gran escala, armado de pedidos programados y beneficios corporativos a través del sistema de membresías.

---

### 5. Roles Y Permisos

- **Visitante:**
    Usuario sin registro o sin membresía activa. Puede navegar por la tienda, explorar los ramos y arreglos florales disponibles, pero no tiene acceso a beneficios exclusivos ni a la funcionalidad completa del sistema (como pedidos automáticos, descuentos, o programa de referidos).

- **Miembro:**
    Usuario registrado que ha adquirido una membresía. Existen tres niveles:
    - **Low Ticket:** Acceso básico a beneficios como descuentos moderados en productos.
    - **Medium:** Beneficios intermedios que incluyen mayores descuentos, contenido exclusivo y acceso anticipado a productos especiales.
    - **Business:** Nivel premium pensado para clientes frecuentes o corporativos. Incluye todos los beneficios anteriores más la posibilidad de generar enlaces de referidos que otorgan comisiones por nuevas membresías adquiridas a través de su link.

- **Admin:**
    Usuario con permisos completos sobre el sistema. Puede gestionar usuarios, productos, membresías, estadísticas, pedidos y beneficios. También tiene control sobre la configuración general de la plataforma y el monitoreo de las actividades de referidos.

## Permisos Por Rol (Propuesta)

| Funcionalidad                                         | Visitante | Miembro Low Ticket | Miembro Medium | Miembro Business | Admin |
| ----------------------------------------------------- | :-------: | :----------------: | :------------: | :--------------: | :---: |
| Navegar el catálogo de productos                      |     ✅     |         ✅          |       ✅        |        ✅         |   ✅   |
| Realizar compras sin membresía                        |     ✅     |         ✅          |       ✅        |        ✅         |   ✅   |
| Acceder a descuentos exclusivos                       |     ❌     |    ✅ (básicos)     |  ✅ (mayores)   |   ✅ (premium)    |   ✅   |
| Acceder a contenido exclusivo                         |     ❌     |         ❌          |       ✅        |        ✅         |   ✅   |
| Acceso anticipado a productos/colecciones             |     ❌     |         ❌          |       ✅        |        ✅         |   ✅   |
| Generar enlace de referido                            |     ❌     |         ❌          |       ❌        |        ✅         |   ✅   |
| Ver estadísticas de referidos                         |     ❌     |         ❌          |       ❌        |        ✅         |   ✅   |
| Gestionar suscripciones/membresías propias            |     ❌     |         ✅          |       ✅        |        ✅         |   ✅   |
| Personalizar ramos o pedidos                          |     ✅     |         ✅          |       ✅        |        ✅         |   ✅   |
| Ver historial de pedidos                              |     ❌     |         ✅          |       ✅        |        ✅         |   ✅   |
| Gestionar productos y catálogo                        |     ❌     |         ❌          |       ❌        |        ❌         |   ✅   |
| Administrar membresías                                |     ❌     |         ❌          |       ❌        |        ❌         |   ✅   |
| Gestionar usuarios y roles                            |     ❌     |         ❌          |       ❌        |        ❌         |   ✅   |
| Ver reportes del sistema (ventas, suscripciones, etc) |     ❌     |         ❌          |       ❌        |        ❌         |   ✅   |
| Configuración general de la plataforma                |     ❌     |         ❌          |       ❌        |        ❌         |   ✅   |
