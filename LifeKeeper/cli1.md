Хотим сделать приложение таск трекер

  

Референс:

  

https://github.com/user-attachments/assets/6e2622b6-cec3-46f8-bd35-dc2c760b33b0

  

Первым шагом давайте сделаем MVP (минимально рабочий прототип), работающий в командной строке (CLI).

  

Первым делом откройте вашу любимую среду разработки, рекомендую PyCharm.

  

Дальше настройте виртуальное окружение venv для установки библиотек. Это позволит устанавливать пакеты через `pip install`, и завести файл с зависимостями `requirements.txt`.

  

После этого можете приступать к разработке. Шаг за шагом реализуйте программу таск трекера, которая будет прямо в терминале взаимодействовать с пользователем в текстовом виде. То есть при запуске `python main.py` должна работать логика на экранах ниже:

  

**Главное меню:**

```

=========================

TASK-TRACKER

=========================

1. Добавить задачу

2. Просмотреть задачи

3. Редактировать задачу

4. Удалить задачу

5. Управление разделами

6. Выход

Выберите опцию (1-6):

```

  

**Добавление задачи:**

```

--- Добавить новую задачу ---

Введите описание задачи: Купить молоко

Выберите раздел:

1. Дом

2. Учёба

3. Хобби

Введите номер раздела: 1

Установить дату выполнения (ДД.ММ.ГГГГ) или оставить пустым: 25.12.2024

Повторять задачу? (нет/каждые 3 дня): каждые 3 дня

Задача успешно добавлена!

Нажмите Enter, чтобы вернуться в главное меню.

```

  

**Просмотр задач:**

```

--- Список задач ---

1. [ ] Купить молоко (Дом) - до 25.12.2024 - Повторять каждые 3 дня

2. [x] Выполнить домашнее задание (Учёба) - до 20.12.2024

3. [ ] Практиковаться в рисовании (Хобби) - до 30.12.2024

-----------------------

Выберите задачу для редактирования или удаления, или нажмите Enter для возврата.

```

  

**Удаление задачи:**

```

--- Удалить задачу ---

Введите номер задачи для удаления: 2

Вы уверены, что хотите удалить задачу "Выполнить домашнее задание"? (да/нет): да

Задача успешно удалена!

Нажмите Enter, чтобы вернуться в главное меню.

```

  

**Управление разделами:**

```

--- Управление разделами ---

1. Добавить раздел

2. Просмотреть разделы

3. Редактировать раздел

4. Удалить раздел

5. Вернуться в главное меню

Выберите опцию (1-5):

```

  
  

**Технические детали:**

- Пока хранение данных делаем просто в Python словарике в памяти. То есть если программа перезапустится, данные потеряются. Дальше будем пристраивать базу данных, позже