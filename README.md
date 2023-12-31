# Анализ продаж

**Использованные данные не имеют отношения к реальности**

## Логика и последовательность выполнения

Сначала, я выгрузил данные по планам продаж и выручке и их фактическим значением "Бухгалтерии.Контур" из базы данных в pandas датафрейм. Далее, посчитал абсолютное и относительное отклонение. На основе этих данных построил погодовой и помесячный план-факт график.

После этого, я перешел к анализу тарифов. Выгрузил по ним данные и сгруппировал по названию (Лайт, Базовый,...) и сроку подписки. По данным построил графики динамики продаж и выручки конкретных тарифов, а так же круговые диаграммы распределения продаж по тарифам за каждый год, чтобы посмотреть на возможное изменение спроса клиентов.

Далее, посмотрел соотношения новых и старых клиентов в течении лет, чтобы проверить успешность привлечения новой аудитории. Посмотрел, на выбор тарифа новых клиентов.

Заметив ранее, что в 2018 продажи упали после роста в предыдущих годах, поискал в интернете внешнеэкономические причины, которые могли бы повлиять на это. Так же, проверил общую тенденцию продаж по всем продуктам Контура и провер гипотезу о переходе клиентов с "Бухгалтерии.Контур" на другой аналогичный продукт контура.

В конце, решил посмотреть на структуру клиентов "Бухгалтерии.Контур": посмотрел на оборот и количество сотрудников компаний, использующих данный продукт и проверил есть ли зависимисть между выбором тарифа и этими показателями. Так же, посмотрел по этим данным размер бизнесов, покупающих "Бухгалтерию" и соответствие этого целевой аудитории продукта. 

![16116d1ef7f041741cea9da7e13c7268d528a3d3](https://github.com/seoful/sales-analysis/assets/34482712/31438b44-055b-4ea7-a1c6-57349de98b2c)

![92bd03b82141303776785107b5aee6f925839fe3](https://github.com/seoful/sales-analysis/assets/34482712/9721bee6-18f9-400e-9a09-9707aa2005b3)

![25c9c76f97eb382f8d2caf2ac5bcb7a03617b7cf](https://github.com/seoful/sales-analysis/assets/34482712/ed89cb16-cd9b-4d31-8c79-7ea3e1a3eb77)

![e916997a2a53c8b2668250a99a8aa7af9276251a](https://github.com/seoful/sales-analysis/assets/34482712/4667052f-93b6-4f0c-a19b-a305fd0bd256)

![7c403fe4ea50c97e6fabe6a53058be599a2e7c67](https://github.com/seoful/sales-analysis/assets/34482712/647baae2-192e-4fe4-bcef-24115cb6a20a)

![ee4926c113991f9696356590914100dc58d2c56a](https://github.com/seoful/sales-analysis/assets/34482712/1cc6cc7d-77c9-4bcd-a830-85971aa97c3c)

![78495cdd4f76fd112ed94900311a7223f983c28b](https://github.com/seoful/sales-analysis/assets/34482712/5991becc-2401-4db3-b31e-569e6fe57dcd)

![eb946dade1889ffd94c84dc16861a9be9d250dc0](https://github.com/seoful/sales-analysis/assets/34482712/b5d1c95a-47b9-4253-b504-196df65e6d56)

![665128710c9995546de1800fb11afe54f0bbadb0](https://github.com/seoful/sales-analysis/assets/34482712/a5077310-558c-4968-bb5f-943416774a73)

![d9901badf91276b78765b9895aa24918288d7ff1](https://github.com/seoful/sales-analysis/assets/34482712/f43c7e06-2a99-43d2-b9d7-39ce5629445e)

![50b73dcba78076c4001615079b7ee51f53a58d85](https://github.com/seoful/sales-analysis/assets/34482712/37389fa7-e7cd-4609-a788-a5163838ece8)

![77c3a105930c8f1d27163dbb093e1e084df80ad0](https://github.com/seoful/sales-analysis/assets/34482712/e2b59eef-5e1d-4b9d-a089-b7d800d4b752)

![7a14fe825aa32cb70553bc490bee9add61ca5f2f](https://github.com/seoful/sales-analysis/assets/34482712/4640b136-90f8-421f-b767-49b27ba71a88)

![31c4677072a7929086c9dc5d745f460ac99ac910](https://github.com/seoful/sales-analysis/assets/34482712/03c57f2a-cb7b-4276-8147-7102065b8303)

![86eb3a9e75accb2d6709664e816c56a64aa97e42](https://github.com/seoful/sales-analysis/assets/34482712/39cd580a-a8c4-40da-8bd8-66bcdb477595)

![42ed0aa8f7aff465f0c45d98daf2a5c6edf8c595](https://github.com/seoful/sales-analysis/assets/34482712/6f1db756-5395-4ee3-bb95-52e3f63013fe)

## Анализ

По графику план-факта продаж и выручки видно, что в годовых разрезах план за 2015-2018 года выполняется и даже перевыполняется. В помесячном же разрезе, в некоторые месяцы план немного недовыполнен, однако таких месяцев мало.

Из динамики продаж и выручки по продукту "Бухгалтерия.Контур" выдно, что продажи в 2018 году пошли на спад в сравнении с предыдущими годами, в которые они показывали рост. Посмотрев на динамику экономики РФ в Википедии, видно, что в 2015-2018 годах показатели ВВП росли, а темпы роста увеличивались. Из основных экономических потрясений в стране за 2018 год можно выделить пенсионную реформу, повышение НДС до 20%, санкции и повышение цен на бензин. Эти критерии не имеют прямого влияния на продукты Контура, кроме разве что санкций. Однако, они были направлены в основном на госкредиты, некоторый экспорт и военно-промышленный комплекс, что не должно было особо сказаться на целевой аудитории продукта. Теория о переходе клиентов с Бухгалтерии.Контур на другие аналогичные продукты Контура неверна, так как спад продаж заметен по всем продуктам компании кроме Экстерна, которая не заменяет бухгалтерские продукты. Можно, сделать вывод, что спад продаж и соответственно выручки в 2018 году был системным по всей продукции контура в том числе и анализируемой "Контур.Бухгалтерии", причинами которой вероятнее всего являются внутренние бизнес-решения компании, чем внешнеэкономические факторы. Смотря на план продаж, можно сделать вывод, что уменьшение продаж в 2018 году было спрогнозировано заранее и об этом было известно руководству.

У Контур.Бухгалтерии есть 4 группы тарифов (Лайт, базовый, максимальный, ТД). ТД является бесплатным тарифом (возможно, промо или пробный тариф), но на него выпадает ~1% продаж. Так что, сконцентрируемся на других трёх тарифах. Продукт можно купить на 6, 12, 18 или 24 месяца.
Самым популярным тарифом по продажам и выручке является Лайт (~82% продаж). Далее, Базовый с ~13% и оставшиеся 3-4% занимает максимальный тариф. Рассматривая продажи по длительности доступа к продукту лидирует самый длинный срок (2 года). Далее процент продаж выстроился по убыванию длительности срока. Можно сделать вывод, что ценовая политика построена грамотно и клиенты склонны выбирать более долгое сотрудничество с компанией и использование продукта. 

В графике продаж и выручки по тарифам и сроку доступа к продукту во всех категориях статистики двигаются в соответствии с глобальным трендом: увеличение в 2015-2017 и спад в 2018 годах. Структура продаж и выручки по срезам при этом из года в год сохраняется с преобладанием тарифа Лайт и выбором более длительных сроков.

Проанализировав клиентскую базу Бухгалтерии.Контур видно, что количество новых клиентов уменьшается, а рост старых клиентов, продолжающих использовать продукт уменьшается, что при сохранении такой тенденции может привести к уменьшению выручки или даже убыточности продукта.

Структура выбора тарифов и длительности тарифов среди новых клиентов (первой покупки) соответствует глобальной структуре по всем продажам и так же не меняется с течением лет.

На последних графиках, показывающих оборот и количество персонала среди клиентов Контур.Бухгалтерии агрегированных по тарифам видно, что основная аудитория продукта это микро и малый бизнес, что соответсвует целевой аудитории. Однако, средний и крупный бизнес тоже использует продукт, но в гораздо меньших масштабах. Также, видно, что выбор тарифа не зависит от размера компании и ее экономических показателей.

## Предложения по целям на будущее время
- Стимулировать покупку более продвинутых и соответственно дорогих тарифных планов, чтобы сместиться с многократного преоблодания тарифа "Лайт". (Пересмотр цен более продвинутых тарифов, стимулировать желание клиентов воспольоваться фичами более дорогих тарифов)
- Поддерживать клиентов оставаться с Контуром на более долгий срок и продлевать подписку на продукт. (Скидки за продолжение сотрудничества, добавление нового функционала, добавление функционала, присутствующего у конкурентов, привязка клиентов к инфраструктуре Контура)
- Увеличить количество новой аудитории продукта. (Реклама, специальные и промо-предложения, пробные тарифы, разработка нового привлекающего функционала).
- Вернуться по показателям продаж до уровня 2017 года.

# Прогноз
## Логика и последовательность выполнения'

Сначала я использовал ARIMA модель. Однако, ее было сложно затюнить на реальные данные и метрики были плохими. После этого, я решил попробовать autoARIMA, которая по сути является grid search-ем над ARIMA. Мне всё равно не понравился результат выдающийся данным методом, и для решения здачи прогнозирования я использовал библиотеку prophet от Meta. 

![0ad07784bcf21721f640c757b37f2b29157dfb11](https://github.com/seoful/sales-analysis/assets/34482712/687944c0-be9d-4cb3-adfb-4bc08ea431a9)

![227388bd87b68510a965dabf4ea56e4a869a8a9d](https://github.com/seoful/sales-analysis/assets/34482712/e7e0bfa3-c9fb-4a82-a3be-7f668c602e8e)

## Выводы

По пронозу prophet, Контур.Бухгалтерию ждёт последующий спад продаж при сохранении текущей политики (маркетинговой, ценовой...) компании. Однако, как и в прошлые годы, будет рост продаж в начале года и в мае.
