**Задача 41 семинара 6**

Console.Clear();

Console.Write("Напиши желаемое количество чисел: ");
int m = Convert.ToInt32(Console.ReadLine());
        
int count = 0; 

for (int i = 0; i < m; i++)
{
    Console.Write($"Введи числа {i+1}: ");
    int number = Convert.ToInt32(Console.ReadLine());
if (number > 0)
    {
    count++; 
    }
}
Console.WriteLine($"Количество чисел, больше нуля: {count}");


