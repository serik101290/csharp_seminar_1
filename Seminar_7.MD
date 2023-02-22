**Задача 47 семинара 7**

Console.Clear();

Random random = new Random();

double[,] arr = new double[3, 4];

for (int i = 0; i < 3; i++)
    {
        for (int j = 0; j < 4; j++)
            {
                arr[i, j] = random.NextDouble() * 10 -5;
            }
    }
for (int i = 0; i < 3; i++)
    {
        for (int j = 0; j < 4; j++)
            {
                Console.Write(Math.Round(arr[i, j], 2) + " ");
            }
            Console.WriteLine();
    }

**Задача 50 семинара 7**

Console.Clear();

int[,] array = new int[,]
    {
        { 1, 4, 7, 2 },
        { 5, 9, 2, 3 },
        { 8, 4, 2, 4 },
        { 1, 7, 0, 0 }
    };
Console.Write("Введи номер строки: ");
int line = Convert.ToInt32(Console.ReadLine());

Console.Write("Введи номер столбца: ");
int column = Convert.ToInt32(Console.ReadLine());

int lineCount = array.GetLength(0);
int columnCount = array.GetLength(1);

if (line >= lineCount || column >= columnCount)
    {
        Console.WriteLine("На данной позиции в массиве нет элемента.");
    }
else
    {
        int element = array[line, column];
        Console.WriteLine($"На данной позиции находится элемент {element}.");
    }

