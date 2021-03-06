# Как настроить конверсии в конструкторе сайтов REG.RU
## regru-constructor-tracker
Конструктор REG.RU - JS скрипт для учета целей в Яндекс Метрике и Google Analytics

По состоянию на 19.05.19 инструмент создания сайтов предлагаемый REG.RU не поддерживает 
возможности добавления JS-событий для учета конверсий.

Эта оболочка была написана для расширения возможности конструктора. Т.к. он является неплохим
и достаточно качественным инструментом для быстрой проверки рекламных идей на низком бюджете.
Однако отсутствие возможности учета конверсий является серьезным недостатком.

Чтобы обойти этот недостаток был наспиан этот небольшой пример. Действующая версия была 
протестирована на сайте Zatochu.ru для оперативного развертывания рекламной кампании.

## Как настроить

1. Для начала вам необходимо привязать сайт к Яндекс Метрике и Google Analytics.
2. Добавьте в яндекс метрике цели-события 
3. В блоке #MAIN SETUP Укажите в константе YANDEX_COUNTER_ID ваш номер счетчика метрики и настройте GOALS_CURRENCY и GOALS_VALUE_* для учета ценности конверсий в Google Analytics
4. В блоке #LABELS Укажите в константах идентификаторы целей-событий из метрики
5. В блоке #ANCORS Укажите название анкоров ссылок и формы в конструкторе
6. Больше никаких изменений в коде не требуется, если вы не хотите добавлять большее количество целей
7. Установите готовый код в Настройки Сайта > Скрипты > Перед </body>
8. Проверьте ваши цели в инспекторе и в системах аналитики

## Спасибо за интерес!
Очень рассчитываю, что данный способ добавления конверсий утратит свою актуальность в ближайшее время и функционал будет добавлен в конструктор. Тем не менее, пока такая возможность отсутствует буду рад любым комментариям и предложениям.
