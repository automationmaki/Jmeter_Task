План по нагрузочному тестированию находится в файле casexe_summary_ivan.jmx (Желательно открывать при помощи Jmeter 5.1.1). Отчет формируется в файле summary.csv
Вначале запускается setUp Thread group, которая выполняет роль смоук теста. Если на смоук-тесте возникает ошибка, то весь план нагрузочного тестирования приостанавливается. Все тесты вынесены в отдельный тест-фрагмент. Так же подключен backend listener для подключения к базе InfuxDb и дальнейшей визуализации в Grafana или Chronograf. 
