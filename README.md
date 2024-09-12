# Adventure_Works

### Dashboard Link : 

## Постановка задачи

Эта информационная панель помогает компании:
- отслеживать товары, каких категорий и подкатегорий клиенты заказывали чаще всего;
- увидеть основные показатели эффективности бизнеса – доход, количество заказов и возвраты за текущий месяц;
- вывести топ-1 продукт по количеству заказов и топ-1 продукт, который приносит больше всего прибыли. Это могут быть два разных продукта;
- проанализировать каждый конкретный продукт: был ли выполнен поставленный план по кол-ву заказов, доходу и не превышен ли лимит по возвратам для данного товара;
- увидеть тенденцию по прибыли по неделям и прогноз на будущее для конкретного товара;
- отслеживать какие клиенты принесли больше всего прибыли, а также к какой демографической группе относятся данные покупатели;
- увидеть возвраты топовых клиентов.



### Выполненные шаги

- Шаг 1 : Подключение к сырым данным.
- Шаг 2 : Построение реляционной модели данных.
- Шаг 3 : Создание новых вычисляемых столбцов и мер DAX.
- Шаг 4 : Создание интерактивного отчета для анализа и визуализации данных.

### Меры DAX

### Описание дашборда

Лист Executive Summary
1)Логотип компании
2) Срез
 
![Dashboard_upload](https://user-images.githubusercontent.com/102996550/174074051-4f08287a-0568-4fdf-8ac9-6762e0d8fa94.jpg)

### Инсайды

for creating new column following DAX expression was written;
       
        Age Group = 
        
        if(airline_passenger_satisfaction[Age]<=25, "0-25 (25 included)",
        
        if(airline_passenger_satisfaction[Age]<=50, "25-50 (50 included)",
        
        if(airline_passenger_satisfaction[Age]<=75, "50-75 (75 included)",
        
        "75-100 (100 included)")))
        
Snap of new calculated column ,

![Snap_1](https://user-images.githubusercontent.com/102996550/174089602-ab834a6b-62ce-4b62-8922-a1d241ec240e.jpg)

        
 - Step 18 : The report was then published to Power BI Service.
 
 
![Publish_Message](https://user-images.githubusercontent.com/102996550/174094520-3a845196-97e6-4d44-8760-34a64abc3e77.jpg)

# Snapshot of Dashboard (Power BI Service)

![dashboard_snapo](https://user-images.githubusercontent.com/102996550/174096257-11f1aae5-203d-44fc-bfca-25d37faf3237.jpg)

 
 # Report Snapshot (Power BI DESKTOP)

 
![Dashboard_upload](https://user-images.githubusercontent.com/102996550/174074051-4f08287a-0568-4fdf-8ac9-6762e0d8fa94.jpg)

# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### [1] Total Number of Customers = 129880

   Number of satisfied Customers (Male) = 28159 (21.68 %)

   Number of satisfied Customers (Female) = 28269 (21.76 %)

   Number of neutral/unsatisfied customers (Male) = 35822 (27.58 %)

   Number of neutral/unsatisfied customers (Female) = 37630 (28.97 %)


           thus, higher number of customers are neutral/unsatisfied.
           
### [2] Average Ratings

    a) Baggage Handling - 3.63/5
    b) Check-in Service - 3.31/5
    
