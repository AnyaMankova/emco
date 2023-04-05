# emco
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=%white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

Представлен датасет, отражающий работу самосвалов за 11 месяцев 2022 года со следующими данными: 
- дата смены
- самосвал
- средний вес в кузове автомобиля БелаЗ 75306 (г.п. 220т) за смену
- пройденное расстояние суммарно за смену
- средняя скорость за смену
- стандартное отклонение перепада высот за смену
- потраченный объем топлива за смену

Поставленные задачи: 
- выявить взаимосвязь технологических параметров (взаимное влияние и влияние на расход топлива);
- дать предложение по диапазонам параметров, при которых расход топлива минимальный (при этом нет ухудшения скорости (снижения), вес в кузове не менее 220 т., ср. перепад высот и пройденное расстояние - без существенных изменений, поскольку параметры нерегулируемые)


<p>#Проведен первичный анализ данных (EDA).

Команда df.describe() генерирует описательную статистику для всех числовых столбцов: число непропущенных значений, среднее, стандартное отклонение, минимум, 25 и 75 процентили, медиану и максимум. 
![describe](https://github.com/AnyaMankova/emco/blob/main/images/describe.png)
 Результат: 
- необычные/аномальные данные не обнаружены;
- имеются пропуски данных.

 Проанализируем пропуски данных. Общее количество пропусков равно 5 881.
![пропуски в датасете](https://github.com/AnyaMankova/emco/blob/main/images/nullst.png)

На рисунке по оси x указаны строки датасета, белые линии на нем отражают пропущенные значения.
Общее количество пропусков - примерно 17% от общего количества данных в датасете.

Для каждого атрибута данных проведем анализ.
Базовым методом проверки данных на нормальность распределения является гистограмма плотности распределения:
![гистограмма](https://github.com/AnyaMankova/emco/blob/main/images/all_hist.png)
Полученные гистограммы визуально соответсвуют признаку нормального распределения - имеют форму колокола, кроме того, во всех наблюдаемых выборках значения среднего, медианы и моды близки что позволяет предположить нормальное распределение выборок.
 
Нормализуем наши данные и 

Размах и стандартное отклонение подвержены выбросам, более надежной альтернативой является инверквартильный размах.
При описании количественного признака, распределение которого отличается от нормального, указываются медиана, значения нижнего и верхнего квартилей (или 25% и 75% перцентилей).
 которые не зависят от вида
распределения – так называемые н е п а р а м е т р и ч е с к и е к р и т е р и и .
мне нужно будет сравнить изменение данных в зависимости от месяца, модели камаза, смены

<<<<<<< HEAD
=======
для зависимых выборок (объем топлива и расстояние) надо будет провести тест по критерию вилкоксона
  
>>>>>>> d418fe3cf83073475c0ca80204e4175f0a31e292
  
  
  </p>
