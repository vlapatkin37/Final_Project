# Связь Долгого Мира и Ценностей Самовыражения
Весь текст и код проекта находится в файле data_science_final_project.ipynb
## Компоненты кода

1) Получение данных с сайтов, в том числе веб-скреппинг с помощью beautifulsoup
2) Обработка данных припомощи Pandas
3) Математические возможности, включая numpy
4) Работа с геоданными
5) Визулизация полученных данных
6) SQL
7) Построение регрессий
8) Необсуждавшиеся в ходе курса библиотеки, используемые, например, для чтения PDF файлов

## Предпосылки проекта
В моём проекте я хотел бы связать между собой две социологические концепции: феномен Долгого Мира и классификацию Систем Ценностей Инглхарта. Давайте для начала разберёмся, что каждая из них из себя представляет.

### 1. Карта Ценностей Инглхарта

Классификация систем ценностей Рональда Инглхарта включает две основные шкалы: "выживание - самовыражение" и "традиционные - секулярные рациональные" ценности. Эти шкалы используются для описания культурных различий между странами и региональными группами.

#### Ось "Выживание - Самовыражение"
##### Ценности выживания
Ценности выживания характерны для обществ, где преобладают экономическая нестабильность и опасности. В таких обществах люди больше озабочены физической и экономической безопасностью. Основные черты:

* Упор на экономическую и физическую безопасность
* Приоритет национальной безопасности и сильного государства
* Низкий уровень доверия к другим людям
* Приоритет национальной безопасности и сильного государства
* Ограниченная социальная и политическая активность

Низкая толерантность к различиям (например, этническим или культурным)
Строгое соблюдение социальных норм и традиций

##### Ценности самовыражения
Ценности самовыражения преобладают в обществах с высоким уровнем экономической стабильности и безопасности. Здесь акцент делается на личную свободу, качество жизни и самореализацию. Основные черты:

* Высокий уровень межличностного доверия
* Активное участие в политической жизни
* Упор на экологическую устойчивость и защиту прав человека
* Высокая толерантность к различиям и культурное разнообразие
* Значимость самовыражения и творчества
* Поддержка гендерного равенства и индивидуальных свобод

#### Ось "Традиционные - Секулярные Рациональные"
##### Традиционные ценности
Традиционные ценности распространены в обществах, где сильна роль религии, семьи и коллективных норм. Основные черты:

* Высокая значимость религии и религиозных практик
* Упор на семейные ценности и традиционные гендерные роли
* Почтение к авторитетам и соблюдение традиций
* Патриотизм и национальная гордость
* Негативное отношение к разводам, абортам и эвтаназии

##### Секулярные рациональные ценности
Секулярные рациональные ценности преобладают в более модернизированных обществах, где религия и традиционные нормы играют меньшую роль. Основные черты:

* Низкая значимость религии и религиозных практик
* Высокая значимость науки и рациональности
* Секуляризация общества и снижение роли религиозных институтов
* Высокая терпимость к различным формам семьи и брака
* Признание прав индивидуума и личной свободы

Посмотреть карту за 2023 год можно будет по ссылке:
https://www.worldvaluessurvey.org/images/Map2023NEW.png

В этом проекте нам интересна будет первая ось.

### 2. Долгий Мир

Концепция "Долгого Мира" относится к периоду после Второй мировой войны, характеризующемуся снижением крупных межгосударственных конфликтов, особенно между либеральными демократиями. Страны стали реже вступать в войны друг с другом благодаря внутренним политическим механизмам, общественному мнению и экономической взаимозависимости.

Предположение проекта заключается в том, что ценности самовыражения не были распространены периода долгого мира и преобладали ценности выживания. Далее, после того как война перестала быть значимой угрозой для человека, он стал думать о чём то нематериальном и ценности переформировались.

При этом разные страны с разной скоростью и на разном этапе развития вошли в кондицию "Долгого Мира" и потому и располагаются на разных координатах по оси "Выживание - Самовыражение".

### Гипотеза:

Степень применимости концепции "Долгого Мира" к стране (которая характеризуется отсутствием военных конфликтов на её территории и степенью развития демокртических институтов) является основным фактором формирования ценности самовыражения.

## Результаты проекта
1) Были получены нужные данные с 5 сайтов
2) Были посчитаны индексы Самовыражения и Долгого Мира ![](self_expression_bar_chart.png) ![](long_peace_bar_chart.png)
3) Предварительные данные прошли проверку на соответсвие нормальному распределению ![](normal_distribution.png)
4) Были посчитаны коэффициенты корреляции и p-value для двух показателей двумя разными способами
5) Был проведёт регрессионный анализ ![](regression.png)
6) Гипотиза подтвердилась
