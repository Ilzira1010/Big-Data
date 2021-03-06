# Big-Data
# Проектная работа по анализу данных

**Работу выполнили**:
* Ахметдинова Ильзира, 11-906
* Бадртдинова Алсу, 11-909
* Камалова Лия, 11-907


**Тема работы**: "Методики работы с big data".
</br>  
**Датасет**: airport-codes.csv содержит данные об аэропортах, рейсах, направлениях. 
</br>  

**Цель**: Продемонстрировать различные подходы работы с BigData, используя Dask, pandas, parquet, Spark. Полное описание проекта с объяснением всех шагов находится в блокноте.


</br>  

## Что такое большие данные и почему для работы с ними нужны отдельные подходы?

Big Data (большие данные) — огромные наборы разнообразных данных. Огромные, потому что их объемы такие, что простой компьютер не справится с их обработкой, а разнообразные — потому что эти данные разного формата, неструктурированные и содержат ошибки. Большие данные быстро накапливаются и используются для разных целей.


Big Data это:
Сами массивы данных.
Инструменты. Метатермин в наше время, не относится к самим данным.
Подходы и методы их обработки.
Любое использование больших данных — это:

Дорого.
Должно себя окупать

Spark — современный и высокоуровневый инструмент для обработки больших массивов информации. Самый распространённый фреймворк для работы с ML на больших данных и расчетов на них.

Индустриальный стандарт.
Под капотом Spark написан на Scala, поэтому через Scala вызовы на него самый богатый доступ к API.
Scala - это JVM friendly язык, поэтому вся логика Spark будет транслироваться в поток байт для JVM.
В питоновских структурах данных есть проблемы, так как Python медленнее Scala. Scala в некоторых тестах может быть в несколько раз или на порядки быстрее Python. Есть бенчмарки, оформленные в виде статей от Димы Бугайченко.
PySpark хватает для 90 процентов задач, остальные 10 процентов будут не так эффективны, но даже они не сильно критичны для маленьких кластеров.

Dask — это библиотека анализа данных с обеспечением параллельных вычислений и масштабируемой производительностью, а также с интеграцией с другими Python-инструментами: Numpy, Pandas и Scikit-learn. Библиотека имеет в основе существующие API-интерфейсы на Python и структуры данных, чтобы упростить переключение между библиотеками.

Датафреймы Dask не полностью совместимы с Pandas, но некоторые наиболее распространенные операции обработки данных всё же поддерживаются обоими библиотеками. Dask больше ориентирован на масштабирование с вычислениями на кластерах.\

Parquet — это хранилище столбцов, что означает, что он может эффективно извлекать только несколько столбцов из вашего набора данных. Это хорошо, потому что помогает избежать ненужной загрузки данных.
