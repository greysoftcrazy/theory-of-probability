## Лекция 1. Правила сложения и умножения

** [Комбинаторика](../../GLOSSARY.md#комбинаторика) ** - это наука, с который каждый встречается в повседневной жизни: сколько способов выбрать 3 дежурных для уборки класса или сколько способов составить слово из данных букв. В целом, комбинаторика позволяет вычислить, сколько различных комбинаций, согласно некоторым условиям, можно составить из заданных объектов (одинаковых или разных).

Как наука комбинаторика возникла еще в 16 веке, а теперь ее изучает каждый студент (и даже школьник). Начинают изучение с понятий *перестановок, размещений, сочетаний* (с повторениями или без). Наиболее известные правила комбинаторики - *правила суммы и произведения*, которые чаще всего применяются в типовых комбинаторных задачах. Два основных правила комбинаторной теории:

**Правило сложения**

Возможно, это правило покажется непосвященному человеку абракадаброй, но ничего сложного нет. Рассмотрим пример – *пусть в одном ящике есть **m** шариков, а во втором ящике – **n** шариков. Сколькими способами можно вытащить шарик из одного этих ящиков*. Очевидно, что ОДИН шарик можно достать ***m+n*** способами.

Закон сложения используется тогда, когда нужно выбрать **только 1 элемент**.

*Пример 1.*  

Вика должна выбрать только один десерт из 8 видов коктейля, 5 видов мороженого и 5 видов йогурта. Сколькими способами она может выбрать десерт?

*Решение.*

Используется закон сложения, т.к. Вика должна выбрать или коктейль, или мороженое, или йогурт.

$$ 8+5+5=18 $$

*Ответ:* Вика может выбрать десерт 18 способами.

При использовании закона сложения надо следить, чтобы ни один из способов выбора объекта **a** не совпадал с каким-либо способом выбора объекта **b**. 

Если объект a можно получить $$ k $$ способами, объект $$ b $$ — $$ n $$ способами, то объект «$$ a $$ или $$ b $$ » можно получить $$ k+n−m $$ способами, где $$ m $$ — это количество повторяющихся способов.

*Пример 2.*

В группе 7 человек имеют «5» по математике, 9 человек — «5» по философии. В сессии 2 экзамена. Известно, что 4 человека сдали сессию отлично. Сколько человек имеют хотя бы одну пятерку в сессии?

*Решение.* 

$$ 7 + 9 - 4 = 12 $$

**Правило умножения** Пусть объект А выбирается **m** способами, объект В выбирается **n** способами, то оба объекта можно выбрать **m·n** способами.

Все очень просто – каждый из **m** способов выбора объекта А комбинируется с каждым из **n** способов выбора объекта В, то есть количество способов просто умножается друг на друга.

*Пример3.* 

Сколько чисел можно составить из цифр 0,1,2,3,4,5,6,7,8,9, если число должно быть двузначным? 

*Решение.*

Можно составить 90 чисел – первую цифру числа (объект А) можем выбрать 9 способами, так как число не может начинаться с нуля. Вторую цифру числа (объект В) можем выбрать 10 способами, так как у нас есть 10 цифр. Итого получается 9·10=90 чисел.


*Пример 4.* 

В классе учится 16 мальчиков и 10 девочек. Сколькими способами можно назначить двух дежурных?

*Решение.*

Первым дежурным можно назначить либо мальчика, либо девочку. Т.к. в классе учится 16 мальчиков и 10 девочек, то назначить первого дежурного можно 16+10=26 способами.

После того, как мы выбрали первого дежурного, второго мы можем выбрать из оставшихся 25 человек, т.е. 25-ю способами.

По теореме умножения двое дежурных могут быть выбраны 26·25=650 способами.

Пусть требуется выполнить последовательно $$ k $$ действий. Если первое действие можно выполнить $$ n_1 $$ способами, второе действие  $$ n_2 $$ способами,  третье – $$ n_3 $$ способами и так до $$ k $$ -го действия, которое можно выполнить  $$ n_k $$ способами, то все $$ k $$ действий вместе могут быть выполнены: $$ n_1 · n_2 ... n_k  $$ способами.


<quiz id="test" name="<h3> Выполните тестовое задание по материалу лекции</h3>">
    <question>
        <p>На стоянке такси находятся 3 автомобиля Audi, 5 автомобилей Hyundai и 7 автомобилей Toyota. Сколькими способами можно выбрать машину для поездки?</p>
        <answer>1</answer>
        <answer>12</answer>
        <answer correct>15</answer>
        <answer>22</answer>
    </question>
    <question>
        <p>В группе 7 человек имеют «5» за экзамен по математике, 9 человек — «5» за экзамен по философии. В сессии 2 экзамена: математика и философия. Известно, что 4 человека сдали сессию отлично. Сколько человек имеют хотя бы одну пятерку в сессии?</p>
        <answer correct>12</answer>
        <answer>16</answer>
        <answer>20</answer>
        <answer>32</answer>
    </question>
    <question>
        <p>Закон сложения используется тогда, когда надо выбрать ...</p>
        <answer correct>1 элемент</answer>
        <answer>2 элемента</answer>
        <answer>3 элемента</answer>
        <answer>Сколько угодно элементов</answer>
    </question>
    <question>
        <p>В классе учится 17 мальчиков и 9 девочек. Сколькими способами можно назначить двух дежурных?</p>
        <answer>26</answer>
        <answer>153</answer>
        <answer>306</answer>
        <answer correct>650</answer>
    </question>
    <question>
        <p>На стоянке такси находятся 3 автомобиля Audi, 5 автомобилей Hyundai и 7 автомобилей Toyota. Сколькими способами можно выбрать три  машины для поездки?</p>
        <answer>15</answer>
        <answer>210</answer>
        <answer>455</answer>
        <answer correct>2730</answer>
    </question>
</quiz>



