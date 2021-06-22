using System;
using System.IO;

namespace JavaProject
{
    class Program
    {
        static void Main(string[] args)
            
        {
            string FirstFile = "First.txt";
            string text1 = "ABCDEFGHIJKLM";
            File.AppendAllText(FirstFile, text1);
            System.Console.WriteLine("Contents of the first file is - " + text1);

            
            string SecondFile = "Second.txt";
            string text2 = "NOPQRSTUVWXYZ";
            File.AppendAllText(SecondFile, text2);
            System.Console.WriteLine("Contents of the second file is - " + text2);

            string ThirdFile = "Third.txt";
            string text3 = text1 + text2;
            File.AppendAllText(ThirdFile, text3);
            System.Console.WriteLine("Contents of third file - " + text3);
            System.Console.WriteLine("The length of the characters in the Third File is - " + text3.Length);

            string FourthFile = "Fourth.txt";
            int square = text3.Length * text3.Length;  //to square a number , multiply it by itself.
            File.AppendAllText(FourthFile, Convert.ToString(square));
            System.Console.WriteLine("The square of the length of the characters is  - " + square);

        }   
    }
}
