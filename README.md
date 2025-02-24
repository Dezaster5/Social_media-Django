# Django Social Network Project

## Описание
Это проект социальной сети, разработанный на Django. Основной функционал включает пользовательскую аутентификацию, социальный вход через Google и Facebook, управление профилями пользователей, подписки, подсчет просмотров и рейтинг самых популярных записей.

## Основные возможности
- **Управление пользователями**
  - Регистрация, вход и выход пользователей.
  - Смена и сброс пароля через встроенный механизм Django.
  - Расширенная модель профиля пользователя.
  - Запрет на регистрацию с существующим адресом электронной почты.

- **Социальная аутентификация**
  - Интеграция социальных сетей (Google и Facebook) с использованием модуля `Python Social Auth`.
  - Автоматическое создание профилей для пользователей, зарегистрировавшихся через социальные сети.

- **Интерактивный контент**
  - Подписка на обновления пользователей.
  - Подсчет просмотров записей с использованием Redis.
  - Рейтинг самых популярных записей.

- **Медиафайлы**
  - Конфигурация загрузки пользовательских медиафайлов (изображения и т.д.).
  - Генерация миниатюр изображений с помощью `easy-thumbnails`.

- **Асинхронное взаимодействие**
  - Реализация бесконечной прокрутки для ленты новостей.
  - Асинхронные HTTP-запросы с использованием JavaScript и Django.

## Установка
1. Клонируйте репозиторий:
   ```bash
   git clone https://github.com/Dezaster5/Social_media-Django.git
   cd <имя папки>
   ```

2. Установите зависимости:
   ```bash
   pip install -r requirements.txt
   ```

3. Выполните миграции:
   ```bash
   python manage.py migrate
   ```

4. Настройте переменные окружения для социальных провайдеров (Facebook, Google) и Redis.

5. Запустите сервер разработки:
   ```bash
   python manage.py runserver
   ```

## Используемые технологии
- Django
- Redis
- Python Social Auth
- Easy-thumbnails
- JavaScript (для динамического взаимодействия)
