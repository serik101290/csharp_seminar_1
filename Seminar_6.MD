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

**Задача 43 семинара 6**

Console.Clear();

Console.WriteLine("Введите значения k1, b1, k2 и b2");

Console.WriteLine("Введи B1");
double b1 = Convert.ToDouble(Console.ReadLine());

Console.WriteLine("Введи K1");
double k1 = Convert.ToDouble(Console.ReadLine());

Console.WriteLine("Введи B2");
double b2 = Convert.ToDouble(Console.ReadLine());

Console.WriteLine("Введи K2");
double k2 = Convert.ToDouble(Console.ReadLine());

double x = (b2 - b1) / (k1 - k2);
double y = k1 * x + b1;

Console.WriteLine($"Точка пересечения: ({x}, {y})");

