**Задача 25 семинара 4**

Console.Clear();

Console.WriteLine("Введи число А:");
int nA = Convert.ToInt32(Console.ReadLine());

Console.WriteLine("Введи число В: ");

int nB = Convert.ToInt32(Console.ReadLine());
int result = 1;

for (int i = 0; i < B; i++)
{
    result *= nA;
}
Console.WriteLine("Result: " + result);


**Задача 27 семинара 4**

Console.Clear();

Console.WriteLine("Enter a number:");
int number = Convert.ToInt32(Console.ReadLine());
int sum = 0;
while (number > 0)
{
    sum += number % 10;
    number /= 10;
}
Console.WriteLine("Sum of digits: " + sum);

