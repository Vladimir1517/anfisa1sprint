# Анфиса для друзей

## Установка окружения 
### Склонируйте проект «Анфиса для друзей» в папку *Dev/*.

Должна получиться такая структура:

```
Dev/
 └── anfisa1sprint/
     ├── anfisa_for_friends/
     ├── html_templates/
     ├── .gitignore
     ├── LICENSE
     ├── requirements.txt
     └── README.md
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
    ├── html_templates/
    ├── venv/   
    ├── .gitignore
    ├── LICENSE
    ├── requirements.txt
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
    

Теперь все команды в терминале будут предваряться строкой `(venv)`.

💡 Все дальнейшие команды в терминале надо выполнять с активированным виртуальным окружением.

Обновите pip:

```bash
python -m pip install --upgrade pip
```

### Установка зависимостей из файла *requirements.txt*:
Находясь в папке *Dev/anfisa1sprint/*, выполните команду:

```bash
pip install -r requirements.txt
```

### Применение миграций

    
В директории с файлом manage.py выполните команду: 

```bash
python manage.py migrate
```

### Запуск проекта в dev-режиме

    
В директории с файлом manage.py выполните команду: 

```bash
python manage.py runserver
```

В ответ Django сообщит, что сервер запущен и проект доступен по адресу [http://127.0.0.1:8000/](http://127.0.0.1:8000/). 
