# ГраФиС SVG
Набор векторных изображений в формате svg для использования в пожарной охране России. Векторные изображения основаны на представлении условных графических обозначений пожарной техники, оборудования и элементов пожарно-тактической обстановки используемых в [АИГС ГраФиС-Тактик](https://github.com/Obsidian-pb/GraFiS-Tactic).

Набор может использоваться как источник графических элементов в веб-представлениях боевых действий по тушению пожаров, а также в картографических проектах связанных с тематикой пожарной охраны России.

## Версия

0.7.0

# Используемые сокращения

 - **ПА** - Пожарный автомобиль
 - **УГО** - Условное графическое обозначение

Сокращения элементов боевых действий по тушению пожаров не используемые в данном тексте приведены в боевом уставе пожарной охраны России, если не указано иное.


# Правила оформления УГО

*версия 1.0*

- Все УГО оформляются в виде векторных изображений SVG
- Установлен базовый размер значка, с учетом толщины линий (`16px`). Данный размер учитывается как: ширина УГО пожарных автомобилей, ширина и высота УГО водоисточников
- Поле УГО должно охватывать изображение по вертикали и горизонтали. Пустые поля выступающие за пределы изображения не допускаются
- В цветовой гамме УГО используются следующие основные цвета:
    - красный: `#FF0000` или `red`
    - белый: `#FFFFFF` или `white`
    - черный: `#000000` или `black`
    - синий: `#0000FF` или `blue`
- В цветовой гамме УГО могут использоваться следующие дополнительные цвета:
    - зеленый: `#008000` или `green`
    - серый: `#808080` или `gray`
- В геометрии УГО используются только теги `path`. Однако, их может быть несколько
- Каждое SVG должно быть снабжено тегом `id`, содержащим наименование УГО идентичное имени файла без расширения
- Имена УГО пишутся латиницей. Используются только строчные буквы
- Имена УГО могут сопровождаться следующими суффиксами:
    - `*_alt(n)`: для УГО имеющих одно и то же значение, но разный внешний вид. При этом `(n)` заменяется номер варианта обозначения
    - `*_v(n)`: для УГО отражающих один и тот же элемент обстановки, но в различных состояниях. Например, пожарные стволы с различным типом струи. При этом `(n)` заменяется уточнением состояния элемента
    - `*_bad`: для УГО находящихся в неисправном или неработоспособном состоянии
    - `*_uncolor`: для фигур с возможностью менять цвета непосредственно в пользовательских решениях
- Суффиксы имен УГО могут сочетаться при этом порядок суффиксов в имени должен быть такой же как они перечислены выше
- В УГО не могут использоваться надписи выполненные шрифтом. Все надписи являющиеся частью УГО должны выполняться при помощи тега `path`
- Основной размер букв в векторных шрифтах фигур `6px х 4px`
- В УГО используются следующие толщины линий:
    - `2px`: основные контуры УГО
    - `1.5px`: дополнительные контуры УГО
    - `1px`: надписи и второстепенные контуры


# Полезные ссылки:

* Набор векторных иконок [maki](https://github.com/mapbox/maki) идеями которого вдохновлялся автор