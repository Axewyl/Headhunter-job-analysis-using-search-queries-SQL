# Проект-1. Анализ резюме из HeadHunter

## Оглавлелние
[1. Описание проекта](https://github.com/Axewyl/Resume_analysis_from_HeadHunter/blob/master/README.md#Описание-проекта)

[2. Какой кейс решаем?](https://github.com/Axewyl/Resume_analysis_from_HeadHunter/blob/master/README.md#Какой-кейс-решаем)

[3. Краткая информация о данных](https://github.com/Axewyl/Resume_analysis_from_HeadHunter/blob/master/README.md#Краткая-информация-о-данных)

[4. Этапы работы над проектом](https://github.com/Axewyl/Resume_analysis_from_HeadHunter/blob/master/README.md#Этапы-работы-над-проектом)

[5. Результат](https://github.com/Axewyl/Resume_analysis_from_HeadHunter/blob/master/README.md#Результаты)

[6. Выводы](https://github.com/Axewyl/Resume_analysis_from_HeadHunter/blob/master/README.md#Выводы)

### Описание проекта
В нашем распоряжении база резюме от соискателей, выгруженная с сайта поиска вакансий *hh.ru*.

Файл с исходными данными о резюме вы можете скачать [здесь](https://drive.google.com/file/d/1-VHPNxV_KmodxAGc-7ds2ysp6AHki_nt/view?usp=share_link).

Файл с исходными данными о курсах валют вы можете скачать [здесь](https://drive.google.com/file/d/1-WEtU7wc2ZmoOvdl3RlRBNOZlRbN2zTM/view?usp=share_link)

**Так же рекомедуем**. В проекте на *GitHube* не отображаются графики *plotly*. Для успешного просмотра перейдите на [nbviewer](https://nbviewer.org/) и вставте ссылку:

https://github.com/Axewyl/Resume_analysis_from_HeadHunter/blob/master/Project-1.%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7_%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5_%D0%B8%D0%B7_HeadHunter.ipynb

:arrow_up:[к оглавлнию](https://github.com/Axewyl/Resume_analysis_from_HeadHunter/blob/master/README.md#Оглавлелние)

### Какой кейс решаем
- Внимательно изучаем детали задачи.
- Ознакомимся с дополнительным теоретическим материалом, который даётся перед заданием.
- Воспользуемся советами и подсказками при выполнении проекта.
- Ответим на все контрольные вопросы.
- Загрузим ноутбук со своим решением на *GitHub*, оформив его в соответствии с требованиями *PEP8*.
- Сдаём проект на проверку и делаем выводы по разведывательному анализу.

**Описание задачи:**
Компания *HeadHunter* хочет построить модель, которая бы автоматически определяла примерный уровень заработной платы, подходящей пользователю, исходя из информации, которую он указал о себе. Но, как вы знаете, прежде чем построить модель, данные необходимо преобразовать, исследовать и очистить.

**Метрика качества**
В процессе работы мы сформировали новые столбцы признаки, удалив старые менее информативные. Очистили данные от выбросов, которые искажают информативность и качество данных. Нашли зависимости в признаках, построили графики и сделали выводы.
Применили метод z-отклонений, основанный на возможности логорифмировать признак, применить гибкий подход 3-х сигм(средних квадратных отклонений).

**Что практикуем**
- Учимся работать с большим объёмом информации табличных данных;
- исследовать, изменять и добавлять новые признаки;
- очищать данные и строить графики; 
- делать взвешенные выводы.

### Краткая информация о данных
Таблица состоит из введённой информации от соискателей в поиске работы. Она состоит из 12 колонок признаков которые пользователь указал о себе. В данной работе учитывается информация о 44744 соискателях в поиске работы по г.Москве, г.Санкт-Петербургу и дргим городам.

### Этапы работы над проектом
1. базовый анализ структуры данных
2. преобразование данных
3. разведывательный анализ
4. очистка данных

### Результаты
1. Исходная база данных состоит из 44744 строк и 12 колонок.
2. Преобразовав, мы получили базу данных из 44482 записей и 23 колонок-признаков.
3. Разведовательный анализ показал:
    - колличество соискателей в зависимости от возроста;
    - уровни распределения желаемой заработной платы(ЗП) сосискателей;
    - зависимость ЗП от уровня образования
    - зависимость ЗП от города;
    - как влияют командировки и переезды на уровень ожидаемой ЗП сосискателей;
    - зависимоть опыта работы от возраста
    - и др.
4. При очистке данных, мы избавились от дубликатов, выбросов. Заполнили пропускив таблице.

### Выводы
В результате продланной работы, определи что:
- Возраст большинства соискателей находится в пределах от 20 до 40 лет.
- Опыт большинства сосикателей находится в пределах от 50 до 150 месяцев.
- Уровень зарплаты большинства соискателей варьируется в предлах от 37 тыс.руб до 94.5 тыс.руб.
- Уровень образования является важным признаком для желаемого уровня заработной платы.
- Максимальны медианный уровень в Москве, как и колличество соискателей, минимальный в других городах.
- Перезды и командировки влияют на ожидания людей по увеличению ЗП. В среднем на 60% хотят получать больше.
- Мужчины желают получать приблизительно на 25-100% больше чем женщины.
- Удалённая работа имеет самый высокую границу по заработной плате.

:arrow_up:[к оглавлнию](https://github.com/Axewyl/Resume_analysis_from_HeadHunter/blob/master/README.md#Оглавлелние)