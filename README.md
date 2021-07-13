# Тестовое задание на позицию frontend разработчика

Результат выполнения задания нужно будет оформить здесь же, на гитхабе. Желательный срок выполнения 5 дней с момента получения задания.
В качестве ответа __не нужно__ присылать никаких ZIP-архивов и наборов файлов. Все ваши ответы должны быть оформлены на https://github.com/.

Вы присылаете только ссылку на ваш репозиторий и нужную информацию https://24.future-group.ru/pub/form/5/2gwpyt/.
Если у вас еще нет аккаунта, то это хороший повод его завести.

Если есть вопросы, вы всегда их можете задать связавшись с человеком, который выдал вам задание.

## Задание

Необходимо разработать React-приложение поиска книг с помощью Google Books API. Документация: https://developers.google.com/books/docs/v1/using. Для авторизации запросов к API выбрать способ с предоставлением API key (https://developers.google.com/books/docs/v1/using#APIKey).

Дополнительным плюсом будет: Финальный билд приложения должен быть запускаться из __Docker контейнера__ (хотябы с минимальной конфигурацией)

__Функционал__

- Должны быть текстовое поле и кнопка поиска. По введенной пользователем подстроке производится поиск книг. Триггером к поиску является либо нажатие Enter (когда текстовое поле в фокусе), либо нажатие кнопки поиска.
- Фильтрация по категориям. Ниже текстового поля располагается селект с категориями: all, art, biography, computers, history, medical, poetry. Если выбрано "all" (выбрано изначально), то поиск производится по всем категориям.
- Сортировка. Рядом с селектом категорий находится селект с вариантами сортировки: relevance (выбран изначально), newest. 
- Найденные книги отображаются карточками, каждая из которых состоит из изображения обложки книги, названия книги, названия категории и имен авторов. Если для книги приходит несколько категорий, то отображается только первая. Авторы отображаются все. Если не приходит какой-либо части данных, то вместо нее просто пустое место.
- Над блоком с карточками отображается количество найденных по запросу книг.
- Пагинация реализована по принципу 'load more'. Ниже блока с карточками находится кнопка 'Load more', по клику на нее к уже загруженным книгам подгружаются еще. Шаг пагинации - 30.
- При клике на карточку происходит переход на детальную страницу книги, на которой выводятся ее данные: изображение обложки, название, все категории, все авторы, описание.

__Замечания__

- __Обязательно__ использование Typescript, Redux/MobX.
- Во время загрузки книг стоит показать какой-то индикатор
- Использование сторонних библиотек будет плюсом только в случае если это оправданно и вы сможете объяснить причину выбора. Показав свои знания в грамотном применении сторонних готовых решений, вы имеете шанс повысить свою профессиональную привлекательность для нас.
- Пишите код так, как бы вы его писали в работе &mdash; внутренности задания будут оцениваться даже тщательней, чем внешнее соответствие заданию. Код должен быть организован так, чтобы его можно было заново использовать.
- Помните про обработку ошибок!
- Верстка может быть самая простая, однако она не должна ломаться при разрешениях от 320px до 1920px. Визуализацию и украшение делайте на ваш вкус. Мы не против использования [Bootstrap](http://getbootstrap.com/) или похожего UI фреймворк, но только для UI представления (нельзя использовать JS код для решения задачи, но можно использовать для оформительских эффектов (анимации и тому подобное))!

__Примерный вид приложения__

![image](https://user-images.githubusercontent.com/61146708/125444523-829f6238-eb1c-42ff-a9c9-a3eb73ba24c4.png)
![image](https://user-images.githubusercontent.com/61146708/125444403-e868dec7-2977-4825-b751-5b2e5abc279a.png)


Дополнительно напишите нам, как вы тестировали результат своей работы. Какие используете инструменты и как вы осуществляете тестирование.

---
