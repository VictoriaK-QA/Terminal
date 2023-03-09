# Terminal
---
<details>

  <summary>TERMINAL LINUX HW#1</summary>

  
  
1. Посмотреть где я - <code> <b>pwd</b> </code>
2. Создать папку - <code> <b>mkdir folder_test</b> </code>
3. Зайти в папку - <code> <b>cd folder_test</b> </code>
4. Создать 3 папки - <code> <b>mkdir folder_test1 folder_test2 folder_test3</b> </code>
5. Зайти в любоую папку - <code> <b>cd folder_test3</b> </code>
6. Создать 5 файлов (3 txt, 2 json) - <code> <b>touch file_bug1.txt file_bug2.txt file_bug3.txt file_bug4.json file_bug5.json</b> </code>
7. Создать 3 папки - <code> <b>mkdir folder_chek1 folder_chek2 folder_chek3</b> </code>
8. Вывести список содержимого папки - <code> <b>ls -la</b> </code>
9. Открыть любой файл - <code> <b>vim file_bug5.json</b> </code>
10. Написать туда что-нибудь, любой текст - <code> <b>Нажать i</b> </code>
```json
{
        "order": {
                "id": 1,
                "firstName": "Константин",
                "lastName": "Иванов",
                "address": "Ленина, 12",
                "metroStation": 4,
                "phone": "+79996663300",
                "status":2

        }
}
```
11. Сохранить и выйти - <code> <b>Нажать Esc :wq Enter</b> </code>
12. Выйти из папки на уровень выше - <code> <b>cd ..</b> </code>
---
13. Переместить любые 2 файла, которые вы создали, в любую другую папку - 
<code> <b> mv file_bug4.json file_bug5.json ~/folder_test/folder_test2/</b> </code>
14. Cкопировать любые 2 файла, которые вы создали, в любую другую папку - 
<code> <b>cp file_bug1.txt file_bug2.txt ~/folder_test/folder_test2/</b> </code>
15. Найти файл по имени - <code> <b>find file_bug5.json</b> </code>
16. Просмотреть содержимое в реальном времени (команда grep) изучите как она работает - 
<code> <b>tail -F file_bug5.json</b> </code>  
Для выхода нажать <code> <b>ctrl+c</b> </code>
17. Вывести несколько первых строк из текстового файла - 
<code> <b>head -n2 file_bug5.json</b> </code>
18. Вывести несколько последних строк из текстового файла - 
<code> <b>tail -n2 file_bug5.json</b> </code>
19. Просмотреть содержимое длинного файла (команда less) изучите как она работает. - 
<code> <b>less long_file.json</b> </code> 
Для выхода нажать <code> <b>q</b> </code> 
20. Вывести дату и время - <code> <b>date</b> </code> или <code> <b>date +%c</b> </code>
---



:star2: Задание
1. Отправить http запрос на сервер.
http://162.55.220.72:5005/terminal-hw-request
<code> <b>curl 'http://162.55.220.72:5005/terminal-hw-request'</b> </code>
2. Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13
Файл <code> <b>file_script.sh</b> </code>
Команда <code> <b>./file_script.sh</b> </code>
```
#!/bin/bash 
cd Terminal_dz1
mkdir folder1 folder2 folder3
cd folder3
touch file1.txt file2.txt file3.txt file4.json file5.json
mkdir folder_dz1 folder_dz2 folder_dz3
ls -la 
mv file3.txt file4.json ~/folder_test/Terminal_dz1/folder1/
```

  

</details>