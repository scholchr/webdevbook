# Python

## pip

* `pip install -r requirements.txt`
* `pip freeze > requirements.txt`
* `pip install --upgrade PACKAGENAME`
* `pip list --outdated --format=freeze`

## Nützliche Python Packages (systemweit installieren)

### [VirtualEnvWrapper](https://github.com/davidmarble/virtualenvwrapper-win)

* Make sure `C:\Python3x\Scripts` is in your $PATH
* `pip install virtualenvwrapper-win`
* Commands:
    * `mkvirtualenv`
    * `lsvirtualenv`
    * `rmvirtualenv`
    * `workon`
    * `deactivate`

### pigar

A fantastic tool to generate requirements for your Python project:

* TODO: testen, ob pigar möglicherweise pip-upgrade ersetzt
* `pigar` Standardaktion: `requirements.txt` generieren und diff ausgeben
* `pigar -p requirements2.txt` Ausgabe in angegebener Datei speichern
* `pigar -s win32api` sucht Python Package nach Importname
* `pigar -c` überprüft `requirements.txt` auf Aktualisierungen
* `pigar -u` pigar Datenbank aktualisieren

## VSCode Integration

* To select a specific environment, use the **Python: Select Interpreter** command from the Command Palette (`Ctrl+Shift+P`).

## [f-strings](https://www.python.org/dev/peps/pep-0498/) (3.6+)

Anstatt `format`:
```python
user = "Jane Doe"
action = "buy"
log_message = f'User {user} has logged in and did an action {action}.'
print(log_message)
# User Jane Doe has logged in and did an action buy.
```

## [pathlib](https://docs.python.org/3/library/pathlib.html) (3.4+)

* Anstatt `os.path`
* [Why you should be using pathlib](https://treyhunner.com/2018/12/why-you-should-be-using-pathlib/)


