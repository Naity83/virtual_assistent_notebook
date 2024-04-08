# Проект "Імплементація боту та сортування файлів"

Цей проект містить бота для управління адресною книгою, управління нотатками та інструмент для автоматичного сортування файлів.

## Вміст

1. [Структура проекту](#структура-проекту)
2. [Опис](#опис)
3. [Встановлення](#встановлення)
4. [Використання](#використання)

<a name='структура-проекту'></a>

### Структура проекту

<pre>
personal-notebook/
├── LICENSE
├── MANIFEST.in
├── README.md
├── requirements.txt
├── setup.py
├── contacts.json
├── notes.json
├── .gitignore
├── personal_assistant2/
│   ├── __init__.py
│   ├── main.py
│   ├── bot.py
│   ├── classes.py
│   ├── colors.py
│   ├── comands.py
│   ├── notes.py
│   ├── sorted.py
│   ├── contacts.json
│   └── notes.json
└── tests/
</pre>

<a name='опис'></a>

## Опис

### bot.py

Файл `bot.py` містить реалізацію бота для управління адресною книгою.

### main.py

Головний файл `main.py`, який запускає бота.

### notes.py

Модуль `notes.py` містить функції для роботи з нотатками, такі як додавання, редагування та видалення.

### sorted.py

У файлі `sorted.py` реалізовано інструмент для сортування файлів за категоріями.

### colors.py

У файлі `colors.py` визначені константи для кольорів консольного виведення.

### classes.py

Модуль `classes.py` включає в себе класи для роботи з контактами та адресною книгою.

<a name='встановлення'></a>

## Встановлення

| Встановлення                        | Windows                           | Linux                              |
| ----------------------------------- | --------------------------------- | ---------------------------------- |
| 1. Створити віртуальне середовище   | py -m venv .venv                  | python3 -m venv .venv              |
| 2. Активувати віртуальне середовище | .venv\Scripts\Activate.ps1        | source .venv/bin/activate          |
| 3. Перевірка встановлених пакетів   | pip list                          | pip3 list                          |
| 4. Встановлення пакету              | pip install -e .                  | pip3 install -e .                  |
| 5. Запуск бота-асистента            | run-assistant                     | run-assistant                      |
| Видалення пакету                    | pip uninstall personal-assistant2 | pip3 uninstall personal-assistant2 |
| Деактивація віртуального середовищя | deactivate                        | deactivate                         |

<a name='використання'></a>

## Використання

### Запуск бота

Використовуйте команду:
`run-assistant`

Після запуску ви побачите команди:

- **hello** - Вивести привітальне повідомлення.
- **add** - Додати новий контакт. Потрібно вказати ім'я та інші дані.
- **change** - Змінити ім'я контакту. Потрібно вказати старе та нове ім'я.
- **phone** - Змінити телефонний номер контакту. Потрібно вказати ім'я та новий номер.
- **email** - Змінити електронну пошту контакту. Потрібно вказати ім'я та нову пошту.
- **show all** - Показати всі доступні контакти.
- **search** - Пошук контакту за ім'ям чи номером телефону.
- **good bye, close, exit** - Вийти з програми.
- **sorted** - Сортувати файли в папці.
- **notes** - Запустити функціонал для роботи з нотатками.

### Сортування файлів

Використовуйте команду:
`python sorted.py Шлях_до_папки`

### Вийнятки та Керування Помилками

Бот має вбудовану систему виправлення помилок, тому слід слідкувати за виведеними повідомленнями та дотримуватися вказівок.

**Тепер ви готові використовувати бота! Бажаємо вам приємного користування та успішної роботи з вашим проектом.**