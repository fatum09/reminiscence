# reminiscence
This repository is dedicated to processing data on a study devoted to the very first memories of people speaking Russian.

Этот репозиторий посвящен обработке данных первых воспоминаний людей. Пока основным языком является русский.

Обычно респонденты отвечали на два вопроса: «Каково ваше первое воспоминание? К какому возрасту оно относится?». По возможности фиксировалось имя и пол отвечающего. Сбор ответов осуществлялся через социальные сети (vk, twitter) в форме диалога в личных сообщениях, а также анонимного опроса в [Google-форме](https://docs.google.com/forms/d/1VgxUitSX7CZqr1RTlymFTjglAZjS_AT36cbRVX-EPXA/) ([англоязычная версия формы](https://docs.google.com/forms/d/e/1FAIpQLSfPgOvrBsthWRVqycJf6SOGhsnSP6w2hR5cn65lf50xbose9w/viewform?usp=sf_link)). Часть воспоминаний была прислана на e-mail в результате распространения исследования. Ответы продолжают приниматься, поэтому если вы случайно натолкнулись на этот опрос – перед исследованием ответов заполните форму.

На декабрь 2019 г. собрано 643 ответа. Набор данных в текущем состоянии представлен в виде [электронной таблицы Google Drive](https://docs.google.com/spreadsheets/d/1KSirtO9hZSmVst--GiqsBPYk6hX-xOCI-SolgiafjcI/edit?usp=sharing). Также время от времени делается бэкап в файл [Reminiscence-backup.xlsx](https://github.com/matyushkin/reminiscence/blob/master/Reminiscence-backup.xlsx).

Описание полей набора данных:
- **№** – номер записи; одна запись может содержать несколько воспоминаний, обычно они отделяются друг от друга одной пустой строкой
- **Имя** – имя респондента (данное в ответе или обозначенное в профиле)
- **Name** – перевод имени на английский язык
- **Воспоминание** – текст ответа на русском языке (если это язык оригинального ответа); если в одной записи воспоминаний несколько, тексты отдельных воспоминаний разделены по возможности пустой строкой
- **Translation** – перевод текста ответа (частично воспоминания переведены на английский язык)
- **Translation footnote** – комментарий к переводу текста воспоминания для сносок
- **Пол** – пол респондента (если известен или понятен из текста)
- **Кол-во** – количество воспоминаний, содержащихся в ответе
- **Возраст** – возраст (возраста) воспоминаний, данный отвечающим, указывается в годах, в случае месяца указывается доля месяца. Если для разных воспоминаний указан разный возраст, перечисляются через точку с запятой. Также приводятся интервалы времени и случаи больше/меньше («не раньше двух лет», «после года»)
- **Ориентир возраста** – указатель возраста в воспоминании или подтверждение возраста лицом из воспоминания, например, родственником. В случае если возраст не указан, может служить как уточняющий маркер (неумение ходить, неумение говорить)
- **Мотив** – категория воспоминания, своеобразные тэги для разделения воспоминаний на группы, описывают происходящую ситуацию
- **Лица** – упомянутые отвечающим одушевленные сущности (люди и животные) 
- **Предметы** – упомянутые отвечающим предметы
- **Цвета** – встречающиеся в тексте воспоминания категории цвета (за исключением имен персонажей, например, Красная шапочка)
- **Звуки** — упомянутые или определенные из текста воспоминания звуки
- **Запахи, вкус**
- **Другие ощущения/действия** (тепло, темнота, объятия и т.д.)
- **Сущности** – наиболее субъективное поле, описывающее не объекты и ощущения напрямую, а процессы и ситуации (близко к комментарии)
- **Пространство** – место действия одного или нескольких воспоминаний, упомянутое или определенное из текста воспоминания. В скобках указывается более крупная категория пространство по отношению к описанной, например: «диван (помещение)»
- **Время дня**, упомянутое, реже – определенное из текста воспоминания. Если время дня можно предположить, но на это нет явных указаний, после времени дня идет знак «(?)», также используется союз «или»
- **Время года**, упомянутое, реже – определенное из текста воспоминания. Использование знак «(?)» аналогично пункту время дня
- **Поведение** – «активное» в случае совершения активных действий рассказчиком, пассивное – если все действия совершаются лишь по отношению к рассказчику, нет явного проявления какого-либо активного действия
- **Комментарий** – замечание исследователя «на полях»

Планируется оформить результаты исследования в виде публикации на Medium, в pdf (с помощью LaTeX) и в других форматах, удобных для книжного чтения: epub, fb2. Публикация будет состоять из двух частей: 1) исследование со ссылками на конкретные воспоминания, 2) сами воспоминания.

Набор данных также планируется опубликовать отдельно на Kaggle. Датасет может представлять пользу не только как набор воспоминаний, но и для различных задач обработки текстов на естественных языках: это и переводы с русского на английский язык, и одновременно набор микротекстов, из которых выделены одушевленные сущности, предметы, запахи и пр.

Предыдущие результаты исследования описаны в [текущей pdf-версии](https://github.com/matyushkin/reminiscence/blob/master/Pervye_vospominaniya_Leva_Matyushkin.pdf).

Русскоязычные страницы проекта в социальных сетях:
[twitter](https://twitter.com/memories_ru), [telegram](t.me/memories_ru), [facebook](https://facebook.com/firstmemoriesru), [vk](https://vk.com/first_memories).

Social networks pages for Engilsh speakers: [twitter](https://twitter.com/en_memories), [telegram](t.me/memories_en), [facebook](https://facebook.com/firstmemoriesen), [vk](https://vk.com/first_memories_en).