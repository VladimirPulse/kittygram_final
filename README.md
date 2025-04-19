# kittygram_final - площадка для размещения своих любимых животных

<img width="884" alt="image" src="https://github.com/user-attachments/assets/c03243e5-801a-4c25-8803-dc2744216e32" />

---

### Стек технологий:
Python, Django REST Framework, Docker, Docker Compose, SQLite, PostgreSQL, Nginx, GitHub Actions, React

---

### Инструкция по развертыванию:
**Клонируйте репозиторий:**

```
git clone git@github.com:shft1/CuteCat.git
```

**Cоздайте и активируйте виртуальное окружение:**

```
python3 -m venv venv
```

* _Если у вас Linux/macOS_

    ```
    source venv/bin/activate
    ```
* _Если у вас Windows_

    ```
    source venv/scripts/activate
    ```

**Установите зависимости из файла requirements.txt:**

```
pip install -r requirements.txt
```

**Заполните файл .env в директории `backend` :**
```
POSTGRES_DB - имя базы данных (если не указать, то БД - SQLite)
POSTGRES_USER - имя пользователя с правами к базе
POSTGRES_PASSWORD - пароль пользователя
DB_NAME - имя контейнера, в котором запущена СУБД
DB_PORT - порт, на котором работает контейнер с СУБД
SECRET_KEY - для секретного ключа
DEBUG - что включения режима отладки значение True/true
ALLOWED_HOSTS - разрешенные хосты
```

**Запустите приложение CuteCat командой:**
```
docker compose up
```

---

### Дополнительные возможности для разработчиков

Пуш в ветку main запускает CI/CD (тестирование и деплой) Kittygram, а после успешного деплоя вам приходит сообщение в телеграм.

---

### Автор 
Этот проект был разработан Кулаковым В.С., 
Контакт: VrachKulakovVS@mail.ru.
