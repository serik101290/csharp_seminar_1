**Задача 54 семинара 8**

Console.Clear();
Console.WriteLine("54 задача");

int[,] array = new int[,] 
{
    {1, 4, 7, 2},
    {5, 9, 2, 3},
    {8, 4, 2, 4}
};
for (int i = 0; i < array.GetLength(0); i++) 
{
    for (int j = 0; j < array.GetLength(1) - 1; j++) 
    {
        for (int k = j + 1; k < array.GetLength(1); k++) 
        {
            if (array[i, k] > array[i, j]) 
            {
                int temp = array[i, j];
                array[i, j] = array[i, k];
                array[i, k] = temp;
            }
        }
    }
}
for (int i = 0; i < array.GetLength(0); i++)
{
    for (int j = 0; j < array.GetLength(1); j++) 
    {
        Console.Write(array[i, j] + " ");
    }
        Console.WriteLine();
}

**Задача 56 семинара 8**

Console.Clear();
Console.WriteLine("56 задача");

int[,] array = new int[,] 
{
    {1, 4, 7, 2},
    {5, 9, 2, 3},
    {8, 4, 2, 4},
    {5, 2, 6, 7}
};

int minRowSum = int.MaxValue; 
int minRowIndex = -1; 

for (int i = 0; i < array.GetLength(0); i++) 
{
    int rowSum = 0;
    for (int j = 0; j < array.GetLength(1); j++) 
    {
        rowSum += array[i, j];
    }
    if (rowSum < minRowSum) 
    {
        minRowSum = rowSum;
        minRowIndex = i;
    }
}

Console.WriteLine($"Строка с наименьшей суммой элементов: {minRowIndex}");

**Задача 58 семинара 8**

Console.Clear();
Console.WriteLine("Задача 58");

int[,] A = { {2, 4}, {3, 2} };
int[,] B = { {3, 4}, {3, 3} };

int[,] C = new int[2, 2];

for (int i = 0; i < 2; i++)
{
    for (int j = 0; j < 2; j++)
        {
            for (int k = 0; k < 2; k++)
                {
                    C[i, j] += A[i, k] * B[k, j];
                }
            }
        }
for (int i = 0; i < 2; i++)
{
    for (int j = 0; j < 2; j++)
        {
            Console.Write(C[i, j] + " ");
        }
            Console.WriteLine();
}