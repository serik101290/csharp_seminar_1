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

