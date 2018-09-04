using System;

namespace To_do_list
{
     class Program
     {

        static void Main(string[] args)
        {
            Choise();
        }
        static void Choise() { 
             string option;
             do
             {
                Console.WriteLine("To Do list" + "\n");

                Console.Write("1.Edit\n");// Text = text.Rename(ind);
                Console.Write("2.Add\n");
                Console.Write("3.Delete\n"); // text = text.Remove(ind);
                Console.Write("4.Swow all\n" + "\n");

                Console.WriteLine("Choose your option..." + "\n");

                option = Console.ReadLine();
                 switch (option)
                 {
                     case "1":
                         Console.WriteLine("Edit");
                         Console.Clear();
                         break;
                     case "2":
                         Console.Clear();
                        Console.WriteLine("Add your note...\n");
                       Add();
                        Console.WriteLine("\n" + "You have added note\n");
                        Console.WriteLine("Write anything to continue...\n");
                        Console.ReadLine();
                        Console.Clear();
                        Choise();
                        break;
                     case "3":
                         Console.WriteLine("Delete");
                         Console.Clear();
                         break;
                     case "4":
                        Console.Clear();
                        Console.WriteLine("Show All");
                       // Notes();
                        break; 
                     default:
                        option = "default";
                        Console.Clear();
                        break;
                 }
             } while (option == "default" );
            

            Console.ReadKey();
    }
        static void Add()
        {
           string Note = Console.ReadLine();
            //string Note = Notes();
           
        }
        /*
        static void Notes()
        {
            Console.WriteLine(Note);
        }*/

    }
}
