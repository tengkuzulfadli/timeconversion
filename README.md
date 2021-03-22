# timeconversion
using System;

namespace LabThreeTwo
{
    public class TimeConversion
    {
        static void Main(string[] args)
        {
            int totalMinutes;
            int hours;
            int minutes;

            Console.WriteLine("Please enter how many minutes have you been working on: ");
            totalMinutes = Convert.ToInt32(Console.ReadLine());

            //Console.WriteLine("You worked : " + TimeSpan.FromMinutes(totalMinutes)); //We use TimeSpan.FromMinutes to convert from minutes to hours in a format of HH:MM:SS

            {
                hours = totalMinutes / 60;
                minutes = totalMinutes % 60;

                Console.WriteLine("You worked for " + hours + " hours and " + minutes + " minutes."); //We also can use this method to convert from minutes to Hours and Minutes
            }

            Console.ReadKey();
        }
    }
}
