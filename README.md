using System;

namespace ConsoleApp1
{
    /* Pedir por consola las dimensiones de una matriz de dos dimensiones. 
     * Luego ingresas valores num{ericos enteros e imprimir la matriz con el siguiente formato: 
     * para cada valor de la matriz una linea que diga MATRIZ [x,y]=VALOR
     */
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Cuantas filas");
            string filas = Console.ReadLine();
            int fila = int.Parse(filas);
            Console.WriteLine("Cuantas columnas");
            string columnas = Console.ReadLine();
            int col = int.Parse(filas);
            Console.WriteLine("Cuantas columnas");
            int[,] matriz = new int[fila, col];
            for (int i = 0; i < fila; i++)
            {
                for (int j = 0; j < fila; j++)
                {
                    Console.WriteLine("Ingrese un número");
                    string ingreso = Console.ReadLine();
                    matriz[i, j] = int.Parse(ingreso);

                }
               


            }
            for (int k = 0; k < fila; k++)
            {
                for (int l = 0; l < fila; l++)
                {
                    Console.WriteLine("Matriz [{0}{1}]={2}", k ,l ,matriz[k, l]);
                    string ingreso = Console.ReadLine();


                }


            }
        }
    }
}
