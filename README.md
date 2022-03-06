# Homework | VS code debug

# Task

```txt
1. Разобраться как работает Debug в VS Code
2. Настроить дебаггер для отладки приложения
3. Тестировщики нашли проблему, что если делается запрос на получение одной манги,
   то она всегда обновляется и выводиться сообщение что манга обновлена. 
   Нужно найти строчку кода, в которой написана неправильная логика. 
   
   (Для тестирования используйте данный 
   URL - http://127.0.0.1:8000/api/manga/875/ )
   !!!(Подсказка - нужно удалить только одну строчку)
```

## Starting

```bash
pip install poetry
poetry install
poetry shell
```


## Usage

```bash
python3 manage.py runserver
```

### In browser
```bash
# Admin

# Login: admin
# Password: admin
http://localhost:8000

# API
http://127.0.0.1:8000/api/manga/875/
# First response can be with message that manga is update
# so you need to make reload after that message.
# CTRL + R
```