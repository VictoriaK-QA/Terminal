# Terminal
---
<details>

  <summary>TERMINAL   LINUX   HW#1</summary>

  
  
1. Посмотреть где я - <code> <b>pwd</b> </code>
2. Создать папку - <code> <b>mkdir folder_test</b> </code>
3. Зайти в папку - <code> <b>cd folder_test</b> </code>
4. Создать 3 папки - <code> <b>mkdir folder_test1 folder_test2 folder_test3</b> </code>
5. Зайти в любоую папку - <code> <b>cd folder_test3</b> </code>
6. Создать 5 файлов (3 txt, 2 json) - <code> <b>touch file_bug1.txt file_bug2.txt file_bug3.txt file_bug4.json file_bug5.json</b> </code>
7. Создать 3 папки - <code> <b>mkdir folder_chek1 folder_chek2 folder_chek3</b> </code>
8. Вывести список содержимого папки - <code> <b>ls -la</b> </code>
9. Открыть любой файл - <code> <b>vim file_bug5.json</b> </code>
10. Написать туда что-нибудь, любой текст - Нажать <code> <b>i</b> </code>
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
11. Сохранить и выйти - Нажать <code> <b>Esc :wq Enter</b> </code>
12. Выйти из папки на уровень выше - <code> <b>cd ..</b> </code>
---
13. Переместить любые 2 файла, которые вы создали, в любую другую папку - <code> <b> mv file_bug4.json file_bug5.json ~/folder_test/folder_test2/</b> </code>
14. Cкопировать любые 2 файла, которые вы создали, в любую другую папку - <code> <b>cp file_bug1.txt file_bug2.txt ~/folder_test/folder_test2/</b> </code>
15. Найти файл по имени - <code> <b>find file_bug5.json</b> </code>
16. Просмотреть содержимое в реальном времени (команда grep) изучите как она работает - 
<code> <b>tail -F file_bug5.json</b> </code>  
Для выхода нажать <code> <b>ctrl+c</b> </code>

17. Вывести несколько первых строк из текстового файла - <code> <b>head -n2 file_bug5.json</b> </code>
18. Вывести несколько последних строк из текстового файла - <code> <b>tail -n2 file_bug5.json</b> </code>
19. Просмотреть содержимое длинного файла (команда less) изучите как она работает. - <code> <b>less long_file.json</b> </code>
Для выхода нажать <code> <b>q</b> </code> 
20. Вывести дату и время - <code> <b>date</b> </code> или <code> <b>date +%c</b> </code>
---



:star: Задание
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

---

<details>

  <summary>TERMINAL   LINUX   HW#2</summary>

  
  
1. 
2.
3.
  

</details>

---

<details>

  <summary>GIT   HW#1</summary>

  
  
  <code> <b></b> </code>

### JSON

 1. Создать внешний репозиторий c названием JSON - <b>GitHub</b> <code> <b>+ New repository</b> </code>
 - [X] Public
 - [X] Add a README file

 <code> <b>Create repository</b> </code>

 2. Клонировать репозиторий JSON на локальный компьютер - <code> <b>git clone git@github.com:VictoriaK-QA/JSON.git</b> </code>
 3. Внутри локального JSON создать файл “new.json” - <code> <b>cd JSON/</b> </code>  <code> <b>touch new.json</b> </code>
 4. Добавить файл под гит - <code> <b>git add .</b> </code>
 5. Закоммитить файл - <code> <b>git commit -m "new file"</b> </code>
 6. Отправить файл на внешний GitHub репозиторий - <code> <b>git push</b> </code>
 7. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON - <code> <b>vim new.json</b> </code>

 <b>Нажать</b> <code> <b>i</b> </code>
 ```json
 {
	"name": "Виктория",
	"age": 28,
	"pet": 1,
	"salary": 300
  }
 ```
 <b>Нажать</b> <code> <b>Esc :wq Enter</b> </code>

 8. Отправить изменения на внешний репозиторий - <code> <b>git commit -am "new file"</b> </code> <code> <b>git push</b> </code>
 9. Создать файл preferences.json - <code> <b>touch preferences.json</b> </code>
 10. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON - <code> <b>vim preferences.json</b> </code>

 <b>Нажать</b> <code> <b>i</b> </code>
 ```json
 {
	"favorite_movie": "The Godfather",
	"favorite_sitcom": "Friends",
	"favorite_food": "pasta",
	"favorite_season": "autumn",
	"country_to_travel": "Italy"
 }
  ```
 <b>Нажать</b> <code> <b>Esc :wq Enter</b> </code>
 
 11. Создать файл skills.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON - <code> <b>touch skills.json</b> </code>
 <code> <b>vim skills.json</b> </code>
 <b>Нажать</b> <code> <b>i</b> </code>
 ```json
 {
	"skills":["Testing Theory", "Client server", "SQL", "Postman", "Charles Fiddler Sniffing", "Web Services", "Git Linux Terminal", "DevTools", "Mobile Testing", "Web Testing", "Load testing"]
 }
 ```

 <b>Нажать</b> <code> <b>Esc :wq Enter</b> </code>
  
 12. Отправить сразу 2 файла на внешний репозиторий - <code> <b>git add .</b> </code>
 <code> <b>git commit -m "info about skills and preferences"</b> </code> <code> <b>git push</b> </code>

 13. На веб интерфейсе создать файл bug_report.json - <b>Нажать</b> <code> <b>Add file</b> </code> + <code> <b>Create new file</b> </code> 
 <b>Имя файла bug_report.json</b>
 14. Сделать Commit changes (сохранить) изменения на веб интерфейсе - <b>Нажать</b> <code> <b>Commit new file</b> </code>

 15. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON - <b>Нажать</b> <code> <b>Edit this file</b> </code>

 ```json
 {
  "ID": "BR-14",
  "Title": "What?Where?When?",
  "Severity": "Minor",
  "Priority": "Medium", 
  "Precondition": "Preparation steps",
  "Environment": "Devices",
  "STR": "Steps to restore",
  "ER": "Expected result",
  "AR": "Actual Result",
  "Attachment": "link"
 }
 ```
 16. Сделать Commit changes (сохранить) изменения на веб интерфейсе - <b>Нажать</b> <code> <b>Commit changes</b> </code>
 17. Синхронизировать внешний и локальный репозиторий JSON - <code> <b>git pull</b> </code>

---
### XML
 1. Создать внешний репозиторий c названием XML - <b>GitHub</b> <code> <b>+ New repository</b> </code>
 - [X] Public
 - [X] Add a README file

 <code> <b>Create repository</b> </code>

 2. Клонировать репозиторий XML на локальный компьютер - <code> <b>git clone git@github.com:VictoriaK-QA/XML.git</b> </code>
 3. Внутри локального XML создать файл “new.xml” - <code> <b>cd XML/</b> </code>  <code> <b>touch new.xml</b> </code>
 4. Добавить файл под гит - <code> <b>git add .</b> </code>
 5. Закоммитить файл - <code> <b>git commit -m "new file"</b> </code>
 6. Отправить файл на внешний GitHub репозиторий - <code> <b>git push</b> </code>
 7. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML - <code> <b>vim new.xml</b> </code>

 <b>Нажать</b> <code> <b>i</b> </code>
 ```xml
 <info>
  <name>Виктория</name>
  <age>28</age>
  <pet>1</pet>
  <salary>300</salary>
  </info>
 ```
 <b>Нажать</b> <code> <b>Esc :wq Enter</b> </code>

 8. Отправить изменения на внешний репозиторий - <code> <b>git commit -am "new file"</b> </code> <code> <b>git push</b> </code>
 9. Создать файл preferences.xml - <code> <b>touch preferences.xml</b> </code>
 10. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML - <code> <b>vim preferences.xml</b> </code>

 <b>Нажать</b> <code> <b>i</b> </code>
 ```xml
 <root>
  <favorite_movie>The Godfather</favorite_movie>
  <favorite_sitcom>Friends</favorite_sitcom>
  <favorite_food>pasta</favorite_food>
  <favorite_season>autumn</favorite_season>
  <country_to_travel>Italy</country_to_travel>
  </root>
  ```
 <b>Нажать</b> <code> <b>Esc :wq Enter</b> </code>
 
 11. Создать файл skills.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML - <code> <b>touch skills.xml</b> </code>
  <code> <b>vim skills.xml</b> </code>
 <b>Нажать</b> <code> <b>i</b> </code>
 ```xml
 <root>
  <skills>Testing Theory</skills>
  <skills>Client server</skills>
  <skills>SQL</skills>
  <skills>Postman</skills>
  <skills>Charles Fiddler Sniffing</skills>
  <skills>Web Services</skills>
  <skills>Git Linux Terminal</skills>
  <skills>DevTools</skills>
  <skills>Mobile Testing</skills>
  <skills>Web Testing</skills>
  <skills>Load testing</skills>
  </root> 
 ```

 <b>Нажать</b> <code> <b>Esc :wq Enter</b> </code>
 
 12. Сделать коммит в одну строку - <code> <b>git add .</b> </code>
 <code> <b>git commit -m "info about skills and preferences"</b> </code>
 
 13. Отправить сразу 2 файла на внешний репозиторий - <code> <b>git push</b> </code>
 14. На веб интерфейсе создать файл bug_report.xml - <b>Нажать</b> <code> <b>Add file</b> </code> + <code> <b>Create new file</b> </code> 
 <b>Имя файла bug_report.xml</b>

 15. Сделать Commit changes (сохранить) изменения на веб интерфейсе - <b>Нажать</b> <code> <b>Commit new file</b> </code> 
 
 16. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML - <b>Нажать</b> <code> <b>Edit this file</b> </code>

 ```xml
 <root>
  <ID>BR-14</ID>
  <Title>What?Where?When?</Title>
  <Severity>Minor</Severity>
  <Priority>Medium</Priority>
  <Precondition>Preparation steps</Precondition>
  <Environment>Devices</Environment>
  <STR>Steps to restore</STR>
  <ER>Expected result</ER>
  <AR>Actual Result</AR>
  <Attachment>link</Attachment>
  </root>
 ```

 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе - <b>Нажать</b> <code> <b>Commit changes</b> </code>
 18. Синхронизировать внешний и локальный репозиторий XML - <code> <b>git pull</b> </code>

---
### TXT
 1. Создать внешний репозиторий c названием TXT - <b>GitHub</b> <code> <b>+ New repository</b> </code>
 - [X] Public
 - [X] Add a README file
 <code> <b>Create repository</b> </code>
 2. Клонировать репозиторий TXT на локальный компьютер -
 <code> <b>git clone git@github.com:VictoriaK-QA/TXT.git</b> </code>
 3. Внутри локального TXT создать файл “new.txt” - <code> <b>cd TXT/</b> </code>  <code> <b>touch new.txt</b> </code>
 4. Добавить файл под гит - <code> <b>git add .</b> </code>
 5. Закоммитить файл - <code> <b>git commit -m "new file"</b> </code>
 6. Отправить файл на внешний GitHub репозиторий - <code> <b>git push</b> </code>
 7. Отредактировать содержание файла “new.txt” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате TXT
  <code> <b>vim new.txt</b> </code>

 <b>Нажать</b> <code> <b>i</b> </code>
 ```
 name - Victoria
 age - 28
 pet - 1 
 salary - 300000
 ```
 <b>Нажать</b> <code> <b>Esc :wq Enter</b> </code>

 8. Отправить изменения на внешний репозиторий - <code> <b>git commit -am "info about me"</b> </code> <code> <b>git push</b> </code>
 9. Создать файл preferences.txt - <code> <b>touch preferences.txt</b> </code>
 10. В файл preferences.txt” добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате TXT

 <code> <b>vim preferences.txt</b> </code>

 <b>Нажать</b> <code> <b>i</b> </code>
 ```
 favorite movie: The Godfather,
 favorite sitcom: Friends,
 favorite food: pasta,
 favorite season: autumn,
 country to travel: Italy	
  ```
 <b>Нажать</b> <code> <b>Esc :wq Enter</b> </code>
 
 11. Создать файл skills.txt добавить информацию о скиллах которые будут изучены на курсе в формате TXT - <code> <b>touch skills.txt</b> </code>
  <code> <b>vim skills.txt</b> </code>
 <b>Нажать</b> <code> <b>i</b> </code>
 ```
 SKILLS: 
 Testing Theory, 
 Client server, 
 SQL, 
 Postman, 
 Charles Fiddler Sniffing, 
 Web Services, 
 Git Linux Terminal, 
 DevTools, 
 Mobile Testing, 
 Web Testing, 
 Load testing 
 ```

 <b>Нажать</b> <code> <b>Esc :wq Enter</b> </code>
 
 12. Сделать коммит в одну строку - <code> <b>git add .</b> </code>
 <code> <b>git commit -m "info about skills and preferences"</b> </code>

 13. Отправить сразу 2 файла на внешний репозиторий - <code> <b>git push</b> </code>
 14. На веб интерфейсе создать файл bug_report.txt - <b>Нажать</b> <code> <b>Add file</b> </code> + <code> <b>Create new file</b> </code> 
 <b>Имя файла bug_report.txt</b>
  15. Сделать Commit changes (сохранить) изменения на веб интерфейсе - <b>Нажать</b> <code> <b>Commit new file</b> </code> 

 16. На веб интерфейсе модифицировать файл bug_report.txt, добавить баг репорт в формате TXT - <b>Нажать</b> <code> <b>Edit this file</b> </code>
 
```
ID: BR-14,
Title: What? Where? When?,
Severity: Minor,
Priority: Medium,
Precondition: Preparation steps,
Environment: Devices,
STR: Steps to restore,
ER: Expected result,
AR: Actual Result,
Attachment: link
```
 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе - <b>Нажать</b> <code> <b>Commit changes</b> </code>
 18. Синхронизировать внешний и локальный репозиторий TXT - <code> <b>git pull</b> </code>
  

</details>

---


<details>

  <summary>GIT   HW#2</summary>

  
  
1. На локальном репозитории сделать ветки для:
- Postman - <code> <b>git branch Postman</b> </code>
- Jmeter - <code> <b>git branch Jmeter</b> </code>
- CheckLists - <code> <b>git branch CheckLists</b> </code>
- Bag Reports - <code> <b>git branch BagReports</b> </code>
- SQL - <code> <b>git branch SQL</b> </code>
- Charles - <code> <b>git branch Charles</b> </code>
- Mobile testing - <code> <b>git branch MobileTesting</b> </code>

2. Запушить все ветки на внешний репозиторий - <code> <b>git add .</b> </code>  
<code> <b>git commit -m "new seven branch"</b> </code> 
<code> <b>git checkout main</b> </code>
<code> <b>git push -u origin Postman SQL Jmeter CheckLists Charles MobileTesting BagReports</b> </code>

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта - <code> <b>git checkout BagReports</b> </code>
<code> <b>touch bug_report.txt</b> </code>
<code> <b>vim skills.txt</b> </code>
 <b>Нажать</b> <code> <b>i</b> </code>
 ```
ID: BR-14,
Title: What? Where? When?,
Severity: Minor,
Priority: Medium,
Precondition: Preparation steps,
Environment: Devices,
STR: Steps to restore,
ER: Expected result,
AR: Actual Result,
Attachment: link
 ```
<b>Нажать</b> <code> <b>Esc :wq Enter</b> </code>

4. Запушить структуру багрепорта на внешний репозиторий - <code> <b>git add .</b> </code>
<code> <b>git commit -m "bug report"</b> </code>
<code> <b>git push</b> </code>

5. Вмержить ветку Bag Reports в Main - <code> <b>git checkout main</b> </code>
<code> <b>git merge Bag_reports</b> </code>

6. Запушить main на внешний репозиторий - <code> <b>git add .</b> </code>
<code> <b>git commit -m "merge branch Bag_reports in main"</b> </code>
<code> <b>git push</b> </code>

7. В ветке CheckLists набросать структуру чек листа - <code> <b>git checkout CheckLists</b> </code>
<code> <b>touch checkl.txt</b> </code>

<code> <b>vim checkl.txt</b> </code>

<b>Нажать</b> <code> <b>i</b> </code>

 ```
Структура чек-листа:
1 - ID/Номер;
2 - Title/Заголовок. В одном пункте — одно требование, элемент или ОР;
3 - Pass/Fail/Статус; 
4 - Link/Ссылка на БР.
 ```
<b>Нажать</b> <code> <b>Esc :wq Enter</b> </code>

8. Запушить структуру на внешний репозиторий - <code> <b>git add .</b> </code>
<code> <b>git commit -m "structure"</b> </code>
<code> <b>git push</b> </code>

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main - <b>После пуша check_list.txt на внешний репозиторий ветки CheckLists нажать на зеленую кнопку</b> <code> <b>Compare&pull requset</b> </code>
10. Синхронизировать Внешнюю и Локальную ветки Main - <code> <b>git checkout main</b> </code> <code> <b>git fetch</b> </code>
<code> <b>git pull</b> </code>

  

</details>

---