//# String-operations-in-C#

using System;

using System.Collections.Generic;

using System.Linq;

using System.Text;

namespace Practical1

{
   
   class StringDemo
    {
        static void Main(string[] args)
        {
            string str = " Welcome to Programming";
            
            int indexOf = str.IndexOf("l");
            int lastIndex = str.LastIndexOf("m");
            bool startsWith = str.StartsWith("S");
            bool endsWith = str.EndsWith("g");
            char[] ch = { 'g' };
            string[] s1 = { "to", "join", "a", "string" };
            string[] words = str.Split(' ');
            Console.WriteLine("Original String={0}", str);
            Console.WriteLine("First Index of l={0}", indexOf);
            Console.WriteLine("Last Index of m={0}", lastIndex);
            Console.WriteLine("Replace String={0}", str.Replace("m", "w"));
            Console.WriteLine("Upper Case={0}", str.ToUpper());
            Console.WriteLine("Lower Case={0}", str.ToLower());
            Console.WriteLine("Length of String={0}", str.Length);
            Console.WriteLine("Removal from string={0}", str.Remove(3));
            Console.WriteLine("Start with 'S' ={0}", startsWith);
            Console.WriteLine("Ends with g' ={0}", endsWith);
            Console.WriteLine("Using Trim={0}", str.Trim());
            Console.WriteLine("Using Trim End={0}", str.TrimEnd(ch));
            Console.WriteLine("Using Trim Start={0}", str.TrimStart(ch));
            Console.WriteLine("Join method={0}", string.Join("-", s1));
            Console.WriteLine("Substring={0}", str.Substring(13));
            Console.WriteLine("PadLeft={0}", str.PadLeft(35, '*'));
            Console.WriteLine("PadRight={0}", str.PadRight(35, '*'));
            Console.WriteLine("Insert method={0}", str.Insert(7, "#"));
            Console.WriteLine("Using Split method");
            foreach (string word in words)
            {
                Console.WriteLine(word);
            }

            Console.ReadKey();
        }
    }
}
