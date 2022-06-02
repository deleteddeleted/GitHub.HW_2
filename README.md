# GitHub.HW_2
1. На локальном репозитории сделать ветки для:  
- Postman  
- Jmeter  
- CheckLists  
- Bag Reports  
- SQL  
- Charles  
- Mobile testing  

-на Githab создаем репозиторий, в котором будут ветки.  
New --> Repos Name:GitHub.-HW_2 --> Check "Add a README file" --> Press "Create repository"  

Клонировать репозиторий на локальный компьютер  
git clone https://github.com/deleteddeleted/HW_2.git  

Заходим в склонируемый репозиторий   
cd GitHub.HW_2  

Создаем ветки:  
git branch Postman  
git branch Jmeter  
git branch CheckLists  
git branch Bag_reports  
git branch SQL  
git branch Charles  
git branch Mobile_testing  

2. Запушить все ветки на внешний репозиторий  
git push origin --all  

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта  
git checkout Bag_reports  
cat > bag_reports.txt  

Краткое описание  
Проект  
Версия  
Серьезность бага  
Приоритет  
Статус  
Автор  
Исполнитель  
Шаги к воспроизведению  
Фактический результат  
Ожидаемый результат  
Дополнения  

ctrl+c  
4. Запушить структуру багрепорта на внешний репозиторий  
git add .  
git commit -m "bag_reports"  
git push -u origin Bag_reports  

5. Вмержить ветку Bag Reports в Main  
git checkout main
git merge Bag_reports  

6. Запушить main на внешний репозиторий
git add .  
git commit -m "merge branch Bag_reports in main"  
git push  

7. В ветке CheckLists набросать структуру чек листа.  
git checkout CheckLists  
cat > check_list.txt  

Чек лист интернет магазина:  

Наличие кнопок Купить, Заказать.  
Можно положить товар в корзину.  
После заказа приходит письмо на почту.  
Есть фильтры для поиска товаров.  
Есть форма обратной связи.  
Есть раздел с контактами.  
Есть ссылки на социальные сети.  
Строка поиска находится на видном месте.  
Присутствуют хлебные крошки.  
Отсутствуют опечатки.  
Проверка возможностей личного кабинета.  
Легко найти нужный товар.  
Нет дублирующихся товаров.  


8. Запушить структуру на внешний репозиторий 

git add .   
git commit -m "create check_list.txt"  
git push -u origin CheckLists  

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main  
Compare&pull requset   
create pull requset  
merge pull requset  
confirm merge  

10. Синхронизировать Внешнюю и Локальную ветки Main  
git checkout main  
git fetch  
git pull  
