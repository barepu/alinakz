# Теория
1) Что такое ООП и для чего оно нужно ?
- ООП - объектно ориентированное программирование, главная идея ООП - мы можем мыслить объетами из настоящей
жизни, например есть объект Машина, у машины есть свойства производитель, марка, модель, есть действия ехать, повернуть, остановиться.

2) Что такое наследование, полиморфизм, инкапсуляция ?
- Наследование - с помощью наследования мы можем создавать новые классы на основе уже существующих,
что помогает не повторять код. Например есть родительский класс Машина, у него есть два дочерних класса
Легковая и Грузовая со своими дополнительными свойствами и методами, но при этом у них есть общие сойства и
методы которые они унаследовали от класса Машина.
- Полиморфизм - с помощью полиморфизма мы можем использовать методы дочерних классов в родительском.
К примеру у нас есть абстрактный класс Транспорт, у него есть метод повернуть, и есть два класса
Машина и Самолет, в этих классах метод повернуть будет описан у каждого по своему.
- Инкапсуляция - защита класса от неправильного использования. К примеру есть класс Машина и у него есть
свойство одометр, если это свойство будет public и доступно для изменения, то одометр можно будет
каждый раз сбрасывать(чего делать нельзя), для защиты это свойство делается private и для него
прописываются getter и setter(accessor,mutator)

3) Что такое MVC и в чём на Ваш взгляд его основное преимущество ?
- MVC - Model View Controller паттерн, с его помощью мы разграничиваем ответсвенность за функциональность приложения
Контроллер отвечает за обработку действий
Модель отвечает за данные, бизнес логику
Вью отвечает за отображение
Основное преимущество на мой взгляд - сторгая структура, благодаря которой в больших проектах проект не
превращается в кашу. Также новому сотруднику будет гораздо легче войти в проект.

4) Что такое фреймворк ?
- Фреймворк это как бы каркас, в котором уже есть базовые компоненты которые упрощают и ускоряют разрабоку
(авторизация, работа с бд и т.д.)

5) Какую реализацию технологии ORM использует фреймворк YII ?
- ActiveRecord

6) Для чего нужна нормализация баз данных ?
- для того чтобы в бд было меньше шансов на ошибку, и для уменьшения занимаемой памяти

7) Для чего нужно пространство имен ?
- Пространства имен нужны для того чтобы случайно не переопределить уже существующий класс, и для того чтобы
не создавать префиксы у классов если класс с аналогичным именем уже существует. В первой версии Yii как раз не было пространства имен, и многие классы начигались с префикcа C(CHtml)

8) Какие плюсы использования JavaScript в веб-приложении ?
- Добавляет интерактивности на страницу, можно проверять данные до отправки на сервер.

9) Что такое область видимости переменных ?
- Переменные бывают глобальными и локальными
глобальные это переменные которые объявлены вне функции
локальные - переменные объявленные внутри функции, и доступны они только внутри нее.

10) Что такое AJAX и в чём на Ваш взгляд его основное преимущество ?
- Это технология для обмена данными с сервером без перезагрузки страницы
Основное преимущество - удобство(пользователю не надо ждать пока перезагрузится вся страница)
экономичнее как для пользователя(меньше трафика) так и для сервера(не надо заново рендерить страницу)

11) Что такое JSON ?
- Javascript object notation - формат обмена данными

# Теория 2
* IDE JetBrains PhpStorm:
	* На какой платформе разработана данная IDE ? IDE написан на java, на платформе IntellijIdea
	* Наличие какого ПО необходимо для запуска IDE ? JDK
	* Какова стоимость ключа на 1 год ? [3] не знаю ))
	* Перечислите некоторые возможности IDE; поиск по всему проекту(double shift), мультиселект(alt+j),связка с
гитом, поддержка плагинов, автокомплит.
	* Как называется модальное окно настройки удаленных серверов ? Remote host
* ОС семейства Linux:
	* Какие преимущества есть у ОС данного семейства ? OpenSource, бесплатный, гибкость настройки
	* Какую графическую оболочку по-умолчанию использует дистрибутив Ubuntu, Debian ? Unity, Gnom
	* Какой менеджер пакетов они используют? 	aptitude(apt-get)
	* Напишите команду поиска файла hosts на локальном компьютере; find / -name hosts
	* Напишите команду подключения к удаленному серверу remote.com через порт 2222 под пользователем user1; ssh user1@remote.com -p 2222
	* Напишите команду копирования файла test.php на удаленный сервер remote.com через порт 2222 в директорию /var/www/html по ssh; scp
* VCS Git:
	* Для чего нужно данное ПО ? для котроля версий, можно создавать ветки и безболезненно откатываться при наличии багов, также просто необходим при работе в команде.
	* Напишите команду клонирования проекта test с удаленного сервера remote.com; git clone git@remote.com:test.git
	* Напишите команду создания ветки develop в проекте test и переход в неё; git checkout -b develop
	* Напишите команду слияние ветки develop в мастер; git merge develop

# Requirements
- База данных alina_db