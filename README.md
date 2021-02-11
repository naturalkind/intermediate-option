# intermediate-option
Вектора размерностью 35005x1 ресурсоемкие в сравнении, попробую использовать предобученную сетьVGG16 для уменьшения размерности 500x1.  
1. Cоздать массив заполненный 0 размерностью 150552x1
2. Вставить 35005x1 в массив 150552x1
3. Конвертировать в размерность 224x224x3
4. Обработать в VGG, получить 500x1
5. Сравнивать.  
Сделать замеры скорости.

Пример словаря с ID клиентов:  
"группа 1":[ "9834", "23", "23121", ....]  
"группа 2":[ "983", "3"]  

После получения этих групп, мы сможем посмотреть в каждую группу:
- средний чек  
- количество покупок   
- популярный продукт в группе  
- доминирующий продукт
- доминирующий пол
- активность клиента по его полям 'join_club_success', 'Could_send_sms', 'Could_send_email'
С данным вроде все отлично их много :)
Допустим получим 20т групп, мы сможем по очереди анализировать каждую, снизить вычислительную нагрузку - это мое предположение и рассчитываю что оно верное.

# TODO
+ исправить медленные куски кода/оптимезировать
+ создать классы/модули
+ структурировать
##### <a name="Parag"></a>	Выводы:
1. Из всего множества пользователей, 4,14% вернулись в 2020.  
![Иллюстрация к проекту](https://github.com/evilsadko/intermediate-option/blob/main/github/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202021-02-10%2019-17-02.png)
2. Из 35376 наименований продуктов, продовались 24290 наименования, 31,4% можно снизить на складе или убрать вообще  
![Иллюстрация к проекту](https://github.com/evilsadko/intermediate-option/blob/main/github/Figure_5.png)
3. 59843 покупателя, совершили 82705 покупки, купив 8239567 едениц товара. На диаграмме показаны товары суммарный обьем продажи привышаеющий 0.5%
![Иллюстрация к проекту](https://github.com/evilsadko/intermediate-option/blob/main/github/Figure_6.png)
4. Диаграмма отображает процент средней активности пользователей из 4,14% вернувшихся в 2020. Активными считаем тех,  
кто оставил какие либо данные или вступил в клуб
![Иллюстрация к проекту](https://github.com/evilsadko/intermediate-option/blob/main/github/Figure_7.png)
5. Самые активыне, вступили в клуб, оставили номер телефона, электронную почту, из 4,14% вернувшихся в 2020. Основной клиент комапании,   
для более детальных выводов нужен анализ потраченых средств
![Иллюстрация к проекту](https://github.com/evilsadko/intermediate-option/blob/main/github/Figure_8.png)
6. Процентное соотношение пола
![Иллюстрация к проекту](https://github.com/evilsadko/intermediate-option/blob/main/github/Figure_9.png)
7. Поиск аномалий в 3D пространстве, Покупатели/Покупки/Продукты
![Иллюстрация к проекту](https://github.com/evilsadko/intermediate-option/blob/main/github/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202021-02-10%2023-49-29.png)
![Иллюстрация к проекту](https://github.com/evilsadko/intermediate-option/blob/main/github/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202021-02-10%2023-48-36.png)
8. 82705 покупок, 8239567 продуктов, среднее количество продуктов в покупке 99,6. Диаграмма не однородна,  
3 аномалии, количество покупок привышает в 17 раз в сравнении с другими
![Иллюстрация к проекту](https://github.com/evilsadko/intermediate-option/blob/main/github/Figure_1.png)
![Иллюстрация к проекту](https://github.com/evilsadko/intermediate-option/blob/main/github/Figure_4.png)
![Иллюстрация к проекту](https://github.com/evilsadko/intermediate-option/blob/main/github/Figure_3.png)
