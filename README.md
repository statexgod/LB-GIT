# LB-GIT
1. ![Скріншот 1](1.png) - mkdir work для створення папки work, 
                cd work - перехід у неї, 
                touch hello.html - створення в ній файлу hello.html
2. ![Скріншот 2](2.png) - git init - створення Git-ропозиторію
3. ![Скріншот 3](3.png) - git add hello.html та git commit -m "Initial Commit" - Додавання в репозиторій сторінки hello.html
4. ![Скріншот 4](4.png) - git status - Перевірка стану репозиторію
5. ![Скріншот 5](5.png) - Перевірка стану директорії після внесення змін до файлу hello.html
6. ![Скріншот 6](6.png) - git add hello.html та git status - Індексація змін і перевірка стану
7. ![Скріншот 7](7.png) - git commit - Коміт усіх змін
8. ![Скріншот 8](8.png) - git add hello.html - Додавання змін до індексу Git
9. ![Скріншот 9](9.png) - git status - Перевірка статусу
10. ![Скріншот 10](10.png) - git commit -m "Added standard HTML page tags" - Комітет проіндексованих змін та git status - перевірка стану
11. ![Скріншот 11](11.png) - git add . - Додавання зміни в індекс і повторна перевірка статусу
12. ![Скріншот 12](12.png) - git commit -m "Added HTML header" - коміт другої зміни
13. ![Скріншот 13](13.png) - git log - Отримання списку зроблених змін
14. ![Скріншот 14](14.png) - git config --global format.pretty '%h %ad | %s%d [%an]', git config --global log.date short - налаштування формату виводу історії,
                  git log - Отримання історії
15. ![Скріншот 15](15.png) - git checkout <hash> - Подивитися історію змін за хешем,
                  cat hello.html - Подивитися вміст файлу hello.html
16. ![Скріншот 16](16.png) - git switch main - Повернення до останньої версії в гілці,
                  cat hello.html - Подивитися вміст файлу hello.html
17. ![Скріншот 17](17.png) - git tag v1 - Додавання тега v1 даної версії сторінки hello.html,
                  git log - Перегляд історії,
                  git checkout v1^ - Позначення попередньої версії,
                  cat hello.html - Подивитися вміст файлу hello.html
18. ![Скріншот 18](18.png) - git checkout v1, git checkout v1-beta - Перемикання між версіями
19. ![Скріншот 19](19.png) - git tag - Перегляд доступних тегів,
                  git log main --all - Перегляд тегів у логах
20. ![Скріншот 20](20.png) - git switch main - Перехід у гілку main,
                  git status - Перевірка статусу після внесення змін до файлу hello.html,
                  git checkout hello.html - перемикання в версію файлу hello.html у репозиторії,
                  git status - Перевірка статусу,
                  cat hello.html - Подивитися вміст файлу hello.html
21. ![Скріншот 21](21.png) - git add hello.html - Індексація змін після їх внесення до файлу hello.html,
                  git status - Перевірка стану,
                  git reset HEAD hello.html - Скасування індексації змін,
                  git checkout hello.html, git status - Перехід на версію коміта
22. ![Скріншот 22](22.png) - git add hello.html, git commit -m "Oops, we didn't want this commit" - Додавання файлу hello.html і небажаний коміт змін,
                  git revert HEAD - використання HEAD як посилання на коміт для скасування,
                  git log - Перевірка логів
23. ![Скріншот 23](23.png) - git log - Перевірка логів,
                  git tag oops - Позначення коміту тегом,
                  git reset --hard v1 - Відкат до коміту до помилкового,
                  git log - Перевірка логів,
                  git log --all - Перегляд усіх логів
24. ![Скріншот 24](24.png) - git tag -d oops - Видалення тегу oops,
                  git log --all - Перегляд усіх логів
25. ![Скріншот 25](25.png) - git add hello.html - Додавання hello.html після внесення змін,
                  git commit -m "Added copyright statement" - Коміт,
                  git log - Перевірка логів,
                  git add hello.html - Додавання hello.html після внесення змін,
                  git commit --amend -m "Added copyright statement with email" - Коміт,
                  git log - Перевірка логів
26. ![Скріншот 26](26.png) - git switch -c style - Створення нової гілки,
                  git status - Перевірка статусу,
                  touch style.css - Створення файлу style.css, 
                  git add style.css - Додавання style.css,
                  git commit -m "Added css stylesheet" - Коміт,
                  git add hello.html, git commit -m "Included stylesheet into hello.html" - Заміна та коміт файлу hello.html
27. ![Скріншот 27](27.png) - git log --all - Перегляд усіх логів,
                  git switch main - Перехід у гілку main,
                  cat hello.html - Перегляд файлу hello.html,
                  git switch style - Перехід у гілку style,
                  cat hello.html - Перегляд файлу hello.html
28. ![Скріншот 28](28.png)- git log hello.html - Історія змін hello.html,
                  git log style.css - Історія змін style.css,
                  git show v1 - Перегляд різниці між версіями,
                  mv hello.html index.html - Перейменування hello.html в index.html,
                  git status - Перевірка статусу,
                  git add ., git status - Додавання зміни в індекс і повторна перевірка статусу,
                  mkdir css - Створення директорії,
                  git mv style.css css/style.css - Переміщення style.css у директорію css,
                  git status - Перевірка статусу,
                  git commit -m "Renamed hello.html; moved style.css" - Коміт змін,
                  git log css/style.css - Перевірка історії змін у файлі css/styles.css,
                  git log --follow css/style.css - Перевірка історії до переміщення файлу
29. ![Скріншот 29](29.png) - touch README - Створення файлу README,
                  git add README - Додавання файлу,
                  git commit -m "Added README" - Коміт
30. ![Скріншот 30](30.png) - git log --all --graph - Перегляд розбіжностей гілок
31. ![Скріншот 31](31.png) - git switch style - Перемикання на гілку style,
                  git merge main - злиття main і style,
                  git log --all --graph - Перегляд гілок
32. ![Скріншот 32](32.png) - git switch main - Перемикання на гілку main,
                  git add hello.html, git commit -m "Added meta title" - Додавання та коміт hello.html після змін,
                  git log --all --graph - Перегляд гілок
33. ![Скріншот 33](33.png) - git switch main - Перемикання на гілку main,
                  git log --graph - Перегляд гілок,
                  git reset --hard HEAD~2 - Скидання гілки,
                  git log --graph - Перегляд гілок
34. ![Скріншот 34](34.png) - git switch style - Перемикання на гілку style,
                  git rebase main - Перенесення змін у гілку style,
                  git status - Перевірка статусу,
                  git add ., git rebase --continue - Додавання всіх змін і продовження перенесення,
                  git status, git log --all --graph - Перевірка статусу та логів
35. ![Скріншот 35](35.png) - git switch main - Перемикання на гілку main,
                  git merge style - Злиття style в гілку main,
                  git log --all --graph - Перевірка логів
36. ![Скріншот 36](36.png) - git clone work home - Створення клону репозиторію work
37. ![Скріншот 37](37.png) - cd home - Перехід у домашню директорію,
                  ls - Перегляд вмісту директорії,
                  git log --all - Перегляд історії репозиторіїв
38. ![Скріншот 38](38.png) - git remote - Дізнатися про імена віддалених репозиторіїв,
                  git remote show origin - більш детальна інформація про ім'я за замовчуванням
39. ![Скріншот 39](39.png) - git branch - Подивитися гілки клонованого репозиторію, 
                  git branch -a - Подивитися всі гілки клонованого репозиторію
40. ![Скріншот 40](40.png) - cd ../work - Перехід в оригінальний репозиторій work,
                  git add README, git commit -m "Changed README in original repo" - Додавання і коміт README після внесення змін,
                  git fetch - Підтягування нових комітів з віддаленого репозиторію,
                  git log --all - Перевірка логів,
                  git merge origin/main - Злиття підтягнутих змін у гілку main,
                  cat README - Перегляд README,
                  git pull - Підтягування нових комітів з віддаленого репозиторію (як і git fetch)
41. ![Скріншот 41](41.png) - git branch --track style origin/style - Додавання лоакльної гілки, яка відстежує віддалену,
                  git branch -a - Перегляд усіх гілок,
                  git log --max-count=2 - Перегляд останніх логів
42. ![Скріншот 42](42.png) - cd .. - перехід вище за дирректорією,
                  git clone --bare work work.git - Створення чистого клону,
                  ls work.git - Перегляд вмісту,
                  cd work - Перехід у work,
                  git remote add shared ../work.git - Додавання work.git в оригінальний репозиторій,
                  git switch main - Перемикання на гілку main,
                  git add README, git commit -m "Added shared comment to readme" - Додавання та коміт README,
                  git push shared main - Відправка змін                  
43. ![Скріншот 43](43.png) - cd ../home - Перехід у домашню директорію,
                  git remote add shared ../work.git - Додавання віддаленого репозиторію в локальний,
                  git branch --track shared main - Створення локальної гілки shared і відстеження main,
                  git pull shared main - отримання змін із гілки main,
                  cat README - Перегляд README
