
# JSON  

1. Создать внешний репозиторий c названием JSON.

    Зайти на сайт [github](https://github.com/)  
    Нажать на кнопку   
    ![New](https://github.com/bryack/JSON/blob/4f209e68a42dea209f36e4192ad5ddb277189202/new_rep.png?raw=true)  
    В поле "Repository name" написать `JSON`  
    Нажать на кнопку  
    ![Create repository](https://github.com/bryack/JSON/blob/main/cr_rep.png?raw=true)

2. Клонировать репозиторий JSON на локальный компьютер.

    Открыть папку D:\YandexDisk\QA\Git  
    Кликнуть правой кнопкой мыши в окне папки  
    В меню выбрать `Git Bash Here`    

    ![Git Bash Here](https://github.com/bryack/JSON/blob/main/git_bash_here.png?raw=true)

    В терминале прописать команду для клонирования репозитория и ссылку HTTPS   
    `git clone https://github.com/bryack/JSON.git`

3. Внутри локального JSON создать файл “new.json”.
    ``` bash
    cd JSON
    touch new.json
    ```

4. Добавить файл под гит.  
`git add new.json`

5. Закоммитить файл.  
`git commit -m "Add file new.json"`

6. Отправить файл на внешний GitHub репозиторий.  
`git push`

7. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.  
    `vim new.json` `i`
    ``` json
    { 
	    "name": "Anna",
	    "age": 32,
	    "number_of_pets": 1,
        "expected_salary": "1000$",
    }
    ```
    Esc `:wq` Enter


8. Отправить изменения на внешний репозиторий.  
    `git commit -am "Edit file new.json"`  
    `git push`

9. Создать файл preferences.json  
`touch preferences.json`

10. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON.  
    `vim preferences.json` `i`  
    ``` json
    { 
	    "favorite_movie": "Scream",
	    "favorite_show": "True Detective",
	    "favotite_food": "Potato",
        "favorite_season": "Summer",
        "country_to_visit": "USA",
    }
    ```
    Esc `:wq` Enter

11. Создать файл skills.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON  
    `vim skills.json` `i`  
    ``` json
    {
    "skills": {
        "1.": "Базовая теория (Что такое тестирование, багрепорты, документация, виды, методы, направления тестирования и т.п.) SDLC, STLC",
        "2.": "Что такое клиент-серверная архитектура",
        "3.": "HTTP Методы запросов на сервер",
        "4.": "Коды ответов HTTP сервера",
        "5.": "Структуры HTTP запросов и ответов",
        "6.": "Что такое JSON, XML. Их структура",
        "7.": "Тестирование API через Postman (JS, автотесты API)",
        "8.": "Снятие и чтение логов c внешнего сервера",
        "9.": "Снифинг http web трафика через Charles и Fiddler",
        "10.": "Dev Tools веб браузеров (Google Chrome, FireFox)",
        "11.": "VPN. (Как работает, зачем нужен, как использовать, варианты инструментов)",
        "12.": "Мобильное тестирование",
        "13.": "Особенность iOS, Android, гайдлайны",
        "14.": "Сборка iOS приложений на XCode. (У кого нет Mac компьютера, просто посмотрят)",
        "15.": "Сборка Android приложений на Android Studio",
        "16.": "ADB (управление андройд девайсами)",
        "17.": "Настройка прокси и vpn на iOS и Android",
        "18.": "Перехват (сниффинг) мобильного трафика через Charles и Fiddler на iOS и Android",
        "19.": "Командная строка (terminal) Linux (копирование, создание, просмотр, перемещение файлов на серверах без графического интерфейса)",
        "20.": "Основы bash скриптинг, автоматизация рутинных задач на сервере",
        "21.": "Доступ к удалённым серверам",
        "22.": "Основы SQL (Create, Delete, Drop, Insert Into, Select, From, Where, Join)",
        "23.": "База данных Postgres (установка, настройка и использование)",
        "24.": "Нереляционная база данных Redis (установка, настройка и использование)",
        "25.": "агрузочное тестирование в Jmeter",
        "26.": "Методология разработки Scrum",
        "27.": "Python. (Изучение основ. Создание клиент серверного приложения)",
        }
    } 
    ```
    Esc `:wq` Enter  


12. Отправить сразу 2 файла на внешний репозиторий.  
    `git add preferences.json skills.json`  
    ` git commit -m "Add new files preferences.json skills.json"`  
    `git push`  

13. На веб интерфейсе создать файл bug_report.json.
14. Сделать Commit changes (сохранить) изменения на веб интерфейсе.  
    Зайти на сайт [github](https://github.com/)  
    Открыть репозиторий `JSON`  
    Нажать на кнопку `Add file`  
    ![Add file](https://github.com/bryack/JSON/blob/main/add_file.png?raw=true)  
    Выбрать в меню `Create new file`  
    В поле `name` написать bug_report.json  
    В поле `Commit new file` написать Create bug_report.json    
    Нажать на кнопку `Commit new file`  
    ![Commit new file](https://github.com/bryack/JSON/blob/main/commit_new_file.png?raw=true)  

15. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
Нажать редактировать файл
``` json
{
    "Summary": "Main page: Button 'Login' doesn't click",
    "Description": {
        "STR": {
                "1.": "Open the Main page",
                "2.": "Click the 'Login' button"
                },
        "Result": "Button 'Login' doesn't click",
        "Expected result": "Button 'Login' is clicked according to requirement №1",
                    },
    "Project": "My Site",
    "Component": "Login",
    "Build": "1.0",
    "Severity": "Blocker",
    "Priority": "High",
    "Author": "Anna Nurgaleeva",
    "Sign to": "Developer",
    "Environment": "Windows 8.1 x64",
}
```  
16. Сделать Commit changes (сохранить) изменения на веб интерфейсе.  
    В поле `Commit changes` написать Update bug_report.json  
    Нажать на кнопку `Commit changes`  
    ![Commit changes](https://github.com/bryack/JSON/blob/main/commit_changes.png?raw=true)  

17. Синхронизировать внешний и локальный репозиторий JSON  
    `git pull`  

# XML  

1. Создать внешний репозиторий c названием XML.  
    Зайти на сайт [github](https://github.com/)  
    Нажать на кнопку   
    ![New](https://github.com/bryack/JSON/blob/4f209e68a42dea209f36e4192ad5ddb277189202/new_rep.png?raw=true)  
    В поле "Repository name" написать `XML`  
    Нажать на кнопку  
    ![Create repository](https://github.com/bryack/JSON/blob/main/cr_rep.png?raw=true)  

2. Клонировать репозиторий XML на локальный компьютер.  

    Открыть папку D:\YandexDisk\QA\Git  
    Кликнуть правой кнопкой мыши в окне папки   
    В меню выбрать `Git Bash Here`    

    ![Git Bash Here](https://github.com/bryack/JSON/blob/main/git_bash_here.png?raw=true)

    В терминале прописать команду для клонирования репозитория и ссылку HTTPS   
    `git clone https://github.com/bryack/XML.git`  

20. Внутри локального XML создать файл “new.xml”.  
     ``` bash
    cd XML
    touch new.xml
    ```  

21. Добавить файл под гит.  
    `git add new.xml`  

22. Закоммитить файл.  
    `git commit -m "Add file new.xml"`  

23. Отправить файл на внешний GitHub репозиторий.  
    `git push`  

24. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.  
`vim new.xml` `i`
    ``` xml
    <?xml version="1.0" encoding="UTF-8"?>
    <about> 
	    <name>Anna</name>
	    <age>32</age>
	    <number_of_pets>1</number_of_pets>
        <expected_salary currency="US dollar">1000</expected_salary>
    </about>
    ```
    Esc `:wq` Enter  

25. Отправить изменения на внешний репозиторий.  
    `git commit -am "Edit file new.xml"`  
    `git push`  

26. Создать файл preferences.xml  
    `touch preferences.xml`  

27. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML.  
     `vim preferences.xml` `i`  
    ``` xml
    <?xml version="1.0" encoding="UTF-8"?>
    <preferences> 
	    <favorite_movie>
            <question>Your favorite movie?</question>
            <answer>Scream</answer>
        </favorite_movie>
	    <favorite_show>
            <question>Your favorite TV show?</question>
            <answer>True Detective</answer>
        </favorite_show>
	    <favotite_food>
            <question>Your favorite food?</question>
            <answer>Potato</answer>
        </favotite_food>
        <favorite_season>
            <question>Your favorite season?</question>
            <answer>Summer</answer>
        </favorite_season>
        <country_to_visit>
            <question>What country would you like to visit?</question>
            <answer>USA</answer>
        </country_to_visit>
    </preferences>
    ```
    Esc `:wq` Enter  

28. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML  
     `vim skills.xml` `i`  
    ``` xml
    <?xml version="1.0" encoding="UTF-8"?>
    <skills_list>
        <skill>
            <number>1.</number>  
            <description>Базовая теория (Что такое тестирование, багрепорты, документация, виды, методы, направления тестирования и т.п.) SDLC, STLC</description>  
        </skill>
        <skill>
            <number>2.</number>  
            <description>Что такое клиент-серверная архитектура</description>  
        </skill>
        <skill>
            <number>3.</number>  
            <description>HTTP Методы запросов на сервер</description>  
        </skill>
        <skill>
            <number>4.</number>  
            <description>Коды ответов HTTP сервера</description>  
        </skill>
        <skill>
            <number>5.</number>  
            <description>Структуры HTTP запросов и ответов</description>  
        </skill>
        <skill>
            <number>6.</number>  
            <description>Что такое JSON, XML. Их структура</description>  
        </skill>
        <skill>
            <number>7.</number>  
            <description>Тестирование API через Postman (JS, автотесты API)</description>  
        </skill>
        <skill>
            <number>8.</number>  
            <description>Снятие и чтение логов c внешнего сервера</description>  
        </skill>
        <skill>
            <number>9.</number>  
            <description>Снифинг http web трафика через Charles и Fiddler</description>  
        </skill>
        <skill>
            <number>10.</number>  
            <description>Dev Tools веб браузеров (Google Chrome, FireFox)</description>  
        </skill>
        <skill>
            <number>11.</number>  
            <description>VPN. (Как работает, зачем нужен, как использовать, варианты инструментов)</description>  
        </skill>
        <skill>
            <number>12.</number>  
            <description>Мобильное тестирование</description>  
        </skill>
        <skill>    
            <number>13.</number>  
            <description>Особенность iOS, Android, гайдлайны</description>  
        </skill>
        <skill>    
            <number>14.</number>  
            <description>Сборка iOS приложений на XCode. (У кого нет Mac компьютера, просто посмотрят)</description>  
        </skill>
        <skill>    
            <number>15.</number>  
            <description>Сборка Android приложений на Android Studio</description>  
        </skill>
        <skill>    
            <number>16.</number>  
            <description>ADB (управление андройд девайсами)</description>  
        </skill>
        <skill>    
            <number>17.</number>  
            <description>Настройка прокси и vpn на iOS и Android</description>  
        </skill>
        <skill>    
            <number>18.</number>  
            <description>Перехват (сниффинг) мобильного трафика через Charles и Fiddler на iOS и Android</description>  
        </skill>
        <skill>    
            <number>19.</number>  
            <description>Командная строка (terminal) Linux (копирование, создание, просмотр, перемещение файлов на серверах без графического интерфейса)</description>  
        </skill>
        <skill>    
            <number>20.</number>  
            <description>Основы bash скриптинг, автоматизация рутинных задач на сервере</description>  
        </skill>
        <skill>    
            <number>21.</number>  
            <description>Доступ к удалённым серверам</description>  
        </skill>
        <skill>    
            <number>22.</number>  
            <description>Основы SQL (Create, Delete, Drop, Insert Into, Select, From, Where, Join)</description>  
        </skill>
        <skill>    
            <number>23.</number>  
            <description>База данных Postgres (установка, настройка и использование)</description>  
        </skill>
        <skill>    
            <number>24.</number>  
            <description>Нереляционная база данных Redis (установка, настройка и использование)</description>  
        </skill>
        <skill>    
            <number>25.</number>  
            <description>агрузочное тестирование в Jmeter</description>  
        </skill>
        <skill>    
            <number>26.</number>  
            <description>Методология разработки Scrum</description>  
        </skill>
        <skill>    
            <number>27.</number>  
            <description>Python. (Изучение основ. Создание клиент серверного приложения)</description>
        </skill>
    </skills_list>
    ```
    Esc `:wq` Enter  

29. Сделать коммит в одну строку.  
    `git add . | git commit -m "Add two new files preferences.xml and skills.xml"`

30. Отправить сразу 2 файла на внешний репозиторий.  
    `git push`  

31. На веб интерфейсе создать файл bug_report.xml.  
32. Сделать Commit changes (сохранить) изменения на веб интерфейсе.  
    Зайти на сайт [github](https://github.com/)  
    Открыть репозиторий `XML`  
    Нажать на кнопку `Add file`  
    ![Add file](https://github.com/bryack/JSON/blob/main/add_file.png?raw=true)  
    Выбрать в меню `Create new file`  
    В поле `name` написать *bug_report.xml*  
    В поле `Commit new file` написать *Create bug_report.xml*  
    Нажать на кнопку `Commit new file`  
    ![Commit new file](https://github.com/bryack/JSON/blob/main/commit_new_file.png?raw=true)  

33. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.  
    Открыть файл *bug_report.xml*  
    Нажать на кнопку *редактировать файл*
``` xml
<?xml version="1.0" encoding="UTF-8"?>
<bug_report>
    <summary>
        <title_first_lvl>Summary</title_first_lvl>
        <text>Main page: Button 'Login' doesn't click</text>
    </summary>
    <description>
        <title_first_lvl>Description</title_first_lvl>
        <str>
            <title_second_lvl>STR</title_second_lvl>
            <text>
                1. Open the Main page
                2. Click the 'Login' button
            </text>
        </str>    
        <result>
            <title_second_lvl>Result</title_second_lvl>
            <text>Button 'Login' doesn't click</text>
        </result>
        <expected_result>
            <title_second_lvl>Expected result</title_second_lvl>
            <text>Button 'Login' is clicked according to requirement №1</text>
        </expected_result>
    </description>
    <project>
        <title_first_lvl>Project</title_first_lvl>
        <text>My Site</text>
    </project>
    <component>
        <title_first_lvl>Component</title_first_lvl>
        <text>Login</text>
    </component>
    <build>
        <title_first_lvl>Build</title_first_lvl>
        <text>1.0</text>
    </build>
    <severity>
        <title_first_lvl>Severity</title_first_lvl>
        <text>Blocker</text>
    </severity>
    <priority>
        <title_first_lvl>Priority</title_first_lvl>
        <text>High</text>
    </priority>
    <author>
        <title_first_lvl>Author</title_first_lvl>
        <text>Anna Nurgaleeva</text>
    </author>
    <sigh_to>
        <title_first_lvl>Sigh to</title_first_lvl>
        <text>Developer</text>
    </sigh_to>
    <environment>
        <title_first_lvl>Environment</title_first_lvl>
        <text>Windows 8.1 x64</text>
    </environment>
</bug_report>
```  

34. Сделать Commit changes (сохранить) изменения на веб интерфейсе.  
    В поле `Commit changes` написать Update bug_report.xml  
    Нажать на кнопку `Commit changes`  
    ![Commit changes](https://github.com/bryack/JSON/blob/main/commit_changes.png?raw=true)  

35. Синхронизировать внешний и локальный репозиторий XML  
    `git pull`  

# TXT  

1. Создать внешний репозиторий c названием TXT.  
    Зайти на сайт [github](https://github.com/)  
    Нажать на кнопку   
    ![New](https://github.com/bryack/JSON/blob/4f209e68a42dea209f36e4192ad5ddb277189202/new_rep.png?raw=true)  
    В поле "Repository name" написать `TXT`  
    Нажать на кнопку  
    ![Create repository](https://github.com/bryack/JSON/blob/main/cr_rep.png?raw=true)  

37. Клонировать репозиторий TXT на локальный компьютер.    
    Открыть папку D:\YandexDisk\QA\Git  
    Кликнуть правой кнопкой мыши в окне папки  
    В меню выбрать `Git Bash Here`    

    ![Git Bash Here](https://github.com/bryack/JSON/blob/main/git_bash_here.png?raw=true)

    В терминале прописать команду для клонирования репозитория и ссылку HTTPS   
    `git clone https://github.com/bryack/TXT.git`  

38. Внутри локального TXT создать файл “new.txt”.  
    ``` bash
    cd TXT
    touch new.txt
    ```  

39. Добавить файл под гит.  
    `git add new.txt`

40. Закоммитить файл.  
    `git commit -m "Add file new.txt"`

41. Отправить файл на внешний GitHub репозиторий.  
    `git push`  

42. Отредактировать содержание файла “new.txt” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате TXT.  
`vim new.txt` `i`
    ``` 
	    name: Anna
	    age: 32
	    number of pets: 1
        expected salary: 1000$
    ```
    Esc `:wq` Enter  

43. Отправить изменения на внешний репозиторий.  
    `git commit -am "Edit file new.txt"`  
    `git push`  

44. Создать файл preferences.txt  
    `touch preferences.txt`  

45. В файл preferences.txt” добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате TXT.  
     `vim preferences.txt` `i`  
    ```
        Your favorite movie? Scream  
        Your favorite TV show? True Detective  
        Your favorite food? Potato   
        Your favorite season? Summer   
        What country would you like to visit? USA   
    ```  
    Esc `:wq` Enter  

46. Создать файл sklls.txt добавить информацию о скиллах которые будут изучены на курсе в формате TXT  
    `vim skills.txt` `i`
     ```
     1. Базовая теория (Что такое тестирование, багрепорты, документация, виды, методы, направления тестирования и т.п.) SDLC, STLC  
     2. Что такое клиент-серверная архитектура   
     3. HTTP Методы запросов на сервер   
     4. Коды ответов HTTP сервера   
     5. Структуры HTTP запросов и ответов   
     6. Что такое JSON, XML. Их структура   
     7. Тестирование API через Postman (JS, автотесты API)   
     8. Снятие и чтение логов c внешнего сервера  
     9. Снифинг http web трафика через Charles и Fiddler 
     10. Dev Tools веб браузеров (Google Chrome, FireFox) 
     11. VPN. (Как работает, зачем нужен, как использовать, варианты инструментов) 
     12. Мобильное тестирование 
     13. Особенность iOS, Android, гайдлайны 
     14. Сборка iOS приложений на XCode. (У кого нет Mac компьютера, просто посмотрят) 15. Сборка Android приложений на Android Studio 
     16. ADB (управление андройд девайсами) 
     17. Настройка прокси и vpn на iOS и Android 
     18. Перехват (сниффинг) мобильного трафика через Charles и Fiddler на iOS и Android 
     19. Командная строка (terminal) Linux (копирование, создание, просмотр, перемещение файлов на серверах без графического интерфейса) 
     20. Основы bash скриптинг, автоматизация рутинных задач на сервере 
     21. Доступ к удалённым серверам 
     22. Основы SQL (Create, Delete, Drop, Insert Into, Select, From, Where, Join) 
     23. База данных Postgres (установка, настройка и использование) 
     24. Нереляционная база данных Redis (установка, настройка и использование) 
     25. агрузочное тестирование в Jmeter 
     26. Методология разработки Scrum 
     27. Python. (Изучение основ. Создание клиент серверного приложения)  
     ```  
     Esc `:wq` Enter  

47. Сделать коммит в одну строку.  
    `git add . | git commit -m "Add two new files preferences.txt and skills.txt"`  

48. Отправить сразу 2 файла на внешний репозиторий.  
    `git push`  

49. На веб интерфейсе создать файл bug_report.txt.  
50. Сделать Commit changes (сохранить) изменения на веб интерфейсе.  
    Зайти на сайт [github](https://github.com/)  
    Открыть репозиторий `TXT`  
    Нажать на кнопку `Add file`  
    ![Add file](https://github.com/bryack/JSON/blob/main/add_file.png?raw=true)  
    Выбрать в меню `Create new file`  
    В поле `name` написать *bug_report.txt*  
    В поле `Commit new file` написать *Create bug_report.txt*  
    Нажать на кнопку `Commit new file`  
    ![Commit new file](https://github.com/bryack/JSON/blob/main/commit_new_file.png?raw=true)  

51. На веб интерфейсе модифицировать файл bug_report.txt, добавить баг репорт в формате TXT.  
    ```
    Summary: Main page: Button 'Login' doesn't click
    Description 
        STR: 
            1. Open the Main page 
            2. Click the 'Login' button 
        Result: Button 'Login' doesn't click 
        Expected result: Button 'Login' is clicked according to requirement №1 
    Project: My Site 
    Component: Login 
    Build: 1.0 
    Severity: Blocker 
    Priority: High 
    Author: Anna Nurgaleeva 
    Sigh to: Developer 
    Environment: Windows 8.1 x64  
    ```  

52. Сделать Commit changes (сохранить) изменения на веб интерфейсе.  
    В поле `Commit changes` написать Update bug_report.txt  
    Нажать на кнопку `Commit changes`  
    ![Commit changes](https://github.com/bryack/JSON/blob/main/commit_changes.png?raw=true)  

53. Синхронизировать внешний и локальный репозиторий TXT  
    `git pull`