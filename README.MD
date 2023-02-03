Здравствуйте, Денис! Вот высылаю вам в текстовом файле задания к семинару 1.

Напишу просто код в данный файл.

Задание на хождение максимального и минимального числа.

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

