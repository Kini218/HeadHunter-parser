# HeadHunter-parser
Парсинг HeadHunter с использованием selenium и занесением данных в excel

Как использовать:
1. Скачайте необходимые библиотеки(файл requirements).
2. Откройте файл hh_parser.

3.Вставьте строчки в конец файла.

'''parser1 = HH_Parser('название вакансии', количество вакансий)

vacancy_data = parser1.get_vacancy_information()

xl1 = Fill_Excel_Table('Имя excel файла')

xl1.fill_xl_table(vacancy_data)'''


Рекомендую искать не более 1000 вакансий, так как алгоритм весьма не быстрый.

Ниже прриведено количество вакансий(1 столбик) и затраченное время(2 столбик).

50	155

100	355

200	670

400	1580

Скрипт может подвисать(до 30 секунд)- это нормально(происходят внутренние ошибки selenium)
