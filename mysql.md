# Mysql

## Индексы

Индекс формируется из значений одного или нескольких столбцов таблицы и указателей на соответствующие строки таблицы и, таким образом, позволяет искать строки, удовлетворяющие критерию поиска. Ускорение работы с использованием индексов достигается в первую очередь за счёт того, что индекс имеет структуру, оптимизированную под поиск, например хэш таблицы или сбалансированные деревья.

Хеш-таблицам свойственны коллизии, когда для различных ключей получается одно и тоже хэш значение.

Некоторые общие принципы, связанные с созданием индексов:

- индексы необходимо создавать для столбцов, которые используются в джойнах, по которым часто производится поиск и операции сортировки. При этом необходимо учесть, что индексы всегда автоматически создаются для столбцов, на которые накладывается ограничение primary key. Чаще всего они создаются и для столбцов с foreign key;
- индекс обязательно в автоматическом режиме создается для столбцов, на которые наложено ограничение уникальности;
- лучше всего индексы создавать для тех полей, в которых - минимальное число повторяющихся значений и данные распределены равномерно.
- Если поиск постоянно производится по определенному набору столбцов (одновременно), то в этом случае, возможно, есть смысл создать композитный индекс - один индекс для группы столбцов;
- при внесении изменений в таблицы автоматически изменяются и индексы, наложенные на эту таблицу. В результате индекс может быть сильно фрагментирован, что сказывается на производительности. Периодически следует проверять степень фрагментации индексов и дефрагментировать их. При загрузке большого количества данных иногда есть смысл вначале удалить все индексы, а после завершения операции создать их заново;

## Движки таблиц MySql

- MyIsam
- InnoDB
- Memory
- Blackhole

##   

##  

##  

##  JOIN

## ![](media/image6.jpeg){width="4.583333333333333in" height="3.6145833333333335in"}

# 