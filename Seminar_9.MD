**Задача 66 семинара 9**

Console.Clear();

Console.Write("Введите 1-e натуральное число: ");
int m = int.Parse(Console.ReadLine());

Console.Write("Введите 2-e натурально число: ");
int n = int.Parse(Console.ReadLine());

int sum = SumNatlNumb(m, n);

Console.WriteLine("Сумма натуральных чисел от {0} до {1} равна {2}", m, n, sum);

static int SumNatlNumb(int m, int n) 
{
    if (m == n) 
    {
        return m;
    } 
    else 
    {
        return m + SumNatlNumb(m + 1, n);
    }
}

**Задача 68 семинара 9**

Console.Clear();
Console.Write("Введите число m: ");
int m = int.Parse(Console.ReadLine());

Console.Write("Введите число n: ");
int n = int.Parse(Console.ReadLine());

int result = Akerman(m, n);
Console.WriteLine("Результат функции Аккермана для m={0} и n={1} равен {2}", m, n, result);

Console.ReadKey();

int Akerman(int m, int n)
{
   
 if (m == 0)
    {
        return n + 1;
    }
else if (n == 0)
    {
        return Akerman(m - 1, 1);
    }
else
    {
        return Akerman(m - 1, Akerman(m, n - 1));
    }
}