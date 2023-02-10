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

