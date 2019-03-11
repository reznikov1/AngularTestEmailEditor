# Тестовое задание на Angular

### Оглавление
1. [Описание задания](#Описание-задания)
2. [Установка](#Установка)

### Описание задания
Необходимо реализовать angular-компонент, который будет представлять собой поле для ввода емэйлов, автоматически формирующее емэйлы в блоки.
Нужно повторить поведение гугловской формы из окна "Совместный доступ", которое можно увидеть, если зайти Google Drive и на любом своем документе через контекстное меню вызвать пункт "Совместный доступ" (Share).

Требуемые поведение и реализация:

Каждый введенный емэйл формируется в блок. Блок можно удалить.
Блок формируется после нажатия Enter или установки запятой после емэйла, а также при потере фокуса полем ввода. Соответственно в блок может сформироваться любая строка.
Ширина поля зависит от ширины родительского контейнера. Если контейнер меняет ширину, блоки с емэйлами должны перераспределиться по строкам.
Вставленные через ctrl+V емэйлы должны формироваться в блоки.
Невалидные емэйлы должны формироваться в блоки с красным подчеркиванием.
При вводе большого кол-ва емэйлов появляется прокрутка.
HTML должен выглядеть примерно следующим образом:
<emails-editor ...attributes></emails-editor>

<button ng-click="...">Add email</button>

<button ng-click="...">Get email count</button>

Где:

<emails-editor> — это реиспользуемая ангуляровская директива с изолированным скопом, ответственная только за редактирование списка емейлов.

Реализация директивы <emails-editor> должна обеспечивать возможность реиспользования этой директивы в любом angular-приложении.

По клику на кнопку "add random email" в поле добавляется случайный емэйл сформированный в блок.

По клику на кнопку "get emails count" показывается alert с количеством введенных емэйлов 

Отправка задания:
Тестовое задание должно представлять собой законченный продукт и размещено по публично доступной ссылке.

Исходный код должен быть доступен через git или отправлен в zip-архиве.

Собранная версия задания должна лежать в репозитории или zip-архиве.
Описание к дизайну:
Шрифт Open sans
Размер заголовка 20рх
Цвет кнопок 6699ff

### Установка

Загрузите этот репозиторий с помощью git clone
```
$ git clone https://github.com/applegod4/AngularTestEmailEditor.git
```
Перейдите в папку с проектом
```
$ cd AngularTestEmailEditor
```
Затем установите необходимые зависимости
```
$ npm install
```
Запустите приложение
```
$ ng serve
```
После успешной сборки приложение будет доступно по адресу http://localhost:4200/

При возникновении ошибок обновите NodeJS и NPM. При разработке использовались NodeJS v10.2.1 и npm v6.1.0
