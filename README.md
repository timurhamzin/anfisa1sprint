# Анфиса для друзей

## Установка окружения 
### Склонируйте проект «Анфиса для друзей» в папку *Dev/*.

Должна получиться такая структура:

```
Dev/
 └── anfisa1sprint/
     ├── anfisa_for_friends/
     ├── html_templates/
     ├── tests/
     ├── .gitignore
     ├── LICENSE
     ├── pytest.ini  
     ├── requirements.txt
     └── READ.ME
```

### Создайте виртуальное окружение

1. Запустите редактор Visual Studio Code и через меню «*Файл» / «Открыть директорию»* откройте папку *Dev/anfisa1sprint/*. 
2. Запустите терминал в VS Code, удостоверьтесь, что вы работаете из директории *anfisa1sprint/* (если вы работаете под Windows, убедитесь, что в терминале запущен Git Bash, а не PowerShell или что-нибудь ещё), и выполните команду:
- Linux/macOS
    
    ```bash
    python3 -m venv venv
    ```
    
- Windows
    
    ```python
    python -m venv venv
    ```
   
В директории *anfisa1sprint/* будет развёрнуто виртуальное окружение и появится папка `venv`, в которой будут храниться все зависимости проекта, а структура файлов станет такой:

```

Dev/
└── anfisa1sprint/
    ├── anfisa_for_friends/
    ├── tests/
    ├── venv/   
    ├── .gitignore
    ├── LICENSE
    ├── pytest.ini  
    ├──  requirements.txt
    └── README.md
```

### Активация виртуального окружения
в терминале перейдите в корневую директорию проекта *Dev/anfisa1sprint/* и выполните команду:
- Linux/macOS
    
    ```bash
    source venv/bin/activate
    ```
    
- Windows
    
    ```bash
    source venv/Scripts/activate
    ```
    

Теперь все команды в терминале будут предваряться строкой `(venv)`:

```bash
(venv) ...$

# В зависимости от настроек вашей системы 
# строка ввода может выглядеть чуть иначе.
# Например, так:
(venv) username@computer-name /directory-name$
# username — имя пользователя
# computer-name — название компьютера
# /directory-name — текущая директория
```


💡 Все дальнейшие команды в терминале надо выполнять с активированным виртуальным окружением.

### Установка зависимостей из файла *requirements.txt*:
Находясь в папке *Dev/anfisa1sprint/*, выполните команду:

```bash
pip install -r requirements.txt
```

### Запуск проекта в dev-режиме

    
В директории с файлом manage.py выполните команду: 

```bash
python manage.py runserver
```

Возможно, в вашей операционной системе нужна немного другая команда:

```bash
python3 manage.py runserver
```

В ответ Django сообщит, что сервер запущен и проект доступен по адресу [http://127.0.0.1:8000/](http://127.0.0.1:8000/). 

Дополнительно Django укажет на 18 каких-то недоделок, *unapplied migration(s)*. Для 
выполнения текущих задач этой фразуой можно пренебречь.


### Тестрвоание проекта:

После выполения задания перейдите в терминале в директорию Django-проекта (в ней лежит файл manage.py) и выполните команду pytest. 
