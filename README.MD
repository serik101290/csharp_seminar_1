Здравствуйте, Денис! Вот высылаю вам в текстовом файле задания к семинару 1.

Напишу просто код в данный файл.

**Задание на хождение максимального и минимального числа**

Console.Clear();

Console.WriteLine("Введите два разных целых числа!");

		if(int.TryParse(Console.ReadLine(), out var firstNumber))

		{
			Console.WriteLine("Ok!");
		}
		else
		{
			Console.WriteLine("Это не целое числом");
		}
		if(int.TryParse(Console.ReadLine(), out var secondNumber))
		{
			Console.WriteLine($"Отлично!2-е число {secondNumber}");
		}
		else
		{
			Console.WriteLine("Это не целое число");
		}

		if (firstNumber > secondNumber) 
		{
			Console.WriteLine($"Большее число {firstNumber}, меньшее число {secondNumber}");
		}
		else if (secondNumber > firstNumber)
		{
			Console.WriteLine($"Большее число {secondNumber}, меньшее число {firstNumber}");
		}
		else 
		{
			Console.WriteLine("Ты ввел неправильные значения, попробуй еще разок!");
        }

**Задание на поиск max out of 3 numbers**

Console.Clear();

int max = 0;

Console.Write("Введи 1-е число: ");
int firstNumber = Convert.ToInt32(Console.ReadLine());

Console.Write("Введи 2-е число: ");
int secondNumber = Convert.ToInt32(Console.ReadLine());

Console.Write("Введи 3-е число: ");
int thirdNumber = Convert.ToInt32(Console.ReadLine());

if(firstNumber > max)
{
    max = firstNumber;
}
if(secondNumber > max)
{
    max = secondNumber;
}
if(thirdNumber > max)
{
    max = thirdNumber;
}

Console.WriteLine("max = " + max);

**Здесь на задача на поиск четного числа**

Console.Clear();
Console.WriteLine("Hello, World!");

Console.Write("Введи число: ");
int number = Convert.ToInt32(Console.ReadLine());

int remDiv = number % 2;

if(remDiv == 0)
{
    Console.WriteLine("Четное");
}
else
{
    Console.WriteLine("Нечетное");
}