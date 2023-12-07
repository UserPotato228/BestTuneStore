# BestTuneStore
## Что это? 
Сайт для продажи автомобильного тюнинга. 
## На чем? 
Сайт будет создан на фреймворке ASP.NET, УВЫ

<img src="https://cs14.pikabu.ru/post_img/big/2023/07/06/5/1688624470117362562.jpg"/>

## Примерная модель БД
User
* ID PK AutoIncrement
* Login nvarchar(50) not null
* Password nvarchar(50) not null
* Fullname nvarchar(120) default "н\з"
* Phonenum nvarchar(15) default "н\з"
* Addres nvarchar(200) default "н\3"
* Flag int default 1

Product
* ID PK AutoIncrement
* Article nvarchar(20) not null
* Title nvarchar(150) not null
* Desc nvarchar(250) default "н\з"
* Cost int default 1
* Amount int default 1
* CategoryID int not null
* SubCategoryID int not null

Category
* ID PK AutoIncrement
* Name nvarchar(100) not null

SubCategory
* ID PK AutoIncrement
* CategoryID int not null
* Name nvarchar (100) not null
