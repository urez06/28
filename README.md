Introduction
------------
Репозитарий содержит базовый набор тестов для https://b2c.passport.rt.ru
Он включает в себя набор тестов для тестирования авторизации, структуру страниц, а также тестов для страницы восстановления и регистриции

Files
-----
[pages/config.py](pages/config.py) Содержит значение переменных (логин, пароли и т.п.) которые будут использоваться в дальнейшем.

[pages/init_page.py](pages/init_page) Включает в себя класс для работы с начальной страницей.

[pages/auth_page.py](pages/init_page) Включает в себя класс для работы по проверки авторизации.

[pages/reg_page.py](pages/init_page) Включает в себя класс для работы по проверки регистрационной формы.

[pages/base.py](pages/base.py) Включает в себя базовый PageObject описание.

[pages/elements.py](pages/elements.py) Включает в себя вспомогательный класс для работы с элементами страниц.

[tests/test_auth_page.py](tests/test_auth_page.py) Содержит тесты для авторизации

[tests/test_reg_page.py](tests/test_reg_page.py) Содержит тесты работы со страницей регистрации

[tests/test_page_structure.py](tests/test_page_structure.py) Содержит тесты для проверки требования к оформлению страницы



How To Run Tests
----------------

1) Установите необходимые модули:

    ```bash
    pip3 install -r requirements
    ```

2) Скачайте Selenium WebDriver из https://chromedriver.chromium.org/downloads 

3) Запустите тесты:

    ```bash
    python3 -m pytest -v --driver Chrome --driver-path ~/chrome tests/*
    ```

   ![alt text](example.png)

Note:
~/chrome Предполагается что драйвер был установлен на предыдущем шаге #2.
