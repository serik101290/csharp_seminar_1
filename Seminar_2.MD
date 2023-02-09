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


Console.Clear();
Console.WriteLine("Zdorovo! zadacha 15 Seminar 2");

Console.Write("Введи цифру, означающую день недели: ");

int cifradnya = Convert.ToInt32(Console.ReadLine());

void CheckingTheDayOfTheWeek (int cifradnya) 

{

  if (cifradnya == 6 || cifradnya == 7) 
  {
  Console.WriteLine("(это выходной день) -> да");

  }

  else if (cifradnya < 1 || cifradnya > 7) 

  {
    Console.WriteLine("это не день недели");

  }

  else Console.WriteLine("(это не выходной день) -> нет");
  
}


CheckingTheDayOfTheWeek(cifradnya);

