Если не открывается, используйте: https://nbviewer.jupyter.org/github/MikhailAleshin/Data-Analysis-Projects/blob/main/Прогнозирование%20оттока%20клиентов%20и%20кластеризация/Прогнозирование%20оттока%20клиентов.ipynb
# Описание работы
Нужно по предоставленным данным фитнес-клуба провести анализ средних значений признаков для тех, кто ушел, и тех, кто остался. Построить две модели бинарной классификации для предсказания 
оттока клиентов и, оценив метрики, выбрать наилучшую. Методами кластеризации выделить несколько групп клиентов 

# Инструменты
Pandas, matplotlib.pyplot, scipy, numpy, seaborn, sklearn,  Прогнозы и предсказания, Кластеризация.

# Вывод проекта
В исследовательском анализе мы увидели, что средние показатели лояльных и ушедших пользователей достаточно сильно отличаются (ушедшие менее активны). Заметили, что у многих ушедших контракт был всего на 1 месяц, и они не стали его продлевать.Очень мало пользователей берут долгий контракт и пропадают. После 5-6 месяцев лояльности посетители с большой долей вероятности не перестанут ходить. Средний возраст ушедних немного меньше с.в лояльных.
Мы обучили две модели 1) логическая регрессия 2) случайный лес. Логическая регрессия оказалась на валидационной выборке лучше по всем метрикам, поэтому я рекомендую ее для использования.
В работе приведена кластеризация посетителей на 5 кластеров. При их анализе мы увидели, что некоторые пользователи перестают ходить в силу удаленности фитнес-центра, у некоторых просто нехватает мотивации продлевать контракт

Возможно, получится уменьшить отток пользователей тем, что убрать месячные контракты. Да, покупателей станет меньше, однако после 5-6 месяц времени жизни пользователи становятся лояльными и уже вряд ли уйдут. Тем самым можно будет сильно уменьшить долю оттока. Можно попробовать изменения, повышающие интерес посетителей, однако это будет не так действенно.
