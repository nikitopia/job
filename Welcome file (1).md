**Проверка компонента: HDFS**
>Проверка версии 
>>hadoop version
>____

>Проверка версии Java
>>java -version
___
>Запуск hadoop 
>> start.all.sh
>___

>Создание директории в HDFS
>>hadoop fs -mkdir /hduser/Input
___
>Создание файла в домашней папке
>> cat > text.csv
___

>Перенос созданного файла из домашней папки в директорию HDFS
>> hadoop fs -put  /home/master/Документы/test.csv /hduser/Input
___

>Удалить созданную директорию
>> hadoop fs -rm -R /hduser/Input
___

Проверка компонента: YARN
>Запуск одного из приложений yarm, подсчет pi из пакета hadoop-mapreduce-examples.jar:
>>yarn jar /usr/local/hadoop/hadoop-2.9.2/share/hadoop/mapreduce/hadoop-mapreduce-examples-2.9.2.jar pi 16 10000000
