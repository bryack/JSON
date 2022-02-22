1. Создать внешний репозиторий c названием JSON.

    Заходим на сайт [github](https://github.com/)  
    Нажимаем на кнопку   
    ![New](https://github.com/bryack/JSON/blob/4f209e68a42dea209f36e4192ad5ddb277189202/new_rep.png?raw=true)  
    В поле "Repository name" пишем `JSON`  
    Нажимаем на кнопку  
    ![Create repository](https://github.com/bryack/JSON/blob/main/cr_rep.png?raw=true)

2. Клонировать репозиторий JSON на локальный компьютер.

    Открываю папку D:\YandexDisk\QA\Git
    Кликаю правой кнопкой мыши в окне папки
    Во меню выбираю `Git Bash Here`  

    ![Git Bash Here](https://github.com/bryack/JSON/blob/main/git_bash_here.png?raw=true)

    В терминале прописываю команду для клонирования репозитория и ссылку HTTPS   
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
git commit -am "Edit file new.json"
