// Пользователь вводит с клавиатуры M чисел. Посчитайте, сколько чисел больше 0 ввёл пользователь.
//0, 7, 8, -2, -2 -> 2
//1, -7, 567, 89, 223-> 3

void CountNull(int[] a, int m)

{

    int n = 0;
    
    for (int i=0;i<m;i++)
    
    {
       if (a[i]> 0)
       
       {
        n = n+1;
       }
       
    }
    
    Console.WriteLine($"{n} чисел, больших 0");
    
}

Console.WriteLine("Введите размерность массива: ");

int m = Convert.ToInt32(Console.ReadLine());

int[] a = new int[m];

Console.WriteLine("Введите элементы массива: ");

for (int i = 0; i<m; i++)

{
    a[i] = Convert.ToInt32(Console.ReadLine());
}

CountNull(a, m);
