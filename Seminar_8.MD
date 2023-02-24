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

**Задача 60 семинара 8**

Console.Clear();
Console.WriteLine("Задача 60");

int[,,] array = new int[2, 2, 2];
int num = 10;

for (int i = 0; i < 2; i++)
{
    for (int j = 0; j < 2; j++)
    {
        for (int k = 0; k < 2; k++)
        {
            array[i, j, k] = num++;
        }
    }
}
for (int i = 0; i < 2; i++)
{
    for (int j = 0; j < 2; j++)
    {
        for (int k = 0; k < 2; k++)
        {
            Console.WriteLine($"{array[i, j, k]} = [{i}, {j}, {k}]");
        }
    }
}4

**Задача 61 семинара 8**

Console.Clear();

Console.Write("Введите количество строк: ");
int rows = int.Parse(Console.ReadLine());

int[][] triangle = new int[rows][];

for (int i = 0; i < rows; i++)
{
    triangle[i] = new int[i + 1];
    for (int j = 0; j <= i; j++)
    {
        if (j == 0 || j == i)
        {
            triangle[i][j] = 1;
        }
        else
        {
            triangle[i][j] = triangle[i - 1][j - 1] + triangle[i - 1][j];
        }
    }
}

Console.WriteLine("Треугольник Паскаля:");
for (int i = 0; i < rows; i++)
{
for (int k = 0; k < rows - i; k++)
{
    Console.Write(" ");
}
// Вывод значений в строке
for (int j = 0; j <= i; j++)
{
    Console.Write("{0} ", triangle[i][j]);
}
    Console.WriteLine();
}
    Console.ReadLine();

**Задача 62 семинара 8**

Console.Clear();

Console.WriteLine("Задача 62");

int[,] array = new int[4, 4];

int row = 0, col = 0, direction = 0;
for (int i = 1; i <= 16; i++)
{
    array[row, col] = i;

    if (direction == 0)
    {
        if (col == 3 || array[row, col + 1] != 0)
        {
            direction = 1;
            row++;
        }
        else
        {
            col++;
        }
    }
    else if (direction == 1)
    {
        if (row == 3 || array[row + 1, col] != 0)
        {
            direction = 2;
            col--;
        }
        else
        {
            row++;
        }
    }
    else if (direction == 2)
    {
        if (col == 0 || array[row, col - 1] != 0)
        {
            direction = 3;
            row--;
        }
        else
        {
            col--;
        }
    }
    else if (direction == 3)
    {
        if (row == 0 || array[row - 1, col] != 0)
        {
            direction = 0; 
            col++;
        }
        else
        {
            row--;
        }
    }
}

for (int i = 0; i < 4; i++)
{
    for (int j = 0; j < 4; j++)
    {
        Console.Write("{0,2} ", array[i, j]);
    }
    Console.WriteLine();
}