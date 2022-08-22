# Индивидуальный проект по анализу данных
## Описание данных
Данные связаны с прямыми маркетинговыми кампаниями португальского банковского учреждения. Маркетинговые кампании основывались на телефонных звонках. Часто требовалось более одного контакта с одним и тем же клиентом, чтобы получить доступ к тому, будет ли продукт (банковский срочный депозит) подписан ("yes") или нет ("no").
## Входные переменные:
### Данные клиента банка:
1. **age**: (числовой)
2. **job**: тип работы (категориальный)
3. **marital**: (категориальный: 'divorced','married','single','unknown')
4. **education** (категориальный: 'basic.4y', 'basic.6y', 'basic.9y', 'high.school', 'illiterate', 'professional.course', 'university.degree', 'unknown')
5. **default**: имеет ли кредит по умолчанию? (категориальный: 'no','yes','unknown')
6. **housing**: есть ли жилищный кредит? (категориальный: 'no','yes','unknown')
7. **loan**: есть ли личный кредит? (категориальный: 'no','yes','unknown')
### Данные связанные с последним контактом текущей кампании:
8. **contact**: тип контактной связи (категориальный: 'cellular','telephone')
9. **month**: последний месяц контакта в году (категориальный: 'jan', 'feb', 'mar', ..., 'nov', 'dec')
10. **day_of_week**: последний контактный день недели (категориальный: 'mon','tue','wed','thu','fri')
11. **duration**: продолжительность последнего контакта в секундах (числовой). Важное примечание: этот атрибут сильно влияет на выходную цель (например, если длительность=0, то y= "no"). Тем не менее, продолжительность не известна до выполнения вызова. Кроме того, после окончания вызова y, очевидно, известен. Таким образом, эти входные данные должны включаться только для целей сравнения и должны быть отброшены, если намерение состоит в том, чтобы иметь реалистичную прогностическую модель. ### Другие атрибуты:
12. **campaign**: количество контактов, выполненных в ходе этой кампании и для данного клиента (числовой - включает последний контакт)
13. **pdays**: количество дней, прошедших после того, как с клиентом в последний раз связывались из предыдущей кампании (числовой; 999 означает, что с клиентом ранее не связывались)
14. **previous**: количество контактов, выполненных до этой кампании и для этого клиента (числовой)
15. **poutcome**: результат предыдущей маркетинговой кампании (категориальный: 'failure','nonexistent','success') 
### Атрибуты социального и экономического контекста
16. **emp.var.rate**: коэффициент вариации занятости - квартальный показатель (числовой)
17. **cons.price.idx**: индекс потребительских цен - месячный показатель (числовой)
18. **cons.conf.idx**: индекс потребительского доверия - месячный показатель (числовой)
19. **euribor3m**: курс euribor 3 месяца - дневной индикатор (числовой)
20. **nr.employed**: численность работников - квартальный показатель (числовой)
### Целевой признак:
21. **y** - подписался ли клиент на срочный депозит? (двоичный: 'yes','no')
