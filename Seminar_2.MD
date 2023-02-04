**Задача 10 к семинару 2**

Console.Clear();

Console.WriteLine("Задача 10/Семинар 2");
Console.Write("Введи трёхзначное число: ");
int xxx4islo = Convert.ToInt32(Console.ReadLine());
string snumber = Convert.ToString(xxx4islo);
Console.WriteLine("вторая цифра этого числа -> "+snumber[1]);


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

