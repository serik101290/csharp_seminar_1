**Задача 34 семинара 5**

Console.Clear();

int[] arr = new int[5]; 
Random rnd = new Random(); 
int even = 0; 

Console.WriteLine("Массив случайных трехзначных чисел:");
for (int i = 0; i < arr.Length; i++) 
{
    arr[i] = rnd.Next(100, 1000); 
    Console.Write(arr[i] + " "); 
}
Console.WriteLine(); 
        

for (int i = 0; i < arr.Length; i++) 
{
    if (arr[i] % 2 == 0) 
    {
        even++;
    }
}
Console.WriteLine("Количество четных элементов: " + even);

**Задача 36 семинара 5**
Console.Clear();

int[] arr = new int[5]; 
Random rnd = new Random(); 

Console.WriteLine("Массив случайных трехзначных чисел:");
for (int i = 0; i < arr.Length; i++) 
{
    arr[i] = rnd.Next(1, 1000); 
    Console.Write(arr[i] + " "); 
    
    Console.Write(" ");
}
int sumnoteven= 0;
for (int i = 1; i < arr.Length; i += 2)
{
    sumnoteven += arr[i];
}
Console.WriteLine("= " + sumnoteven);

**Задача 38 семинара 5**

Console.Clear();
Random rnd = new Random();
double[] arr = new double[5];

Console.WriteLine("Массив случайных чисел:");
for (int i = 0; i < arr.Length; i++)
{
    arr[i] = rnd.NextDouble() * 100;
    Console.Write(Math.Round(arr[i], 1, MidpointRounding.AwayFromZero) + " ");//Я эту функцию нашел на сайте майкрософта,
    Console.Write(" ");
}
double max = arr[0];
double min = arr[0];
for (int i = 1; i < arr.Length; i++)
{
    if (arr[i] > max)
    {
        max = arr[i];
    }
    if (arr[i] < min)
    {
        min = arr[i];
        Console.WriteLine(" ");
     }
}
double diff = max - min;
Console.WriteLine(" ");

Console.WriteLine("Максимальный элемент массива: " + Math.Round(max, 1, MidpointRounding.AwayFromZero));
 Console.WriteLine(" ");
Console.WriteLine("Минимальный элемент массива: " + Math.Round(min, 1, MidpointRounding.AwayFromZero));
 Console.WriteLine(" ");
Console.WriteLine("Разница между максимальным и минимальным элементами: " + Math.Round(diff, 1, MidpointRounding.AwayFromZero));