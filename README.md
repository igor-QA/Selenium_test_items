Создайте GitHub-репозиторий, в котором будут лежать файлы conftest.py и test_items.py.
Добавьте в файл conftest.py обработчик, который считывает из командной строки параметр language.
Реализуйте в файле conftest.py логику запуска браузера с указанным языком пользователя. Браузер должен объявляться в фикстуре browser и передаваться в тест как параметр.
В файл test_items.py напишите тест, который проверяет, что страница товара на сайте содержит кнопку добавления в корзину. Например, можно проверять товар, доступный по http://selenium1py.pythonanywhere.com/catalogue/coders-at-work_207/.

*Тест должен запускаться с параметром language следующей командой:  pytest --language=es
*Проверка работоспособности кода для разных языков. Добавьте в файл с тестом команду time.sleep(30) сразу после открытия ссылки. Запустите тест с параметром --language=fr и визуально проверьте, что фраза на кнопке добавления в корзину выглядит так: "Ajouter au panier".
*Браузер должен объявляться в фикстуре browser и передаваться в тест как параметр.
*В тесте проверяется наличие кнопки добавления в корзину. Селектор кнопки является уникальным для проверяемой страницы. Есть assert.
*Название тестового метода внутри файла test_items.py соответствует задаче. Название test_something не удовлетворяет требованиям/
