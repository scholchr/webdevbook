```eval_rst
:github_url: https://github.com/scholchr/webdevbook/tree/master/source/python.md
```

# Python

## [VirtualEnvWrapper](https://github.com/davidmarble/virtualenvwrapper-win)

* Make sure `C:\Python3x\Scripts` is in your $PATH
* `pip install virtualenvwrapper-win`
* Commands:
    * `mkvirtualenv`
    * `lsvirtualenv`
    * `rmvirtualenv`
    * `workon`
    * `deactivate`

## pip

* `pip install -r requirements.txt`
* `pip freeze > requirements.txt`
* `pip list --outdated --format=freeze`

## pip-upgrade

* `pip install pip-upgrader`
* `pip-upgrade`

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


