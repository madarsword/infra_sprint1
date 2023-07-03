
# **DevOps** для самых маленьких

## Деплой проекта **Kittygram** на удалённый сервер
###  **Kittygram** — социальная сеть для обмена фотографиями любимых питомцев. Это полностью рабочий проект, который состоит из бэкенд-приложения на **Django** и фронтенд-приложения на **React**.

### Описание:
#### Приложение **Kittygram** — социальная сеть для обмена фотографиями любимых питомцев. При подключении к приложению можно:
- зарегистрироваться и авторизоваться;
- добавить нового питомца на сайт или изменить существующего;
- просмотреть записи других пользователей.

### Запуск проекта *backend*:
Клонируйте проект: 
> *git clone git@github.com:madarsword/infra_sprint1.git*

При необходимости установите и активируйте виртуально окружение: 
> *python(3) -m venv venv*

> *source venv/bin/activate*

Установите зависимости: 
> *pip install -r requirements.txt*

Произведите миграции: 
> *python manage.py migrate*

Запустите отладочный веб-сервер Django: 
> *python manage.py runserver*

### Запуск проекта *frontend*:
Установите пакетный менеджер:
> *curl -fsSL https://deb.nodesource.com/setup_18.x* *|* *sudo -E bash - &&\*

> *sudo apt-get install -y nodejs*

Установите зависимости для фронтенд-приложения, для этого нужно перейти в директорию frontend/ и ввести команду:
> *npm i*

Запуск осуществляется командой:
> *npm run start*

### При подключении к Kittygram доступны все возможности проекта: можно зарегистрироваться и авторизоваться, добавить нового котика на сайт или изменить существующего, а также просмотреть записи других пользователей.

### Для взаимодействия с приложением через **API** предусмотрены следующие методы:
- добавить питомца: POST /cats/add
- редактировать информацию о питомце: PUTCH /cats/edit
- просмотр питомца: GET /cats/{cat_id}
