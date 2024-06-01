
<br>

# Автоматизация тестов для сайта https://qa-scooter.praktikum-services.ru/

<br>

### Тестовые сценарии:

##### Тестируем выпадающий список в разделе «Вопросы о важном»: 
````
1.1 Проверки: когда нажимаешь на стрелочку, открывается соответствующий текст
1.2 Отдельный тест на каждый вопрос
````
<br>



#### Тестируем весь флоу заказа самоката. Есть две точки входа в сценарий: кнопка «Заказать» вверху страницы и внизу

````
Из чего состоит позитивный сценарий:
1.1 Заполнить форму заказа
1.2 Проверить: 
    - что появилось всплывающее окно с сообщением об успешном создании заказа,
    - если нажать на логотип «Самоката», попадёшь на главную страницу «Самоката»,
    - Проверка: если нажать на логотип Яндекса, в новом окне откроется главная страница Яндекса.

````

### Для начала работы:
1. Установи webdriver: 
```
https://www.selenium.dev/documentation/webdriver/getting_started/install_drivers/
```
2. Установи зависимости из requirements.txt
```
pip3 install -r requirements.txt
```
3. Запусти тесты из корневого каталога проекта:
```
pytest tests --alluredir=allure_results
```
4. Посмотри отчет Allure:
```
allure serve allure_results 
```
