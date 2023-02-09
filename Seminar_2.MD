**Задача 10 к семинару 2**
Здравствуйте, здесь код почему ошибку выдает. И работает только на 1 раз. Когда щаново дотнетран делаешь, выводит текст только с ошибкой
Console.Clear();

Console.Write("Seminar_2/Zadanie_10 ");

Console.WriteLine("Введи число! ");
int n = Convert.ToInt32(Console.ReadLine());
while (n < 99 || n > 999)
{
    Console.Write("Ошибка! Введи 3-хзначное число ");
    int n2 = Convert.ToInt32(Console.ReadLine());
}
Console.WriteLine($"Результат: {n / 10 % 10}");
И еще одно решение:
 Console.WriteLine("Enter a three-digit number:");
            int number = int.Parse(Console.ReadLine());

            int secondDigit = (number / 10) % 10;

            Console.WriteLine("The second digit of the number is: " + secondDigit);


**Задача 13 к семинару 2**
Тут стало ясно, что пока число меньше 100 оно не 3-хзначное, а если больше 1000 нужно делить на 10 и находить остаток.
Console.Clear();
Console.WriteLine("Zdorovo! Zadacha 13/Seminar 2");

Console.WriteLine("Введи число:");
int number = Convert.ToInt32(Console.ReadLine());

if (number < 100)
{
  Console.WriteLine("3-й цифры нет: ");
}
else
{
  while (number > 1000)
  {
    number = number / 10;
  Console.WriteLine($"Результат: {number} % 10 = {number % 10}");
}
}



**Задача 15 к семинару 2**
Здесь я проверил код, но он пятницу здесь выходным выдает.

Console.Clear();
Console.WriteLine("Введи номер дня недели (1-7):");
int day = Convert.ToInt32(Console.ReadLine());
while (day < 1 || day > 7)
{
  Console.Write("It's now week day");
  day = Convert.ToInt32(Console.ReadLine());
}
if (day>=5)
{
  Console.WriteLine("It's a weekend!");
}
else
{
 Console.WriteLine("It's a weekday.");
}

