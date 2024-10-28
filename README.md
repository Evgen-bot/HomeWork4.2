## План тестирования:
Перечень автоматизируемых сценариев:

_Сценарии навигации:_

#1 Переход на страницу заполнения формы заявки через меню “Каталог курсов”
 
Шаги:
* открыть в браузере сайт Нетологии
* кликнуть на “Каталог курсов”
* выбрать “все курсы”
* выбрать из списка “Инженер по тестированию”
* кликнуть кнопку “Записаться”
* в открывшейся форме записи ввести валидные данные в поля “Имя” и “телефон”

#2 Переход на страницу заполнения формы заявки через меню “Освоить профессию”
 
Шаги:
* открыть в браузере сайт Нетологии
* кликнуть на “Освоить профессию”
* выбрать из списка “Инженер по тестированию”
* кликнуть кнопку “Записаться”
* в открывшейся форме записи ввести валидные данные в поля “Имя” и “телефон”

#3 Переход на страницу заполнения формы заявки через меню “Программирование”
   
 Шаги:
*    открыть в браузере сайт Нетологии
*    кликнуть на кнопку “Программирование”
*    выбрать из списка “Инженер по тестированию”
*    кликнуть кнопку “Записаться”
*    в открывшейся форме записи ввести валидные данные в поля “Имя” и “телефон”

#4 Переход на страницу заполнения формы заявки через меню “Поиск”
   
 Шаги:
*    открыть в браузере сайт Нетологии
*    кликнуть на кнопку “Каталог курсов”
*    в строке поиска ввести “Инженер по тестированию”
*    кликнуть кнопку “Записаться”
*    в открывшейся форме записи ввести валидные данные в поля “Имя” и “телефон”


Валидные данные:

Поле “Имя” - Ввод на русском языке, допустим ввод тире, не допустимы цифры, спецсимволы, максимальная длина 30 символов; (Например, Евгений)

Поле “Телефон” - +7 далее 10 цифр, не допустим ввод букв, спецсимволов. (Например, +7 9555000214);

Поле “Электронная почта” - Ввод на английском языке, допустимы ввод цифр, обязательно наличие “символа” - “@” (Например, obuchenie2024@yandex.ru)


_Сценарии заполнения и отправки формы записи:_

Предусловие:
На сайте Нетология перейти на страницу с формой записи

#1 Отправка формы записи при вводе валидных данных
  
 Шаги:
*    ввести в поле “Имя” валидные данные
*    ввести в поле “Телефон” валидные данные
*    ввести в поле “Электронная почта” валидные данные
*    кликнуть кнопку “Записаться”
   Ожидаемый результат:
   переход на страницу с сообщением “Запись произведена успешно. В ближайшее время с Вами свяжется оператор”

#2 Отправка формы записи при вводе невалидных данных в поле “Имя”
   
Шаги:
*    ввести в поле “Имя” невалидные данные
*    ввести в поле “Телефон” валидные данные
*    ввести в поле “Электронная почта” валидные данные
*    кликнуть кнопку “Записаться”
   Ожидаемый результат:
   Вывод сообщения: “Проверьте данные в поле “Имя””

#3 Отправка формы записи при вводе невалидных данных в поле “Телефон”
   
Шаги:
*    ввести в поле “Имя” валидные данные
*    ввести в поле “Телефон” невалидные данные
*    ввести в поле “Электронная почта” валидные данные
*    кликнуть кнопку “Записаться”
   Ожидаемый результат:
   Вывод сообщения: “Проверьте данные в поле “Телефон””

#4 Отправка формы записи при вводе невалидных данных в поле “Электронная почта”
   
Шаги:
*    ввести в поле “Имя” валидные данные
*    ввести в поле “Телефон” валидные данные
*    ввести в поле “Электронная почта” невалидные данные
*    кликнуть кнопку “Записаться”
   Ожидаемый результат:
   Вывод сообщения: “Проверьте данные в поле “Электронная почта””

_Перечень используемых инструментов:_
Gradle, Idea, JUnit, Selenide, JDK 11, lombok

_Перечень необходимых разрешений, данных и доступов:_
Доступ к базам данных, API

_Перечень и описание возможных рисков при автоматизации:_
Изменения на сайте, баги

_Перечень необходимых специалистов для автоматизации:_
Инженер по автоматизации


_Интервальная оценка с учётом рисков:_
150 часов
