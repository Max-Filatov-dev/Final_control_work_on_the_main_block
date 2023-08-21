# Этот репозиторий специально создан для контрольной работы основного блока.

## Задача:

Написать программу, которая из имеющегося массива строк формирует новый массив из строк, длина которых меньше, либо равна 3 символам. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.

## Алгоритм решения:

1. Согласно условиям задачи, первоначальный массив можно задать самому, так и поступим. Объявляем, произвольно заполненый строковыми элементами, массив.

    ```C#
    string [] array = {"Hello", "TV", "World", "Max"}
    ```

2. Объявляем метод, в качестве параметра он будет принимать наш массив строк. В методе пробежим циклом с условием, длина элемента <= 3, по массиву, если элемент соответсвует условию цикла, увеличиваем значение переменной "счетчика" (инкремент переменной). В результате метод вернет значение int переменной "счетчика".

    ```C#
    int NameMethod(string [] arr)
    ```
3. Объявляем новый метод, в качестве параметра он будет принимать наш массив строк, а так же результат возрата, int значение, первого метода.

    ```C#
    string [] NewNameMethod(string [] arr, int len)
    ```
    - В методе, объявляем новый строковый массив, длина которого равняется значению параметра len. Этот новый массив будем возваращать в результате выполнения.

        ```C#
        string [] newArray = new string[len]
        ``````
    - Далее пробежим циклом с условием, длина элемента <= 3, по массиву, и если элемент соответсвует условию цикла, добавляем текущий элемент в наш новый массив.

4. Чтобы вывести результат возврата последнего метода в терминал, создадим отдельный метод с циклом перебора массива. 