Работаем с объектом "Таблица данных"
      Программно создаём таблицу с заданными характеристиками, добавляем туда данные строк и вычисляемый столбец,
      считаем по формулам с помощью агрегатных выражений.

        1.Создать строку   
        2.Добавить строку в базу
        3.Создать вычисляемый столбец
        4.Добавить строку в базу
        5.Создали таблицу
        6.Добавили данные в строки
		Console.WriteLine("Avg(Оплата) = " + Formula.Exec("Avg(Оплата)"));
		
        7.Посчитали по формуле
        DataColumn dc = Formula.CreateColumn("Итого", typeof(double), "Оплата - Оплата * Комиссия");
        Console.WriteLine("Sum(Итого) = " + Formula.Exec("Sum(Итого)"));
			
        8.Посчитали выражение над добавленным столбцом
        (30000-30000*0.15)+(40000-40000*0.20)