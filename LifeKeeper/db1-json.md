### Задача: Хранение задач в JSON-файле

Мы сделали таск-трекер, который хранит задачи в памяти (словарике Python). Но при перезапуске программы все задачи пропадают. Теперь давай добавим возможность сохранять данные в файл, чтобы задачи сохранялись даже после закрытия программы.

---

### Цель задачи:

1. Реализовать сохранение задач в файл формата JSON.
2. При запуске программы загружать задачи из файла.
3. Протестировать новую логику и убедиться, что задачи сохраняются корректно.

---

### Шаги к выполнению:
- Создай файл `tasks.json` в корне проекта.
- В конце каждой операции с задачами (например, добавление, редактирование, удаление) сохраняй данные из словарика в файл `tasks.json`. Используй встроенный модуль `json` для сериализации данных.
- При старте программы проверяй, существует ли файл `tasks.json`. Если файл существует, загружай задачи из него.

### Что делать, если возникнут вопросы:
- Если что-то непонятно с модулем `json`, посмотри документацию Python: [https://docs.python.org/3/library/json.html](https://docs.python.org/3/library/json.html).
- Если файл не создается или не загружается, проверь права на запись в папке проекта.
- Если застрял — спроси умного помощника! 😊

После выполнения у нас будет таск-трекер, который сохраняет задачи даже после закрытия программы.