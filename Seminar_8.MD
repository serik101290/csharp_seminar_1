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

