**Задача 31 семинара 5**

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

