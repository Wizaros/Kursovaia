# Программа анализа данных о продажах товаров в магазине

Эта программа предназначена для анализа данных о продажах товаров в магазине. Она читает информацию из CSV-файла, а затем рассчитывает общую выручку магазина, находит товар, который был продан наибольшее количество раз, находит товар, который принес наибольшую выручку, и составляет отчет с дополнительной информацией о продажах.

## Использование программы

1. Запустите программу и выберите CSV-файл с данными о продажах, щелкнув по кнопке "Выберите файл CSV".
2. Программа автоматически прочитает данные из выбранного файла и проведет анализ.
3. После завершения анализа программа выведет отчет о продажах в таблице и графике.

## Описание работы программы

1. `readsales(filename)`: Эта функция считывает данные о продажах из CSV-файла и возвращает их в виде списка словарей.
2. `choose_file()`: Эта функция открывает диалоговое окно для выбора CSV-файла и возвращает путь к выбранному файлу.
3. `Hash`: Этот класс реализует хеш-таблицу для быстрого доступа к данным о продажах по имени товара.
4. `Salyzer`: Этот класс проводит анализ данных о продажах. Он рассчитывает общую выручку магазина, находит товары, проданные наибольшее количество раз, и товары, принесшие наибольшую выручку.
5. `generate(sales_data, total_revenue)`: Эта функция генерирует отчет о продажах на основе данных о продажах и общей выручки магазина.
6. `SalesTableWidget`: Этот класс создает окно с отчетом о продажах в виде таблицы.
7. `closeEvent(self, event)`: Этот метод переопределяет обработчик события закрытия окна, чтобы запросить подтверждение перед закрытием программы.

## Реализованные задачи

1. **Рассчитать общую выручку магазина**: Программа автоматически вычисляет общую выручку магазина на основе данных о продажах.
2. **Найти товар, который был продан наибольшее количество раз**: Программа определяет товар, который был продан наибольшее количество раз, используя хеш-таблицу для подсчета количества проданных единиц каждого товара.
3. **Найти товар, который принес наибольшую выручку**: Программа находит товар, который принес наибольшую выручку, суммируя общую стоимость продаж для каждого товара и выбирая товар с наибольшей выручкой.
4. **Составить отчет о продажах**: Программа составляет отчет, содержащий информацию об общей выручке магазина, количестве проданных единиц каждого товара и их доле в общей выручке.

## Ограничения при использовании Jupyter Notebook
1. **Библиотека PyQt5**: Использование графических интерфейсов, особенно в интерактивном режиме, может вызвать проблемы в Jupyter Notebook.
2. **Диалоговые окна**: Диалоговые окна, такие как окно выбора файла, могут не отображаться или вызывать проблемы в Jupyter Notebook.
3. **Отображение графиков**: Графики, созданные с помощью Matplotlib, обычно отображаются в Jupyter Notebook без проблем, но иногда может потребоваться использовать магическую команду `%matplotlib inline`.
4. **Интерактивность**: Некоторые функции программы, например, обработка событий или взаимодействие с пользователем, могут не работать или не отображаться в Jupyter Notebook.

## Использование
Программу можно запустить из среды разработки, такой как Visual Studio Code, с расширением ipynb, или из Jupyter Notebook.
При возникновении ошибки "The Kernel "Python ... died" при нажатии на кнопку "Run All" рекомендуется нажать "Restart" и попробовать вновь.