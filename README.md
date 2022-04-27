# C-Sharp-Projeleri-Ortalama-Hesaplama

Kulanıcıdan alınan derinliğe göre fibonacci serisindeki rakamların ortalamasını alıp ekrana yazdıran uygulamayı yazınız.

    using System;

    class Program {
        public static void Main (string[] args) {
          Console.WriteLine ("Lütfen fibonacci seri uzunluğunu giriniz: ");
          int len = int.Parse(Console.ReadLine());

          Console.WriteLine("Fibonacci serisinin toplamı: {0}", fibonacci(len));
          Console.ReadLine();


        }

        public static int fibonacci(int x)
            {
                if (x <= 2)
                {
                    return 1;
                }
                else
                {
                    return fibonacci(x - 1) + fibonacci(x - 2);
                }
            }
    }
