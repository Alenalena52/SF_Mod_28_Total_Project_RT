В рамках выполнения дипломного проекта требуется протестировать новый интерфейс авторизации в личном кабинете от заказчика Ростелеком Информационные Технологии.

Объект тестирования: https://b2c.passport.rt.ru

Заказчик передал следующее задание:

1. Протестировать требования.
2. Разработать тест-кейсы (не менее 15). Необходимо применить несколько техник тест-дизайна.
3. Провести автоматизированное тестирование продукта (не менее 15 автотестов). Заказчик ожидает по одному автотесту на каждый написанный тест-кейс. Оформите свой набор автотестов в GitHub.
4. Оформить описание обнаруженных дефектов. 

Требования по проекту: https://docs.google.com/document/d/1RRWhr_4bV_VTyNxr-lyDkJ3jaPVwXQFg/edit?usp=sharing&ouid=100674749469134479365&rtpof=true&sd=true

Тест-кейсы и баг-отчет: https://docs.google.com/spreadsheets/d/12JgyW8qOhoWak9BE-K6iTfrVC2ymedoj/edit#gid=999401712

Проведено ручное и автоматизированное тестирование

Для составления и написания тест-кейсов применены техники тест-дизайна: классы эквивалентности, анализ граничных значений, предугадывание ошибок.

В файле base_data.py находятся базовые классы, процедуры, функции и локаторы для автотестов

В файле settings.py - регистрационные данные для позитивных тестов авторизации

В файле test_SF_RT_passport.py - автотесты (номер автотеста совпадает с номером тест-кейса)

запуск автотестов (драйвер в одной папке с тест-скриптом)

python -m pytest -v --driver Chrome --driver-path chromedriver.exe test_SF_RT_passport.py
