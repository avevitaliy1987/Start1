Задаем два массива:
string[] array1 = new string[6] {"1234", "hello", "234", "wor", ":)", "string"};
string[] array2 = new string[array1.Length];

Создаем метод, который на вводе принимает два заданных массива:

void MetArray2(string[] array1, string[] array2)

Задаем счетчик
{
    int count = 0;
    for (int i = 0; i < array1.Length; i++)
Задаем условие, при котором если элемент массива array1 <= 3, то такой элемент выводим в массиме array2.
    {
    if(array1[i].Length <= 3)
        {
        array2[count] = array1[i];
        count++;
        }
    }
}

Задаем метод вывода массива

void PrintArray(string[] array)
{
    for (int i = 0; i < array.Length; i++)
    {
        Console.Write($"{array[i]} ");
    }
    Console.WriteLine();
}

Используем метод

MetArray2(array1, array2);

Выводим массив array2

PrintArray(array2);
