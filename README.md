# FurryGallery

<br/>

[![Nginx](https://img.shields.io/badge/Nginx-1.22-blue?style=for-the-badge&labelColor=333333&logo=NGINX&logoColor=white)](https://nginx.org/ru/)
[![Docker](https://img.shields.io/badge/Docker-20.10.18-blue?style=for-the-badge&labelColor=333333&logo=Docker&logoColor=white)](https://www.docker.com/)
[![Docker-compose](https://img.shields.io/badge/Docker%20compose-2.10.0-blue?style=for-the-badge&labelColor=333333&logo=Docker&logoColor=white)](https://www.docker.com/)
[![Docker Hub](https://img.shields.io/badge/Docker%20Hub-latest-blue?style=for-the-badge&logo=Docker&logoColor=white&labelColor=333333)](https://www.docker.com/products/docker-hub)
[![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-Workflow-blue?style=for-the-badge&logo=GitHub%20actions&logoColor=white&labelColor=333333)](https://github.com/features/actions)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-13.1-blue?style=for-the-badge&labelColor=333333&logo=PostgreSQL&logoColor=white)](https://www.postgresql.org/)
[![gunicorn](https://img.shields.io/badge/gunicorn-20.1.0-blue?style=for-the-badge&labelColor=333333&logo=gunicorn&logoColor=white)](https://gunicorn.org/)
[![Django](https://img.shields.io/badge/Django-3.2.16-blue?style=for-the-badge&labelColor=333333&logo=django&logoColor=white&color=blue)](https://www.djangoproject.com/)
[![DRF](https://img.shields.io/badge/django--rest--framework-3.12.4-blue?style=for-the-badge&labelColor=333333&logo=django&logoColor=white&color=blue)](https://www.django-rest-framework.org/)
[![SimpleJWT](https://img.shields.io/badge/simplejwt-4.7.2-blue?style=for-the-badge&labelColor=333333&logo=django&logoColor=white&color=blue)](https://github.com/davesque/django-rest-framework-simplejwt)
[![PyJWT](https://img.shields.io/badge/PyJWT-2.1.0-blue?style=for-the-badge&labelColor=333333&logo=python&logoColor=white&color=blue)](https://github.com/jpadilla/pyjwt)
[![Djoser](https://img.shields.io/badge/djoser-2.1.0-blue?style=for-the-badge&labelColor=333333&logo=django&logoColor=white&color=blue)](https://github.com/sunscrapers/djoser)
[![Лицензия](https://img.shields.io/github/license/kluevevga/FurryGallery?color=blue&style=for-the-badge&labelColor=333333&logo=github)](https://github.com/kluevevga/FurryGallery/blob/master/LICENSE)
[![Размер кода](https://img.shields.io/github/languages/code-size/kluevevga/FurryGallery?style=for-the-badge&labelColor=333333&logo=github)](https://github.com/kluevevga/FurryGallery)

## О проекте

PrettyPets — это социальная сеть, созданная для обмена фотографиями и историями о вашей милой компании -
ваших питомцах. Проект объединяет бэкенд-приложение, основанное на Django, и фронтенд-приложение, разработанное на
React. Весь процесс развертывания проекта осуществляется на виртуальном удалённом сервере, используя три контейнера:
nginx, PostgreSQL и Django+Gunicorn. Заготовленный контейнер с фронтендом активно используется для сборки файлов, и
контейнер с проектом обновляется на Docker Hub.

PrettyPets предоставляет возможности:

* Регистрации новых пользователей.
* Добавления уникальных фотографий ваших питомцев.
* Удаления изображений питомцев по вашему желанию.
* Персонализации окраски и описания каждого питомца.
* Поделиться особенностями и достижениями вашего друга на четыре лапы.
* Указания года рождения каждого питомца.

FurryGallery, с другой стороны, является уютным уголком для всех, кто обожает кошек. Это специализированная социальная
сеть, где пользователи имеют возможность делиться фотографиями своих пушистых друзей и наслаждаться уникальными
фотографиями, опубликованными другими участниками. Проект активно использует GitHub Actions для автоматизации
тестирования и развертывания на сервере, что обеспечивает стабильное функционирование и удобство использования для
пользователей.

## Структура проекта 📁

- `kittygram_workflow.yml`: Этот файл содержит настройки для непрерывной интеграции и доставки (CI/CD), которые
  автоматизируют тестирование и развертывание проекта.


- `docker-compose.production.yml`: Здесь определены настройки для запуска проекта в производственной среде с
  использованием образов Docker из Docker Hub.


- `docker-compose.yml`: Этот файл содержит настройки для локальной разработки и тестирования проекта с локальной сборкой
  контейнеров Docker.


- `backend`: В этой директории находится бекенд-часть проекта, отвечающая за серверную логику и взаимодействие с базой
  данных.


- `frontend`: Здесь расположена фронтенд-часть проекта, написанная на React, которая обеспечивает пользовательский
  интерфейс и взаимодействие с бекендом.

## Запуск проекта 🚀

Для запуска проекта вам потребуется установить следующие компоненты: Node.js, Python и Pip.

### Frontend:

Для настройки фронтенд-части проекта выполните следующие шаги:

1. Клонирование проекта:

   ```shell
   git clone https://github.com/kluev-evga/FurryGallery.git
   ```

2. Перейдите в директорию фронтенда:

   ```shell
   cd frontend
   ```

3. Установите зависимости:

   ```shell
   npm install
   ```

4. Запустите фронтенд:

   ```shell
   npm run dev
   ```

После успешного выполнения этих шагов, вы получите доступ к React-приложению по
адресу [127.0.0.1:3000](https://127.0.0.1:3000).

### Backend:

Чтобы настроить бекенд-часть проекта, выполните следующие действия:

1. Клонирование проекта:

   ```shell
   git clone https://github.com/kluev-evga/FurryGallery.git
   ```

2. Перейдите в директорию бекенда:

   ```shell
   cd backend
   ```

3. Создайте виртуальное окружение:

   ```shell
   python3 -m venv venv
   ```

4. Активируйте виртуальное окружение (для Linux/macOS):

   ```shell
   source venv/bin/activate
   ```

   Для Windows:

   ```shell
   source venv/scripts/activate
   ```

5. Установите зависимости:

   ```shell
   pip install -r requirements.txt
   ```

6. Выполните миграции базы данных:

   ```shell
   python manage.py migrate
   ```

7. Запустите бекенд-приложение:

   ```shell
   python manage.py runserver
   ```

После успешного выполнения этих шагов, вы сможете использовать бекенд-приложение по
адресу [127.0.0.1:8000](https://127.0.0.1:8000).

## Автоматизация развертывания: CI/CD

Процесс автоматизации развертывания построен на основе CI/CD. Workflow настроен таким образом, что каждое обновление
ветки `master` служит событием-триггером для запуска тестирования и деплоя.

При возникновении события-триггера, GitHub Actions считывает файл с описанием workflow и назначает отдельный раннер для
каждой задачи-job в этом workflow. Эти раннеры выполняют соответствующие задачи, включая настройку Docker, сборку
образов и их загрузку на Docker Hub. После этого, на боевом сервере, производится перезапуск контейнеров, чтобы они были
обновлены из свежих образов.

Для выполнения этих операций, раннеру требуется аутентификация на Docker Hub, чтобы загрузить образы, а также
аутентификация на боевом сервере для перезапуска контейнеров. Конфиденциальные данные, такие как токены, пароли и другая
приватная информация, могут быть безопасно храниться в специальном хранилище на платформе GitHub Actions.

Эти конфиденциальные данные, называемые секретами (secrets), могут быть сохранены в разделе Secrets. Во время выполнения
workflow, значения из этого хранилища будут переданы в переменные, доступные только раннеру во время запуска workflow.

Для более надежного контроля над выполнением workflow в GitHub Actions, также подключен Telegram-бот для уведомлений и
мониторинга.

## Лицензия 📜

Этот проект распространяется под лицензией `MIT`. Дополнительную информацию можно найти
в [LICENSE](https://github.com/kluevevga/FurryGallery/blob/master/LICENSE).