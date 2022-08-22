# Выявление параметров объявлений о продаже недвижимости, указывающих на вероятную мошенническую деятельность

[Ссылка на проект](https://nbviewer.org/github/anapon-DA/projects/blob/main/Defining%20Parameters%20for%20a%20Fraud%20Detection%20System/real%20estate%20online%20service%20and%20fraud%20detection.ipynb) :point_left:

В нашем распоряжении данные сервиса по продаже недвижимости — архив объявлений о продаже квартир в Санкт-Петербурге и соседних населённых пунктах за несколько лет. Нужно научиться определять рыночную стоимость объектов недвижимости. Необходимо установить параметры. Это позволит построить автоматизированную систему: она отследит аномалии и мошенническую деятельность.

Например, расстояние до центра, аэропорта, ближайшего парка и водоёма.

Предоставлены данные сервиса по продаже недвижимости — архив объявлений о продаже квартир в Санкт-Петербурге и соседних населённых пунктах за несколько лет:
- последняя стоимость в объявлении;
- расстояние до центра, аэропорта, ближайшего парка и водоёма;
- высота потолков, этажность дома, площадь;
- принадлежность к апартаментам;
- длительность размещения объявления на сайте;
- и др.



| [Рендер проекта на `nbviewer`](https://nbviewer.org/github/anapon-DA/projects/blob/main/Defining%20Parameters%20for%20a%20Fraud%20Detection%20System/real%20estate%20online%20service%20and%20fraud%20detection.ipynb) | [Проект на `github`](https://github.com/anapon-DA/projects/blob/main/Defining%20Parameters%20for%20a%20Fraud%20Detection%20System/real%20estate%20online%20service%20and%20fraud%20detection.ipynb) |
| --- | --- |
| **корректный переход по внутренним ссылкам в оглавлении проекта, отображаются интерактивные графические объекты Plotly** | статичный вариант |

# Выводы

В ходе исследоваемя были выявлены общие закономерности и тенденции, характерные для объявлений о продаже квартир:

- квартиры в Санкт-Петербурге дороже квартир в соседних населенных пунктах;
- в центре Санкт-Петербурга общая площадь квартир больше примерно на 20 кв.м, цена квартир выше почти на 50%, за квадратный метр - дороже на 10 000 руб. и более, среднее количество комнат больше на одну, потолки в среднем выше на 30 см;
- в центре сильнее прямая связь стоимости квартиры с высотой этажа и слабее обратная связь с удаленностью от центра города, слабее корреляция цены с числом комнат
- в центре города присутствуют сезонные "пики" зависимости цены от даты размещения - более дорогие квартиры, продающиеся в центре города, размещают в конце года и в начале лета;
- дороже всего стоят квартиры с 15 комнатами (несмотря на то, что есть квартиры с большим числом комнат)
- последний этаж - самый дорогой.

Отсутствие в объявлении выявленных закономерностей будет говорить о вероятных мошеннических действиях, особенно если имеется сразу несколько несоответствий.

# Статус проекта

:white_check_mark: Завершен

# Инструменты

`Matplotlib`
`Pandas`
`Python`
`Seaborn`