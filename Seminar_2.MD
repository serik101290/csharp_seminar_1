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

Console.Clear();
Console.WriteLine("Zdorovo za---bal! Zadacha 13/Seminar 2");

Console.Write("Введи число: ");

int luboechislo = Convert.ToInt32(Console.ReadLine());

string luboechislovvode = Convert.ToString(luboechislo);

if (luboechislovvode.Length > 2)

{
  Console.WriteLine("третья цифра -> " + luboechislovvode[2]);

}

else {
  Console.WriteLine("-> третьей цифры нет");

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

