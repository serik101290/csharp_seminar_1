**Задача 19 семинара 3**

Console.WriteLine("Введи 5-тизначное число:");
int number = int.Parse(Console.ReadLine());

int d1 = number / 10000;
int d2 = (number / 1000) % 10;
int d3 = (number / 100) % 10;
int d4 = (number / 10) % 10;
int d5 = number % 10;

if (d1 == d5 && d2 == d4)
{
    Console.WriteLine("Число палиандром.");
}
else
{
    Console.WriteLine("Число не палиандром.");
}

**Задача 21 семинара 3**

Console.Clear();

Console.WriteLine("Seminar_3/Zadacha_21");
//Сначала вводим координаты x,y,z 1-й точки. 
Console.WriteLine("Введи x координату 1-й точки: ");
double x1 = Convert.ToDouble(Console.ReadLine());
Console.WriteLine("Введи y координату 1-й точки: ");
double y1 = Convert.ToDouble(Console.ReadLine());
Console.WriteLine("Введи z координату 1-й точки: ");
double z1 = Convert.ToDouble(Console.ReadLine());
//ВВодим координаты 2-й точки
Console.WriteLine("Введи x координату 2-й точки: ");
double x2 = Convert.ToDouble(Console.ReadLine());
Console.WriteLine("Введи y координату 2-й точки: ");
double y2 = Convert.ToDouble(Console.ReadLine());
Console.WriteLine("Введи z координату 2-й точки: ");
double z2 = Convert.ToDouble(Console.ReadLine());
//Находим расстояние с помощью суммы квадратов разностей координат точек и длине разности радиоусов
double distance = Math.Sqrt(Math.Pow(x2 - x1, 2) + Math.Pow(y2 - y1, 2) + Math.Pow(z2 - z1, 2));
//Выводим результат
Console.WriteLine(Math.Round(+distance, 2));

**Задача 23 семинара 3**

Console.Clear();

Console.Write("Zadacha_21/Seminar_3/Вывод таблицы кубов число до N ");

Console.WriteLine("Введи число ");
int n = Convert.ToInt32(Console.ReadLine());

for (int i = 1; i <= n; i++)
{
   Console.WriteLine($"{i} ^ 3 = {i * i * i}"); 
}
