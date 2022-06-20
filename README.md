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
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace Alex
{
    class Alex
    {
        private double[] Valores; //declaramos valores

        public void cargar()
        {
            Valores = new double[6]; //iniciamos en 5 
            for (int f = 1; f <= 5; f++)
            {
                Console.WriteLine("Ingrese 5 numeros " + f + ": ");
                String linea;
                linea = Console.ReadLine();
                Valores[f] = int.Parse(linea);//Agregamos los 5 valores
            }
        }
        //para mostrar los numeros
        public void imprimir()
        {
            Console.Write("Ingrese 5 valores");
            for (int f = 1; f <= 5; f++)
            {
                Console.Write("[" + Valores[f] + "]");
            }
            Console.ReadKey();
        }
        //menu principal
        static void Main(String [] args)
        {
            Alex pv = new Alex();
            pv.cargar();
            pv.imprimir();
        }
        }

            }
        
