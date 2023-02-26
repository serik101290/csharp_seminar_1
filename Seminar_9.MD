**Задача 66 семинара 9**

Console.Clear();

Console.Write("Введите 1-e натуральное число: ");
int m = int.Parse(Console.ReadLine());

Console.Write("Введите второе натурально число: ");
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

