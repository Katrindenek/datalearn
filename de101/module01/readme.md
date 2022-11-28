# Домашнее задание для модуля 1.

В данном домашнем задании требовалось
1. Построить диаграмму архитектуры аналитического решения своей или какой-либо иной компании.
2. Проанализировать данные из таблицы Sample-Superstore.xls, используя функции Excel, и построить дашборд.

## Архитектура аналитического решения

На диаграмме представлена архитектура аналитического решения рекламного агенства.

<img src="https://github.com/Katrindenek/datalearn/blob/e433f3723fb2cd922649fe5af0e733023d01df8b/de101/module01/Diagram/Diagram.drawio.png" width="400">

В слой _Source_ входят, например, выгрузка данных из Mediascope, собирающей различные метрики на ТВ, интернет-площадках и т.д., выгрузки из Google Analytics и Яндекс.Метрика со статистикой активности посетителей на веб-сайте, данные продаж и других метрик, получаемые от клиента, выгрузки статистики поисковых запросов по ключевым словам из Google Trends и Яндекс Wordstat, и др.

Слой _Storage_ — хранилище данных.

В слой _Business_ входят такие инструменты аналитики как Excel и Business Intelligence (в моем случае, это было Tableau), а также построение прогнозов с использованием алгоритмов Machine Learning (в моем случае, на Python). 

## Аналитика в Excel

Таблица [_Sample-Superstore.xls_](https://github.com/Katrindenek/datalearn/blob/e433f3723fb2cd922649fe5af0e733023d01df8b/de101/module01/Sample-Superstore.xls):
| Название столбца | Значение                          |
|------------------|-----------------------------------|
| Row ID           | Идентификатор строки (уникальный) |
| Order ID         | Идентификатор заказа              |
| Order Date       | Дата заказа                       |
| Ship Date        | Дата доставки                     |
| Ship Mode        | Класс доставки                    |
| Customer ID      | Идентификатор покупателя          |
| Customer Name    | Имя и фамилия покупателя          |
| Segment          | Сегмент покупателя                |
| Country          | Страна                            |
| City             | Город                             |
| State            | Штат                              |
| Postal Code      | Почтовый индекс                   |
| Region           | Регион                            |
| Product ID       | Идентификатор товара              |
| Category         | Категория                         |
| Sub-Category     | Подкатегория                      |
| Product Name     | Название товара                   |
| Sales            | Продажи (Доход)                   |
| Quantity         | Количество                        |
| Discount         | Скидка в %                        |
| Profit           | Прибыль                           |
| Person           | Региональный менеджер             |
| Returned         | Возвраты товара                   |

### Задание:
- Использовать Lookup:
 <img src="https://github.com/Katrindenek/datalearn/blob/128f29d386cf3985f24ea9a45f057b8cccd2c310/de101/module01/Pictures/%D0%92%D0%9F%D0%A0.png" width="400">
- Построить Сводную таблицу (выполнено в рамках дашборда)
- Построить примеры отчетов (выполнено в рамках дашборда)
- Создать дашборд:

#### Дашборд: Overview
- Total sales, total profit, profit ratio:

 <img src="https://github.com/Katrindenek/datalearn/blob/128f29d386cf3985f24ea9a45f057b8cccd2c310/de101/module01/Pictures/Total_Sales_Profit.png" width="400">

- Profit per Order:


Данные                     |  График
:-------------------------:|:-------------------------:
 | <img src="https://github.com/Katrindenek/datalearn/blob/128f29d386cf3985f24ea9a45f057b8cccd2c310/de101/module01/Pictures/Profit_per_order.png" width="250"> | <img src="https://github.com/Katrindenek/datalearn/blob/128f29d386cf3985f24ea9a45f057b8cccd2c310/de101/module01/Pictures/Profit_per_order_chart.png" width="600"> |

- Sales per customer

<img src="https://github.com/Katrindenek/datalearn/blob/128f29d386cf3985f24ea9a45f057b8cccd2c310/de101/module01/Pictures/Sales_per_Customer.png" width="200">

- Avg. Discount

<img src="https://github.com/Katrindenek/datalearn/blob/128f29d386cf3985f24ea9a45f057b8cccd2c310/de101/module01/Pictures/Average_Discount.png" width="200">

- Monthly Sales by Segment

Данные                     |  График
:-------------------------:|:-------------------------:
 | <img src="https://github.com/Katrindenek/datalearn/blob/128f29d386cf3985f24ea9a45f057b8cccd2c310/de101/module01/Pictures/Monthly_Sales_by_Segment.png" width="350"> | <img src="https://github.com/Katrindenek/datalearn/blob/128f29d386cf3985f24ea9a45f057b8cccd2c310/de101/module01/Pictures/Monthly_Sales_by_Segment_chart.png" width="600"> |
 
 - Monthly Sales by Product Category

Данные                     |  График
:-------------------------:|:-------------------------:
 | <img src="https://github.com/Katrindenek/datalearn/blob/128f29d386cf3985f24ea9a45f057b8cccd2c310/de101/module01/Pictures/Monthly_Sales_by_Category.png" width="350"> | <img src="https://github.com/Katrindenek/datalearn/blob/128f29d386cf3985f24ea9a45f057b8cccd2c310/de101/module01/Pictures/Monthly_Sales_by_Category_chart.png" width="600"> |
