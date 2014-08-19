# Приступая к работе

## Редакции «Центра охраны»

Программное обеспечение «Андромеда Центр охраны» поставляется в различных редакциях. 

### А100 и А600

Это редакции «Центра охраны», предназначенные специально для эксплуатации совместно с пультами централизованного наблюдения производства компании «Альтоника». В составе редакций «А100» и «А600» допускается использование только тех источников событий, которые предназначены для приема извещений от этих пультов. При заказе «Центра охраны» редакции «А100» или «А600» необходимо указать количество источников событий от «Lonta-202» или «RS-200» — оно должно соответствовать количеству пультов, которые предполагается подключить к «Центру охраны».

Между собой редакции отличаются максимальным возможным количеством обслуживаемых объектов: не более 100 охраняемых объектов допускает редакция «А100» и не более 600 объектов — редакция «А600».

Если в процессе эксплуатации «Центра охраны» редакции «А100» или «А600» потребуется подключить другой пульт централизованного наблюдения, либо количество обслуживаемых объектов превысит 600, то необходимо обновить редакцию «Центра охраны» до одной из стандартных.

### Стандартные редакции

Стандартные редакции программного обеспечения «Центр охраны» отличаются максимально возможным количеством обслуживаемых объектов: 250, 500, 750, 1000, 1500, 2000 и так далее.

Ограничений на использование источников событий нет, при этом источники событий от пультов централизованного наблюдения третьих фирм приобретаются отдельно.

## Назначение модулей

Программное обеспечение «Андромеда Центр охраны» состоит из модулей, каждый из которых предназначен для решения конкретных задач.

Модуль «**Менеджер событий**» служит для приема извещений от приемного оборудования центральной станции, а также напрямую от некоторых видов объектового оборудования, например, по каналам связи GPRS и Ethernet. 

Кроме того, именно в модуле «Менеджер событий» происходит автоматизированной обработка событий: контроль цепочек событий, отправка SMS-сообщений и передача событий в другие системы. 
Необходимо отметить, что «Менеджер событий» является связующим звеном для всех остальных модулей «Центра охраны»: он должен быть запущен первым, так как именно с его помощью модули обмениваются информацией о новых событиях, действиях операторов и других изменениях, произошедших при работе модулей.

С помощью модуля «**Менеджер объектов**» осуществляется создание новых объектов и изменение описания для существующих объектов.

Модуль «**Дежурный оператор**» используется оператором для обработки событий. Основные функции модуля — наблюдение за оперативным состоянием объектов, просмотр последних полученных событий, регистрация действий оператора по отработке тревог, полученных от объектов.

Назначение модуля «**Карты объектов**» - создание схем подъезда к объекту, поэтажных планов и расположения рубежей охраны. Кроме того, модуль «Карты объектов» используется для отображения тревожных шлейфов объекта на поэтажном плане при отработке тревоги.

Список операторов «Центра охраны», а также их прав в каждом из модулей устанавливаются в «**Менеджере персонала**». В этом же модуле можно изменить список групп реагирования, а также список компьютеров локальной сети, на которых эксплуатируются сетевые рабочие места «Центра охраны».

Модуль «**Мастер базы данных**» предназначен для выполнения следующих операций:

* проверка базы данных и устранение ошибок
* создание резервной копии базы данных
* восстановление базы данных из резервной копии
* импорт данных из базы данных программного обеспечения «Андромеда», программного обеспечения «Андромеда Либерти», программного обеспечения «Страж» и программного обеспечения «CSM32»
* экспорт данных из базы данных «Центра охраны» для использования в других программах

В модуле «**Настройка системы**» можно изменить справочники, которые используются при описании объектов: список шаблонов событий, классы событий и связанные с ними действия, типы объектов и список дополнительных характеристик.

## Первый запуск

Для того чтобы приступить к работе нужно запустить модуль «Менеджер событий» и настроить источники событий — специальные компоненты модуля, предназначенные для приема событий от оборудования центральной станции.

Настройка источников событий осуществляется в окне «Источники событий». Для доступа к нему нужно выбрать пункт «Источники событий...» в меню модуля «Менеджер событий» (щёлкнуть правой кнопкой мыши на иконке в системной области панели задач).

Если «Центр охраны» установлен для ознакомительных целей, то для создания событий от объектов можно воспользоваться пунктом «Эмуляция событий...» в меню «Менеджера событий».

После того, как модуль «Менеджер событий» запущен, можно приступить к работе с другими модулями. Заводить объекты в систему следует с помощью модуля «Менеджер объектов», а наблюдать за принимаемыми событиями и отрабатывать тревоги — используя модуль «Дежурный оператор».

## Пароль администратора
Непосредственно после установки программного обеспечения «Центр охраны» в списке операторов присутствует только один оператор – «Администратор». Пароль оператора «Администратор» по умолчанию – **222222**.

## Импорт данных 

В программном обеспечении «Андромеда Центр охраны» реализована функция импорта информации об объектах из баз данных следующих программ:

* «Андромеда» версий 2.0 — 2.76
* «Андромеда Либерти»
* «Страж»
* «CSM32»

Если до «Центра охраны» использовалось программное обеспечение из списка, приведенного выше, то для комфортного перехода на применение «Центра охраны» можно выполнить импорт описаний объектов из базы данных этих программ.

Если предполагается импорт данных из программного обеспечения «Андромеда» версий 2.0 — 2.76 или «Андромеда Либерти», то при установке «Центра охраны» нужно указать необходимость установки BDE — именно эта подсистема используется для доступа к данным этих программ.

Импорт данных осуществляется с помощью модуля «Мастер базы данных». В случае импорта данных программного обеспечения «Андромеда» версий 2.0 — 2.76 или «Андромеда Либерти», для его выполнения потребуются все файлы из папки базы данных. При наличии резервной копии базы данных в формате ZIP, необходимо извлечь файлы из архива в любую папку на жестком диске компьютера.
