# negative&positive samples 
Выборки, использованные в работе "Прогнозирование неблагоприятных эффектов межлекарственных взаимодействий на сердечно-сосудистую систему на основе анализа связей структура-активность".

Каталог содежит выборки, используемые в вышеупомянутой работе. Для удобства каждая выборка разбита на две части: позитивные и негативные эффекты, что видно по постфиксам "_pos" и "_neg" соответственно; первая же часть названия файла представляет собой название Нежелательной Лекарственной Реакции (НЛР).

Каждый файл представляет собой текстовый файл со столбцами, разделёнными табуляцией.
Структура каждого файла следующая:
1.	id - уникальный идентификатор пары.
2.	Drug_1 и Drug_2 - идентификаторы базы данных DrugBank (<https://go.drugbank.com/>).
3.	class - характеристика лекарства по отношению к конкретному НЛР. Если 1, то данная пара вызывает данную НЛР и не вызывает, если равно 0.

# do_pass
Файл do_pass содержит исходную информацию по МЛВ, полученную из DrugBank путём парсинга с использованием регулярных выражений .

Структура файла:
1.	Drug_1 Drug_2	- идентификаторы базы данных DrugBank (<https://go.drugbank.com/>).
2.	Adverse_effect	- названии НЛР в соответствии со словарём MedDRA (<https://www.meddra.org/>)
3.	Meddra_ID	- идентификатор MedDRA
4.	Meddra_category - категория MedDRA
