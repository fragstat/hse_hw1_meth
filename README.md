# hse_hw1_meth
-----------------
### [Colab](https://colab.research.google.com/drive/1xfETB4pEkqle7dYU9JWJ-L7rOT8NQcwE?usp=sharing)
## Анализ QC прочтений
-------------
## Какие особенности можно наблюдать по сравнению с секвенированием ДНК или РНК?
По сравнению с секвенированием ДНК и РНК можно отметить необычный нуклеотидный состав. Гуанин и аденин присутствуют в нормальном процентном соотношении (23-30%). В то же время тимин преобладает (около 45%), а цитозина очень мало (около 5%). 
Состав можно объяснить тем, что в бисульфитном секвенировании неметилированные цитозины превращаются в урацил, а урацил воспринимается ферментами как тимин. 
## Соотношение нуклеотидов в составе
-----------
![1_image](https://github.com/fragstat/hse_hw1_meth/blob/main/images/nucleotides.png?raw=true) 
## GC-состав
-----------
![2_image](https://github.com/fragstat/hse_hw1_meth/blob/main/images/GC.png?raw=true) 
## Статистика по каждому из 3 образцов
|Номер образца|Тип клеток|Риды на 11347700-11367700 нуклеотидах|Риды на 40185800-40195800 нуклеотидах|% дуплицированных|
|---------------|----------|-------------------------|---------------------------|---------------|
|SRR5836473|8 cell|1090|464|18.31%|
|SRR3824222|Epiblast|2328|1062|2.92%|
|SRR5836475|ICM|1456|630|9.08%|
## M-bias графики
---------------
8 cell

![3_image](https://github.com/fragstat/hse_hw1_meth/blob/main/images/8cell_1_bias.png?raw=true)
![4_image](https://github.com/fragstat/hse_hw1_meth/blob/main/images/8cell_2_bias.png?raw=true)

Epiblast

![5_image](https://github.com/fragstat/hse_hw1_meth/blob/main/images/epiblast_1_bias.png?raw=true)
![6_image](https://github.com/fragstat/hse_hw1_meth/blob/main/images/epiblast_2_bias.png?raw=true)

ICM

![7_image](https://github.com/fragstat/hse_hw1_meth/blob/main/images/icm_1_bias.png?raw=true)
![8_image](https://github.com/fragstat/hse_hw1_meth/blob/main/images/icm_2_bias.png?raw=true)

Метилированных нуклеотидов в клетках Epiblast выше по сравнению с другими типами клеток. 
Также в ридах у клеток ICM и 8 cell с обратными цепями наблюдается чуть больший процент метилирования в начале последовательности, в клетках Epiblast процент метилирования в начале образца наоборот чуть меньше.
Риды с разбросом метилирования можно игнорировать, так как bias не так значительно отклоняется.


------------
## Гистограммы распределения метилирования цитозинов по хромосоме
8 cell

![9_image](https://github.com/fragstat/hse_hw1_meth/blob/main/images/8cell_met_c.png?raw=true) 

Epiblast

![10_image](https://github.com/fragstat/hse_hw1_meth/blob/main/images/epiblast_met_c.png?raw=true) 

ICM

![11_image](https://github.com/fragstat/hse_hw1_meth/blob/main/images/icm_met_c.png?raw=true) 

Полученные графики идентичны графикам из статьи.
Метилирование сильнее в образце Epiblast, в ICM большая часть цитозина не метилирована, а в 8 cell распределение по метидированию равномерное.
-----------
## Уровень метилирования и покрытия для каждого образца

![12_image](https://github.com/fragstat/hse_hw1_meth/blob/main/images/level_met_c.png?raw=true)
