## Create Enviroment

1- Create virtual enviroment inside a project

```bash
python -m venv venv
```

2 - Activate env mode

```bash
source venv/bin/active
```

3 - Install dependencies

```bash
pip install cowsay
```

4 - Freeze dependencies

```bash
pip freeze > requirements.txt
```

5 - Exit venv

```bash
deactivate
```

---

### List Installed Versions

```bash
pyenv versions
```

List Versions

```bash
pyenv install --list
```

install specific version

```bash
pyenv install 3.x.x
```
