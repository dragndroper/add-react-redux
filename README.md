# Приложение "Add post" на React-Redux

Приложение реализовано на основе React и Redux. Оно представляет собой 
интерфейс, позволяющий добавлять посты и загружать данные с другого домена.

* Кнопка "Создать" - это "синхронные посты".  

Введите текст в поле input и нажмите "Создать" или нажмите Enter.
Нельзя добавить пустой пост, - Вы увидите предупреждение.
Нельзя использовать запрещенные слова ('bad', 'example', 'spam').

* Кнопка "Загрузить" - это "асинхронные посты".  

Нажмите на кнопку и произойдет асинхронный fetch-запрос на другой домен.
Используется метод чтения "json". Во время загрузки показан loader.
Если произойдет сетевая ошибка, - Вы увидите предупреждение. Код обернут в конструкцию try {} catch (err) {}.  

Асинхронность функционирует на основе библиотеки redux-thunk. Позже переделал на redux-saga. Принциальное отличие в том, что redux-saga работает с асинхронным кодом на основе функций-генераторов function* и здесь чистые функции, большая функциональность, но нельзя использовать reducer'ы. У redux-thunk отличие в том, что компонент не знает об асинхронном действии.

***Все предупреждения исчезают через 3 сек.***

В процессе создания приложения использовались:

- React Developer Tools,
- Redux DevTools,
- redux-thunk (async),
- redux-saga,
- json placeholder.

### `Скриншот`

![Alt-add-post](https://s10.gifyu.com/images/React-Redux-App.gif "add post")
