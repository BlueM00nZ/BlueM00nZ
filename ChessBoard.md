using System;
using System.Collections.Generic;
using System.Globalization;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            WhiteBoard(5);
            WhiteBoard(1);
            WhiteBoard(10);
            WhiteBoard(8);

            Console.Read();
        }

        static void WhiteBoard(int size)
        {
            Console.WriteLine($"ChessBoard on {size} x {size}");
            for (int i = 0; i < size; i++)                           
            {                                                        
                for(int j = 0; j < size; j++)                        
                {
                    if (i % 2 == 0)
                    {
                        if (j % 2 == 0)
                            Console.Write('#');
                        else
                            Console.Write('.');
                    }
                    else
                    {
                        if (j % 2 == 0)
                            Console.Write('.');
                        else
                            Console.Write('#');
                    }
                    
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
