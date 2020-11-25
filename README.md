using System;

    class program
{
    static void Main()
    {

        Console.WriteLine(" Напишите коэффициэнты по порядку с a-b-c в уравнение вида: ax2+bx+c ");
       

       
        int num1 = int.Parse(Console.ReadLine());

        int num2 = int.Parse(Console.ReadLine());

        int num3 = int.Parse(Console.ReadLine());

        int D = num2 * num2 - 4 * num1 * num3;

        if (D == 0)
        {

            int K = (-num2 / (2 * num1));

            Console.WriteLine("Присутствует лишь один корень");
            Console.WriteLine(K);

        }
        else if (D > 0)
        {


            double K1 = (-num2 + Math.Sqrt(D) / (2 * num1));

            double K2 = (-num2 - Math.Sqrt(D) / (2 * num1));

            Console.WriteLine("Первый корень");
            Console.WriteLine(K1);
            Console.WriteLine("Второй коронь");
            Console.WriteLine(K2);


        }
        else
        {

            Console.WriteLine("Корней нет");

        }
 
         

    }


}
