# <u>Инструкция для работы с Git и удаленными репозиториями.</u>

* ## __*Создаем папку на рабочем столе*__
  1. Переходим в директорию рабочего стола
  2. Создаём папку --> mkdir Git_test

* ## __*Создаем файл*__ instructions_Git __*в *папке*__ Git_test __*и сразу записываем в него текст:*__
     * echo "# <u>Инструкция для работы с Git и удаленными репозиториями.</u>" > Git_test/instructions_Git.md
     
* ## __*Переходим в папку Git_test инициализируем её проводим некоторые манипуляции*__
  1. Переходим в папку --> cd Git_test
  2. Смотрим содержимое --> ls -a
  3. Инициализируем репозиторий --> git init
  4. Смотрим содержимое --> ls -a
  5. Проверяем статус --> git status
  6. Сохраняем изменения в git --> git add instructions_Git.md
  7. Проверяем статус --> git status
  8. Создаём первый комит --> git commit -m "Initial commit"
  9. Смотрим лог --> git log
  10. Смотрим содержимое файла --> cat instructions_Git.md
  11. Увидеть разницу между текущим файлом и закоммиченным файлом --> git diff
  12. Сохраняем изменения и коммитим
  13. Переход от одного коммита к другому --> git checkout
  * ## __*Создаем паралельные ветки*__
    1. git branch inspector
    2. git branch creator
      * #### Сохраняем, коммитим и переходим на ветку creator
        1. git add instructions_Git.md
        2. git commit "Created two branches"
        3. git checkout creator
  * ## __*Изменим ветку*__ creator __*сохраним и создадим пару коммитов (фиксаций)*__
    1. git add instructions_Git.md
    2. git commit -m "Commit 1 branch creator"
    3. git commit -m "Commit 2 branch creator"