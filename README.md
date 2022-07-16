# yamdb_final
## <h1 align="center"> Проект YaMDb </h1>
>"Review and comment your favourites" 

![Django-app workflow](https://github.com/SpaceJesusJPG/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)

## Описание
Проект YaMDb собирает отзывы пользователей на произведения. Произведения делятся на категории: «Книги», «Фильмы», «Музыка». Список категорий может быть расширен администратором (например, можно добавить категорию «Изобразительное искусство» или «Ювелирка»).
Сами произведения в YaMDb не хранятся, здесь нельзя посмотреть фильм или послушать музыку.
В каждой категории есть произведения: книги, фильмы или музыка. Например, в категории «Книги» могут быть произведения «Винни-Пух и все-все-все» и «Марсианские хроники», а в категории «Музыка» — песня «Давеча» группы «Насекомые» и вторая сюита Баха.
Произведению может быть присвоен жанр из списка предустановленных (например, «Сказка», «Рок» или «Артхаус»). Новые жанры может создавать только администратор.
Благодарные или возмущённые пользователи оставляют к произведениям текстовые отзывы и ставят произведению оценку в диапазоне от одного до десяти; из пользовательских оценок формируется усреднённая оценка произведения — рейтинг. На одно произведение пользователь может оставить только один отзыв.


### Используемые технологии:

* Python 3.8
* Django 2.2
* Django Rest Framework 3.12
* Simple JWT
* nginx
* Docker
* Docker-Compose

### Посмотреть уже развернутый проект:

[API YaMDb](http://51.250.18.216/api/v1/)

Примеры запросов к API и документацию можно посмотреть [тут](http://51.250.18.216/redoc/)


### Как развернуть проект локально:

Клонировать репозиторий и перейти в папку с инструкциями в командной строке: 

 

``` 

git clone git@github.com:SpaceJesusJPG/yamdb_final.git 

``` 

 

``` 

cd infra_sp2/infra 

``` 

 

Собрать контейнер, выполнить миграции и собрать статику: 

 

``` 

docker-compose up 

``` 

 

``` 

docker-compose exec web python manage.py migrate 

``` 

 

``` 

docker-compose exec web python manage.py collectstatic --no-input 

``` 

 

### Автор: 

* [Никита Гладышев](https://github.com/SpaceJesusJPG) 
