# Zad3
{
            Console.WriteLine("Kalkulator mnożenia 2 liczb");
            Console.Write("Podstaw a= " );
            long a = long.Parse(Console.ReadLine());
            Console.Write("Podstaw b= ");
            long b = long.Parse(Console.ReadLine());
            long wynik = a * b;
            Console.WriteLine(a + " x " + b + " = " + wynik);
}
#Zad3pkt1
 {
            Console.WriteLine("Kalkulator");
            Console.WriteLine("Jaką chcesz wybrać operacje:");
            Console.WriteLine("1. Odejmowanie");
            Console.WriteLine("2. Dodawanie");
            long wybor = long.Parse(Console.ReadLine());
            if (wybor == 1)
            {
                Console.Write("Podstaw a= ");
                long a = long.Parse(Console.ReadLine());
                Console.Write("Podstaw b= ");
                long b = long.Parse(Console.ReadLine());
                long wynik = a - b;
                Console.WriteLine(a + " - " + b + " = " + wynik);
            }
            else if(wybor==2)
            { 
            Console.Write("Podstaw a= ");
            long a = long.Parse(Console.ReadLine());
            Console.Write("Podstaw b= ");
            long b = long.Parse(Console.ReadLine());
            long wynik = a + b;
            Console.WriteLine(a + " + " + b + " = " + wynik);
            }
            else
            {
                Console.WriteLine("Nie ma takiego wyboru. Wybierz 1 lub 2, natępnie naciśnij Enter");
            }
#Zad3pkt2
{
            float wynik = 0;
            Console.WriteLine("Wpisz liczby");
            Console.Write("a= ");
            float a = float.Parse(Console.ReadLine());
            Console.Write("b= ");
            float b = float.Parse(Console.ReadLine());
            Console.Write("Wybierz operację: ");
            string operacja = Console.ReadLine();
            switch (operacja)
            {

                case "+":
                    wynik = a + b;
                    break;
                case "-":
                    wynik = a - b;
                    break;
                case "*":
                    wynik = a * b;
                    break;
            }
            Console.WriteLine("Wynik= " + wynik);
        }
#zad3pkt3
        {
            float wynik = 0;
            Console.WriteLine("Wpisz liczby");
            Console.Write("a= ");
            float a = float.Parse(Console.ReadLine());
            Console.Write("b= ");
            float b = float.Parse(Console.ReadLine());
            Console.Write("Wybierz operację: ");
            string operacja = Console.ReadLine();
            switch (operacja)
            {

                case "+":
                    wynik = a + b;
                    break;
                case "-":
                    wynik = a - b;
                    break;
                case "*":
                    if (a == 0 || b == 0)
                    {
                        Console.WriteLine("Nie można dzielić przez 0!");
                    }
                    else
                    {
                        wynik = a * b;
                        Console.WriteLine(wynik);
                    }
                    break;
                case "/":
                    if (a == 0 || b == 0)
                    {
                        Console.WriteLine("Nie można dzielić przez 0!");
                    }
                    else
                    {
                        wynik = a / b;
                        Console.WriteLine(wynik);
                    }
                    break;
                default: Console.WriteLine("Zła operacja");
                    break;
            }
            Console.WriteLine("Wynik= " + wynik);
        }
