# db\_home\_tasks

## Описание проекта

Этот репозиторий представляет собой коллекцию SQL-скриптов, предназначенных для выполнения учебных заданий по работе с базами данных (PostgreSQL).

Проект разделён на четыре независимые группы задач:
**t1\_transport**, **t2\_racing**, **t3\_hotels**, **t4\_organization**, каждая из которых содержит собственный набор скриптов для создания структуры базы данных, заполнения её данными и их последующей обработки.

## 1. Описание проекта

- **Цель**: Отработка навыков составления SQL-запросов, проектирования и заполнения таблиц, а также выполнения специфических операций в рамках учебных задач.
- **Задача**: Продемонстрировать навыки работы с SQL-запросами, полученных в рамках изучения модуля "Базы данных"
- **СУБД**: Проект реализован на СУБД PostgreSQL (от 12 и выше).
- **Состав**: В каждой папке (t1_transport, t2_racing, t3_hotels, t4_organization) содержится один файл инсталляции для создания и наполнения базы (`[directory_name]_install.sql`) и файлы с решениями заданий (`[directory_name]_task_n.sql`) в рамках ДЗ.

## 2. Структура проекта

Ниже представлена структура папок и файлов:

```
db_home_tasks
│  
├── t1_transport
│   ├── t1_transport_install.sql
│   ├── t1_transport_task_1.sql
│   └── t1_transport_task_2.sql
├── t2_racing
│   ├── t2_racing_install.sql
│   ├── t2_racing_task_1.sql
│   ├── t2_racing_task_2.sql
│   ├── t2_racing_task_3.sql
│   ├── t2_racing_task_4.sql
│   └── t2_racing_task_5.sql
├── t3_hotels
│   ├── t3_hotels_install.sql
│   ├── t3_hotels_task_1.sql
│   ├── t3_hotels_task_2.sql
│   └── t3_hotels_task_3.sql
└── t4_organization
    ├── t4_organization_install.sql
    ├── t4_organization_task_1.sql
    ├── t4_organization_task_2.sql
    └── t4_organization_task_3.sql
```

### Краткое описание содержимого папок

- **t1\_transport**

    - `t1_transport_install` – скрипт создания и наполнения базы данных транспортных средств.
    - `t1_transport_task_1`, `t1_transport_task_2` – SQL-скрипты с решениями задач.

- **t2\_racing**

    - `t2_racing_install` – скрипт создания и наполнения базы данных автомобильных гонок.
    - `t2_racing_task_1`, `t2_racing_task_2`,
    - `t2_racing_task_3`, `t2_racing_task_4`,
    - `t2_racing_task_5` – SQL-скрипты с решениями задач.

- **t3\_hotels**

    - `t3_hotels_install` – скрипт создания и наполнения базы данных бронирований отелей.
    - `t3_hotels_task_1`, `t3_hotels_task_2`, `t3_hotels_task_3` – SQL-скрипты с решениями задач.

- **t4\_organization**

    - `t4_organization_install` – скрипт создания и наполнения базы данных структур организаций.
    - `t4_organization_task_1`, `t4_organization_task_2`, `t4_organization_task_3` – SQL-скрипты с решениями задач.

## 3. Инструкция по запуску

1. **Создайте базу данных (если ещё не создана).**

   ```sql
   CREATE DATABASE mydatabase;
   ```

   Вы можете задать свое название базы данных (например, `mydatabase`).

2. **Подключитесь к созданной базе данных.**

   ```bash
   psql -U postgres -d mydatabase
   ```

3. \*\*Выполните скрипт \*\***`[directory_name]_install.sql`** (например, `[directory_name]_task_n.sql`) для создания и наполнения таблиц в ранее созданную БД.

4. **Запустите SQL-скрипты с решениями задач** (например, `[directory_name]_task_n.sql` и последующие).

5. **Проверьте результаты.**

    - Убедитесь, что все таблицы и данные созданы правильно.
    - Запросы выполняются корректно и возвращают ожидаемые результаты.

