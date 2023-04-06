# Git_Branch-HW2
1. На локальном репозитории сделать ветки для:
- git branch Postman
- git branch Jmeter
- git branch CheckLists
- git branch BagReports
- git branch SQL
- git branch Charles
- git branch MobileTesting

2. Запушить все ветки на внешний репозиторий - git push -u origin Postman SQL Jmeter CheckLists Charles MobileTesting BagReports

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта - git checkout BagReports
- touch bug_report.txt
- vim skills.txt /Нажать i
    ID: BR -01,
    Title: What? Where? When?,
    Severity: Minor,
    Priority: Medium,
    Precondition: Preparation steps,
    Environment: Devices,
    STR: Steps to restore,
    ER: Expected result,
    AR: Actual Result,
    Attachment: link

        /Нажать Esc :wq Enter
4. Запушить структуру багрепорта на внешний репозиторий - git add .
-git commit -m "bug report"
-git push

5. Вмержить ветку Bag Reports в Main - git checkout main
-git merge Bag_reports

6. Запушить main на внешний репозиторий - git add .
-git commit -m "merge branch Bag_reports in main"
-git push

7. В ветке CheckLists набросать структуру чек листа - git checkout CheckLists
-touch checkl.txt
-vim checkl.txt
        /Нажать i
Структура чек-листа:
    ID/Номер;
    Title/Заголовок. В одном пункте — одно требование, элемент или ОР;
    Pass/Fail/Статус; 
    Link/Ссылка на БР.

        /Нажать Esc :wq Enter

8. Запушить структуру на внешний репозиторий - git add .
-git commit -m "structure"
-git push

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main - После пуша check_list.txt на внешний репозиторий ветки CheckLists нажать на зеленую кнопку Compare&pull requset

10.  Синхронизировать Внешнюю и Локальную ветки Main 
-git fetch
-git pull
