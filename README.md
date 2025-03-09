# Students Database

Этот проект создает базу данных студентов и курсов, используя PostgreSQL. Данные загружаются из CSV-файлов и SQL-скриптов.

## Как использовать

1. **Восстановите базу данных из файла `students.sql`**:
   - Используйте команду:
     ```bash
     psql -U postgres -d students -f students.sql
     ```

2. **Запустите скрипт `insert_data.sh`**:
   - Скрипт `insert_data.sh` заполняет базу данных данными из CSV-файлов (`courses.csv` и `students.csv`).
   - Сделайте скрипт исполняемым:
     ```bash
     chmod +x insert_data.sh
     ```
   - Запустите скрипт:
     ```bash
     ./insert_data.sh
     ```

3. **Запустите скрипт `student_info.sh`**:
   - Скрипт `student_info.sh` выводит полезную информацию о студентах и курсах из базы данных.
   - Сделайте скрипт исполняемым:
     ```bash
     chmod +x student_info.sh
     ```
   - Запустите скрипт:
     ```bash
     ./student_info.sh
     ```

## Структура проекта

- `students.sql` — SQL-скрипт для создания структуры базы данных и таблиц.
- `insert_data.sh` — Bash-скрипт для вставки данных из CSV-файлов.
- `student_info.sh` — Bash-скрипт для вывода информации о студентах и курсах.
- `courses.csv` — CSV-файл с данными о курсах.
- `students.csv` — CSV-файл с данными о студентах.
- `README.md` — документация проекта.

