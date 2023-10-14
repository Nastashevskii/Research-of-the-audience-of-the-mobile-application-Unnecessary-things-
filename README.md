# Research-of-the-audience-of-the-mobile-application-Unnecessary-things-
В приложении «Ненужные вещи» пользователи продают свои ненужные вещи, размещая их на доске объявлений. Необходимо провести исследование аудитории сервиса по логам пользовательских событий в приложении, совершенных после 07.10.2019.

Цель исследования - на основе сегментации пользователей (заданной и выделенной самостоятельно) получить гипотезы о том как можно было бы улучшить приложение с точки зрения клиентского опыта. Заданная сегментация пользователей - по источникам скачиванaия приложения.

Задачи исследования:

 - Выделить сегменты пользователей для создния второй пары тестируемых групп.
 - Исследовать, какие пользователи склонны чаще возвращаться в мобильное приложение.
 - Исследовать, какие пользователи чаще совершают целевое событие (конверсия в целевое действие).
 - Определить, как различается время между распространенными событиями пользователей из разных групп.
 - Подготовить презентацию с результатами исследования.

Описание данных:

Датасет содержит данные о событиях, совершенных в мобильном приложении "Ненужные вещи". В нем пользователи продают свои ненужные вещи, размещая их на доске объявлений.

В датасете содержатся данные пользователей, впервые совершивших действия в приложении после 7 октября 2019 года.

Датасет mobile_dataset.csv содержит колонки: 

 - event.time — время совершения 
 - event.name — название события user.id — идентификатор пользователя

Датасет mobile_sources.csv содержит колонки:

 - userId — идентификатор пользователя
 - source — источник, с которого пользователь установил приложение
 
Расшифровки событий:

 - advert_open — открытие карточки объявления
 - photos_show — просмотр фотографий в объявлении
 - tips_show — пользователь увидел рекомендованные объявления
 - tips_click — пользователь кликнул по рекомендованному объявлению
 - contacts_show и show_contacts — пользователь нажал на кнопку "посмотреть номер телефона" на карточке объявления
 - contacts_call — пользователь позвонил по номеру телефона на карточке объявления
 - map — пользователь открыл карту размещенных объявлений
 - search_1 — search_7 — разные события, связанные с поиском по сайту
 - favorites_add — добавление объявления в избранное

# Выполнены задачи исследования:

Выделены сегменты пользователей для создния второй пары тестируемых групп. В данном случае были созданы две группы пользователей: пользователи, добавившие объявления в избранное, и пользователи, не добавившие объявления в избранное

Исследовали, какие пользователи склонны чаще возвращаться в мобильное приложение. Пользователи группы google и пользователи с короткими сессиями чаще возвращаются в приложение

Исследовали, какие пользователи чаще совершают целевое событие (конверсия в целевое действие). Среди пар сравниваемых групп конверсия находится примерно на одном уровне: среди групп yandex и google конверсия равна 25,28% против 24,11%
Определены, как различается время между распространенными событиями пользователей из разных групп. Среди пользователей групп google и yandex время, проводимое в приложении, практически не отличается: 10:12 против 10:43

Исходя из результатов статистической проверки гипотез, можно сделать вывод, что:

Нет статистически значимых различий в конверсии в просмотры контактов между пользователями, пришедшими с источника Yandex и Google. Это означает, что нет достаточных доказательств для того, чтобы утверждать, что одна группа пользователей имеет значительно выше или ниже конверсию в просмотры контактов по сравнению с другой группой.

Нет статистически значимых различий в конверсии пользователей, добавивших объявления в избранное, и пользователей, не добавивших объявления в избранное. Это говорит о том, что пользователи, добавившие объявления в избранное, не имеют отличающуюся конверсию в просмотры контактов от пользователей, не добавивших объявления в избранное.

Общие рекомендации:
Для повышения конверсии в целевое действие среди пользователей группы Yandex необходимо улучшить их удержание, а для группы Google стоит сосредоточиться на возможности повышения активности пользователей.

Для увеличения конверсии среди групп с короткими сессиями необходимо улучшить их удержание и сосредоточиться на возможности повышения активности пользователей, а для улучшения конверссии среди пользователей с длинными сессиями необходимо повышать их удержание
