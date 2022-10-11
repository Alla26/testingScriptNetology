# Сценарии перехода к форме

**Путь № 1**
Главная страница -> Каталог курсов -> Программирование -> Тестировщик ПО

**Путь № 2**
Главная страница -> В Направлениях обучения -> Программирование -> Тестировщик ПО

**Путь № 3**
Главная страница -> Каталог курсов -> Полный каталог -> Тестировщик ПО

**Путь № 4**
Главная страница -> В Выберите вектор развития -> Выбрать курс -> Тестировщик ПО

**Путь № 5**
Главная страница -> В футере страницы Обучение -> Каталог курсов -> Тестировщик ПО

**Путь № 6**
Главная страница -> В футере страницы Обучение -> Программирование -> Тестировщик ПО

**Путь № 7**
Главная страница -> В футере страницы Обучение -> Популярные курсы -> Тестировщик ПО

# Путь к форме со страницы курса

**Путь №1**
Страница курса -> Кнопка Записаться

**Путь №2**
Страница курса -> Прокрутить страницу до конца до формы записи

**Путь №3**
Страница курса -> При прокручивании страницы вниз в хэдере появляется кнопка Записаться

# Сценарии тестов

*для выполнения каждого теста существует предусловие: необходимо переместиться одним из приведенных выше способом на
страницу формы записи*

**Ввод валидных значений в поле Имя:**

1. Ввод в поле Имя кириллицы с буквой Ё
   <p>Ввести в поле Имя : Алёна</p>
   <p>Ввести в поле Телефон : +79999999999</p>
   <p>Нажать кнопку Записаться</p>

2. Ввод в поле Имя латиницы
   <p>Ввести в поле Имя : Sonya</p>
   <p>Ввести в поле Телефон : +79999999999</p>
   <p>Нажать кнопку Записаться</p>

3. Ввод в поле Имя кириллицы с дефисом
   <p>Ввести в поле Имя : Анна-Виктория</p>
   <p>Ввести в поле Телефон : +79999999999</p>
   <p>Нажать кнопку Записаться</p>

4. Ввод в поле Имя латиницы с дефисом
   <p>Ввести в поле Имя : Anne-Jacqueline</p>
   <p>Ввести в поле Телефон : +79999999999</p>
   <p>Нажать кнопку Записаться</p>

5. Ввод в поле Имя кириллицы 2 символа
   <p>Ввести в поле Имя : Ия</p>
   <p>Ввести в поле Телефон : +79999999999</p>
   <p>Нажать кнопку Записаться</p>

6. Ввод в поле Имя кириллицы с маленькой буквы
   <p>Ввести в поле Имя : иван</p>
   <p>Ввести в поле Телефон : +79999999999</p>
   <p>Нажать кнопку Записаться</p>

7. Ввод в поле Имя латиницы с маленькой буквы
   <p>Ввести в поле Имя : kseniya</p>
   <p>Ввести в поле Телефон : +79999999999</p>
   <p>Нажать кнопку Записаться</p>

8. Ввод в поле Имя кириллицы с апострофом
   <p>Ввести в поле Имя : Д'Артаньян</p>
   <p>Ввести в поле Телефон : +79999999999</p>
   <p>Нажать кнопку Записаться</p>

9.  Ввод в поле Имя латиницы с апострофом
    <p>Ввести в поле Имя : D'Andre</p>
    <p>Ввести в поле Телефон : +79999999999</p>
    <p>Нажать кнопку Записаться</p>

10. Ввод в поле Имя латиницы и пробела
    <p>Ввести в поле Имя : Jack son</p>
    <p>Ввести в поле Телефон : +79999999999</p>
    <p>Нажать кнопку Записаться</p>

11. Ввод в поле Имя кириллицы и пробела
    <p>Ввести в поле Имя : Иван Иванов</p>
    <p>Ввести в поле Телефон : +79999999999</p>
    <p>Нажать кнопку Записаться</p>

* Ожидаемый результат при заполнении формы валидными данными: запрос успешно обрабатывается, появляется сообщение, что
запись осуществлена

**Ввод невалидных значений в поле Имя:**

12. Ввод в поле Имя кириллицы 1 символ
    <p>Ввести в поле Имя : Ю</p>
    <p>Ввести в поле Телефон : +79999999999</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат: запрос не обрабатывается, появляется сообщение о том, что в поле имя возможно ввести только более 2х символов

13. Ввод в поле Имя кириллицы 50 символ
    <p>Ввести в поле Имя : Яяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяяя</p>
    <p>Ввести в поле Телефон : +79999999999</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат: запрос не обрабатывается, появляется сообщение о том, что в поле имя превышено допустимое количество символов

14. Ввод в поле Имя кириллицы со спецсимволом
    <p>Ввести в поле Имя : Иннокен+тий</p>
    <p>Ввести в поле Телефон : +79999999999</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат: запрос не обрабатывается, появляется сообщение о том, что в поле имя можно ввести кириллицу, латиницу, дефис, апостороф, Ё

15. Ввод в поле Имя кириллицы и цифры
    <p>Ввести в поле Имя : Том5</p>
    <p>Ввести в поле Телефон : +79999999999</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат: запрос не обрабатывается, появляется сообщение о том, что в поле имя можно ввести кириллицу, латиницу, дефис, апостороф, Ё

16. Ввод в поле Имя кириллицы и тегов
    <p>Ввести в поле Имя : Мари>я</p>
    <p>Ввести в поле Телефон : +79999999999</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат: запрос не обрабатывается, появляется сообщение о том, что в поле имя можно ввести кириллицу, латиницу, дефис, апостороф, Ё

17. Ввод в поле Имя латиницы и тегов
    <p>Ввести в поле Имя : Jo>n</p>
    <p>Ввести в поле Телефон : +79999999999</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат: запрос не обрабатывается, появляется сообщение о том, что в поле имя можно ввести кириллицу, латиницу, дефис, апостороф, Ё


**Ввод валидных значений в поле Телефон:**


18. Ввод в поле Телефон номера телефона через 8
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : 89999999999</p>
    <p>Нажать кнопку Записаться</p>

19. Ввод в поле Телефон номера телефона без международного кода
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : 9999999999</p>
    <p>Нажать кнопку Записаться</p>

20. Ввод в поле Телефон номера телефона через дефис
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : +7-999-999-99-99</p>
    <p>Нажать кнопку Записаться</p>

21. Ввод в поле Телефон номера телефона со скобками
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : +7(999)9999999</p>
    <p>Нажать кнопку Записаться</p>

22. Ввод в поле Телефон номера телефона со скобками и дефисами
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : +7(999)999-99-99</p>
    <p>Нажать кнопку Записаться</p>

23. Ввод в поле Телефон номера телефона с пробелами
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : +7 999 999 99 99</p>
    <p>Нажать кнопку Записаться</p>

24. Ввод в поле Телефон номера телефона со скобками, пробелами и дефисами
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : +7 (999) 999-99-99</p>
    <p>Нажать кнопку Записаться</p>

25. Ввод в поле Телефон номера телефона со скобками и пробелами
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : +7 (999) 9999999</p>
    <p>Нажать кнопку Записаться</p>

26. Ввод в поле Телефон номера телефона со пробелами и дефисами
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : +7 999-999-99-99</p>
    <p>Нажать кнопку Записаться</p>


* Ожидаемый результат при заполнении формы валидными данными: запрос успешно обрабатывается, появляется сообщение, что
запись осуществлена

**Ввод невалидных значений в поле Телефон:**

27. Ввод в поле Телефон номера телефона с символом на кириллице
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : +79999999А99</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат: запрос не обрабатывается, появляется сообщение о том, что в поле телефон можно внести только цифры, +, пробел, (), дефис

28. Ввод в поле Телефон номера телефона со спецсимволом
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : 89999999=99</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат: запрос не обрабатывается, появляется сообщение о том, что в поле телефон можно внести только цифры, +, пробел, (), дефис

29. Ввод в поле Телефон номера телефона с тегом
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : +79999999>99</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат: запрос не обрабатывается, появляется сообщение о том, что в поле телефон можно внести только цифры, +, пробел, (), дефис

30. Ввод в поле Телефон номера телефона апострофом
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : +79999999'99</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат: запрос не обрабатывается, появляется сообщение о том, что в поле телефон можно внести только цифры, +, пробел, (), дефис

31. Ввод в поле Телефон номера телефона с символом на латинице
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : +799F9999999</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат: запрос не обрабатывается, появляется сообщение о том, что в поле телефон можно внести только цифры, +, пробел, (), дефис

32. Ввод в поле Телефон девяти цифр
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : 999999999</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат: запрос не обрабатывается, появляется сообщение о том, что в поле телефон необходимо ввести минимум 10 цифр

33. Ввод в поле Телефон 50ти цифр
    <p>Ввести в поле Имя : Ева</p>
    <p>Ввести в поле Телефон : 99999999999999999999999999999999999999999999999999</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат: запрос не обрабатывается, появляется сообщение о том, что в поле телефон превышено максимально возможное количество символов


**Проверка функции заполнения и отправки формы**

**Позитивный сценарий:**

34. Ввести в поле Имя валидное значение Ева
    <p>Ввести в поле Телефон валидное значение +79999999999</p>
    <p>Нажать кнопку Записаться</p>

* Ожидаемый результат при заполнении формы валидными данными: запрос успешно обрабатывается, появляется сообщение, что
  запись осуществлена

**Негативные сценарии:**

35. Ввести в поле Имя невалидное значение Ка555
    <p>Ввести в поле Телефон валидное значение +79999999999</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат при заполнении формы невалидными данными: запрос не обрабатывается, появляется сообщение, что необходимо скорректировать поле Имя

36. Ввести в поле Имя валидное значение Ева
    <p>Ввести в поле Телефон невалидное значение 7999</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат при заполнении формы невалидными данными: запрос не обрабатывается, появляется сообщение, что необходимо скорректировать поле Телефон

37. Оставить поле Имя пустым
    <p>Оставить поле Телефон пустым</p>
    <p>Нажать кнопку Записаться</p>

 *  Ожидаемый результат при незаполненной форме: запрос не обрабатывается, появляется сообщение, что необходимо заполнить поля Имя и Телефон

38. Оставить поле Имя пустым
    <p>Ввести в поле Телефон валидное значение +79999999999</p>
    <p>Нажать кнопку Записаться</p>

  * Ожидаемый результат при незаполненной форме: запрос не обрабатывается, появляется сообщение, что необходимо заполнить поле Имя

39. Ввести в поле Имя валидное значение Ева
    <p>Оставить поле Телефон пустым</p>
    <p>Нажать кнопку Записаться</p>

 *  Ожидаемый результат при незаполненной форме: запрос не обрабатывается, появляется сообщение, что необходимо заполнить поле Телефон

# Перечень используемых инструментов

1. IntelliJ IDEA 2022.1.2 (Community Edition) как среда разработки для написания автотестов;
2. OpenJDK 11 платформа Java;
3. Браузер Chrome и chromedriver - браузер для работы со страницей, программа для передачи команд браузеру;
4. Selenide - инструмент для автоматизации действия пользователя в браузере;
5. JUnit Jupiter как среда тестирования для приложений Java;
6. Lombok как библиотека для сокращения кода в классах;
7. Gradle как система автоматической сборки;
8. Github в качестве хранилища SUT и авто-тестов;
9. Allure для создания отчетов о выполнении авто-тестов.

# Перечень необходимых разрешений, данных и доступов

* Необходимо разрешение на автоматизированное тестирование
* Необходим доступ к базе данных и API

# Перечень и описание возможных рисков при автоматизации

1. Зависимость автотестов от текущей версии кода;
2. Стоимость автоматизации;
3. Необходимость поддерживать и модифицировать;
4. Трудность в поиске локаторов.

# Перечень необходимых специалистов для автоматизации

Инженер по автоматизированному тестированию

# Интервальная оценка с учётом рисков в часах

24 часа



