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



