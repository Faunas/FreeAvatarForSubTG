# Telegram Bot — Уникальные Аватарки за Подписку  


## 📌 Описание проекта  

**Telegram-бот** для генерации **уникальных аватарок** на основе предпочтений пользователя.  
Для получения аватарки пользователь должен подписаться на указанный Telegram-канал.  

📌 **Ботом воспользовались уже более 50 000 человек!**  

## 🚀 Функционал  

✔ **Подписка на канал** — обязательное условие для использования бота.  
✔ **Выбор стиля** аватарки из предустановленных шаблонов.  
✔ **Настройка цветовой гаммы** для персонализации аватарки.  
✔ **Ввод никнейма**, который будет добавлен на изображение.  
✔ **Подтверждение выбора** перед окончательной генерацией.  
✔ **Получение аватарки** в высоком качестве прямо в чате с ботом.  
✔ **Лимиты**: Одна аватарка каждые 24 часа.  
✔ **Реферальная система**: Снятие лимита за приглашение друга.  

## 🖼 Скриншоты 

1. **Обязательная подписка**
   <br>
   ![Обязательная подписка](git_img/subscribe_start.png)

2. **Выбор аватарки**
   <br>
   ![Выбор аватарки](git_img/choose_avatar.png)

3. **Выбор цвета**
   <br>
   ![Выбор цвета](git_img/choose_color.png)

4. **Выбор никнейма**
   <br>
   ![Выбор никнейма](git_img/choose_nickname.png)
   
5. **Подтверждение введенных данных**
   <br>
   ![Подтверждение](git_img/check_info.png)

6. **Уведомление после подтверждения**
   <br>
   ![Ожидание](git_img/wait_please.png)

7. **Готовая аватарка по заданным критериям отправляется файлом**
   <br>
   ![Готовая аватарка](git_img/result_ava.png)

8. **Ограничения на 4 аватарки в день**
   <br>
   ![Выбор никнейма](git_img/restrict_ava_4.png)
   
9. **Реферальная система**
   <br>
   ![Рефка](git_img/refferal_system_info.png)

## 📂 Структура проекта

```plaintext
PostgreAvatarTGBotAlchemy/
│── BASIC_HALLOWEEN_NEWYEAR_SQLALCHEMY_POSTGRESQL/
│   ├── database/                   # Работа с базой данных
│   │   ├── models.py               # Определение моделей БД
│   │   ├── session.py              # Настройки сессии SQLAlchemy
│   │   ├── settings.py             # Конфигурация базы данных
│   │
│   ├── ImageEngine/                 # Движок обработки изображений
│   │   ├── all_avatars_templates/   # Шаблоны аватарок
│   │   ├── all_fonts/               # Шрифты для аватарок
│   │   ├── ImageEngine/             # Модули обработки изображений
│   │   │   ├── __init__.py
│   │   │   ├── change_psd_basic.py  # Базовая генерация PSD
│   │   │   ├── change_psd_halloween.py  # Хэллоуинские аватарки
│   │   │   ├── change_psd_new_year2025.py  # Новогодние аватарки
│   │   │   ├── core.py               # Основная логика обработки
│   │
│   ├── KonkursEngine/               # Модуль конкурсов
│   │   ├── konkurs_handlers.py      # Обработчики команд конкурса
│   │   ├── konkurs_requests.py      # Запросы в БД для конкурса
│   │
│   ├── lkEngine/                     # Личный кабинет
│   │   ├── generate_csv.py          # Генерация CSV-файлов
│   │   ├── lk.py                    # Основная логика ЛК
│   │   ├── lk_utils.py              # Вспомогательные утилиты для ЛК
│   │
│   ├── ReferralEngine/               # Реферальная система
│   │   ├── ref_handlers.py          # Обработчики рефералов
│   │   ├── ref_requests.py          # Запросы к БД рефералов
│   │
│   ├── .env                          # Конфигурационный файл
│   ├── bot_instance.py               # Инициализация бота
│   ├── config.py                      # Конфигурация проекта
│   ├── database_requests.py          # Общие запросы к БД
│   ├── dispatcher.py                 # Диспетчер команд
│   ├── KeyboardMarkups.py            # Inline-кнопки
│   ├── logger.py                      # Логирование
│   ├── requirements.txt               # Список зависимостей
│   ├── semaphore_restrict.py          # Ограничения доступа
│   ├── start.py                       # Точка входа в проект
│   ├── states.py                      # FSM состояния
│   ├── subscribeEngine.py             # Проверка подписок
│   ├── utils.py                       # Вспомогательные функции
```

## 🛠 Технологии  

- **Python** — основной язык разработки  
- **aiogram** — асинхронная работа с Telegram API  
- **PostgreSQL** — база данных  
- **SQLAlchemy** — ORM для взаимодействия с БД  
- **Pillow** — обработка изображений  
- **asyncio** — асинхронная работа  


