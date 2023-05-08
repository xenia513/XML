# XML

## Homework to the first GIT lesson - XML part - Vadim Ksendzov's course

### 1. Создать внешний репозиторий c названием XML

    Repositories >> New >> XML >> Create repository 

### 2. Клонировать репозиторий XML на локальный компьютер

    XML >> Code >> Copy HTTPS

    $ git clone https://github.com/xenia513/XML.git

### 3. Внутри локального XML создать файл “new.xml”

    $ touch new.xml

### 4. Добавить файл под гит

    $ git add new.xml

### 5. Закоммитить файл

    $ git commit -m "created new.xml"

### 6. Отправить файл на внешний GitHub репозиторий

    $ git push

### 7. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML

    $ vim new.xml

Эта команда открывает встроенный редактор текста, для начала редактирования необходимо нажать `i` и ввести текст:
    
    <aboutMe>
	    <name>Kseniia_Kiseleva</name>
	    <age>30</age>
	    <petsCount>1</petsCount>
	    <salary>80000</salary>
    </aboutMe>

После завершения редактирования нажимаем `Esc` и `:wq` для сохранения внесенных изменений и выхода из режима редактора.

### 8. Отправить изменения на внешний репозиторий

    $ git commit -a -m "added text"

### 9. Создать файл preferences.xml

    $ cat > preferences.xml
    
После ввода этой команды открывается поле ввода текста для записи в файл, поэтому мы сразу же приступаем к выполнению следующего задания.

### 10. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, стрaна, которую хотели бы посетить) в формате XML

    <preferences>
      <favouriteMovie>Inception</favouriteMovie>
    	<favouriteSeries>YouAreTheWorst</favouriteSeries>
    	<favouriteFood>Curry</favouriteFood>
    	<favouriteSeason>Summer</favouriteSeason>
    </preferences>

Для завершения редактирования нажимаем `Enter` и `Ctrl+C`

### 11. Создать файл skills.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML

    $ cat > skills.xml

    <skills>
     <skills>bash</skills>
     <skills>postman</skills>
     <skills>GIT</skills>
     <skills>clientServerArchitecture</skills>
     <skills>devTools</skills>
     <skills>charlesProxy</skills>
     <skills>fiddler</skills>
     <skills>andriodStudio</skills>
    </skills>


### 12. Сделать коммит в одну строку

    $ git add . && git commit -m "added preferences.xml and skills.xml"

### 13. Отправить сразу 2 файла на внешний репозиторий

    $ git push

### 14. На веб-интерфейсе создать файл bugReport.xml

    XML >> Add file >> Create new file >> bugReport.xml

### 15. Сделать Commit changes (сохранить) изменения на веб-интерфейсе

    Commit new file 

### 16. На веб-интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML

    XML >> bugReport.xml >> Edit this file

Кнопка редактирования файла выглядит так:

![Edit this file button](https://docs.github.com/assets/cb-47677/mw-1440/images/help/repository/edit-file-edit-button.webp)

Вводим текст: 

    <bugReport>
     <ID>0001</ID>
     <Severity>Trivial</Severity>
      <Enviroment>Win 7 Chrome 109 IPhone 11 IOS 16.4.1 </Enviroment>
      <Title>The link [Share price] redirects to the english page from Trading Course 1, section 2 when AR, NL, VI, TH or ZN is chosen</Title>
      <Precondition></Precondition>
      <Steps>
         <Step1>Navigate to capital.com</Step1>
         <Step2>Hover over the [Education] menu section</Step2>
         <Step3>Click the [Trading сourses] menu item</Step3>
         <Step4>Click the [Who are the main market players?] row in the Introduction to Financial Markets box</Step4>
         <Step5>Select AR, NL, VI, TH or ZN language</Step5>
         <Step6>Scroll to the second to the last paragraph</Step6>
         <Step7>Click the link [Share price]</Step7>
      </Steps>
      <Postcondition></Postcondition>
      <ExpectedResult>The link [Share price] redirects to the page translated into chosen language</ExpectedResult>
      <ActualResult>The link [Share price] redirects to the english page</ActualResult>
      <Attachment>link</Attachment>
      <Author>@xenia513</Author>
    </bugReport>

### 17. Сделать Commit changes (сохранить) изменения на веб-интерфейсе

    Commit changes

### 18. Синхронизировать внешний и локальный репозиторий XML

    $ git pull
