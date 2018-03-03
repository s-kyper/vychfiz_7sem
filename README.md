# vychfiz_7sem
Задание:
Создать модель взаимодействия заряженных частиц в сфере, рассматривая их энергии с помощью метода Монте-Карло.
Ход работы:
	Задаем радиус сферы R, количество частиц N, радиус частиц r. Заряды q = 1.
	 Энергию частицы E_i считаем по формуле E_i=∑_(j=1)^n▒E_ij , где E_ij=  1/r_ij  , 
r_(ij ) - расстояние между частицами c соответствующими индексами

	На каждом шаге перебираем все частицы p_i и находим ее новые координаты с помощью метода Монте-Карло. Смещаем частицу p_i в произвольном направлении на какое-то расстояние ε < δ (δ задано). Если разница начальной и конечной энергий частицы p_i больше 0, то возвращаем в точку с исходными координатами и повторяем действие до получения требуемого результата, иначе оставляем частицу p_i в точке с данными координатами, иначе. Проверяем, лежат ли новые координаты частицы p_i внутри сферы.
Результат: 
Все частицы лежат на сфере.
