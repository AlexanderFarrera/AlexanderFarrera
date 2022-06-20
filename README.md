- 👋 Hi, I’m @AlexanderFarreraDiego_No.de control_20887049_informatica
- 👀 I’m interested in ....Aprender mucho.
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me  a mi whatssapp: 9661043291

<!---
AlexanderFarrera/AlexanderFarrera is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

//FARRERA DIEGO ERVIN ALEXANDER_20887049_INFORMATICA_4_E.
//BELEN ESTEFANIA PEREZ NUCAMENDI_20887036_INFORMATICA_4_E.

//Belen Estefania Perez Nucamendi 
//Farrera Diego Ervin Alexader

using System;
using System.Threading;
namespace Menoramayor
{
    class Program
    {
        public static void Main(string[] args)
        {

            int mydelay = 1000;
            {

                //Creamos un vector (Array) de enteros con una longitud de 5 elementos
                double[] numeros = new double[5];

                //Solicitamos al usuario los 5 valores (desordenados)
                for (int i = 0; i < 5; i++)
                {
                    Console.WriteLine("Ingrese un valor:");

                    numeros[i] = double.Parse(Console.ReadLine());

                }

                //Ordenamos la lista e imprimimos los valores.
                Array.Sort(numeros);

                Console.WriteLine("\nLos números ordenados de menor a mayor son:");

                for (int i = 0; i < 5; i++)
                {
                    Console.WriteLine(numeros[i]);
                    Thread.Sleep(mydelay);
                }

                Array.Reverse(numeros);
                Console.WriteLine("\nLos números ordenados de mayor a menor son:");

                for (int i = 0; i < 5; i++)
                {
                    Console.WriteLine(numeros[i]);
                    Thread.Sleep(mydelay);
                }

                Console.WriteLine("\nLos Datos han sido guardados");
                using (StreamWriter writer = new StreamWriter("ArchivodeErvin.txt", false))
                {
                    for (int i = 0; i < numeros.Length; i++)
                    {
                        writer.WriteLine(numeros[i].ToString());
                    }
                }


                //Para mantener la consola abierta
                Console.ReadKey();
            }
        }
    }
}
