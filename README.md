# Different-Integers-Size
Just another repository
using System;
using System.Collections.Generic;
using System.Linq;
using System.Numerics;
using System.Text;
using System.Threading.Tasks;

namespace Different_Integers_Size
{
    class Program
    {
        static void Main(string[] args)
        {          
            long num;
            var line = Console.ReadLine();
            var canFitInLong = long.TryParse(line, out num);

            if (!canFitInLong)
            {
                Console.WriteLine($"{line} can't fit in any type");
                return;
            }

            Console.WriteLine($"{num} can fit in:");
            

            if (num >= sbyte.MinValue && num <= sbyte.MaxValue)
            {
                Console.WriteLine("* sbyte");
            }

            if (num >= byte.MinValue && num <= byte.MaxValue)
            {
                Console.WriteLine("* byte");
            }

            if (num >= short.MinValue && num <= short.MaxValue)
            {
                Console.WriteLine("* short");
            }

            if (num >= ushort.MinValue && num <= ushort.MaxValue)
            {
                Console.WriteLine("* ushort");
            }

            if (num >= int.MinValue && num <= int.MaxValue)
            {
                Console.WriteLine("* int");
            }

            if (num >= uint.MinValue && num <= uint.MaxValue)
            {
                Console.WriteLine("* uint");
            }

            if (num >= long.MinValue && num <= long.MaxValue)
            {
                Console.WriteLine("* long");
            }
        }
    }
}
