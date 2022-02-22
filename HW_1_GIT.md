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
    Во меню выбрать `Git Bash Here`  

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
        "expected_salary": "1000$"
    }
    ```
    `:wq` `Enter`


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
        "country_to_visit": "USA"
    }
    ```
    `:wq` `Enter`

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
        "27.": "Python. (Изучение основ. Создание клиент серверного приложения)"
        }
    } 
    ```
    `:wq` `Enter`  


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
    ![Commit new file]()
