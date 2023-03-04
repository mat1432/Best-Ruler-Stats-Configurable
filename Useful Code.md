# Generate More Options Scripts
*Made by mat1432 [Steam](https://steamcommunity.com/id/mat1432/) [GitHub](https://github.com/mat1432/)*
## Generate Options
Compile and run with your chosen tool. Though for quick use, I suggest https://www.w3schools.com/ tryit interpreter
### C#
https://www.w3schools.com/cs/trycs.php?filename=demo_compiler
```c#
using System;

namespace EU4_Generation_Code
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.Write("Start Value (number): ");
            int start = Convert.ToInt32(Console.ReadLine());
            Console.Write("\nEnd Value (number): ");
            int end = Convert.ToInt32(Console.ReadLine());
            Console.Write("\nShow only options up to max skill (yes/no): ");
            var maxskill = Console.ReadLine();

            Console.WriteLine("\n");
            Console.WriteLine("");
            Console.WriteLine("Options Code\t\tevents/brsc_events.txt");
            for (int x = start; x <= end; x++)
            {
                Console.WriteLine("");
                Console.WriteLine("option = {");
                Console.WriteLine("\tname = \"brs_change_" + x + "\"");
                if (x == 0 || maxskill != "yes")
                {
                    Console.WriteLine("\ttrigger = { NOT = { brs_check_target_setup = { a=" + x + " b=" + (x + 1) + " } } }");
                }
                else
                {
                    Console.WriteLine("\ttrigger = {");
                    Console.WriteLine("\t\tAND = {");
                    Console.WriteLine("\t\t\tbrs_check_maxskill = { b=" + (x + 1) + " }");
                    Console.WriteLine("\t\t\tNOT = { brs_check_target_setup = { a=" + x + " b=" + (x + 1) + " } }");
                    Console.WriteLine("\t\t}");
                    Console.WriteLine("\t}");
                }
                Console.WriteLine("\tbrs_set_target = { a=" + x + " }");
                Console.WriteLine("\thidden_effect = { country_event = { id = brs.1010 } }");
                Console.WriteLine("\ttooltip = { country_event = { id = brs.10 } }");
                Console.WriteLine("}");
                Console.WriteLine("");
                Console.WriteLine("option = {");
                Console.WriteLine("\tname = \"brs_change_" + x + "\"");
                if (x == 0 || maxskill != "yes")
                {
                    Console.WriteLine("\ttrigger = { brs_check_target_setup = { a=" + x + " b=" + (x + 1) + " } }");
                }
                else
                {
                    Console.WriteLine("\ttrigger = {");
                    Console.WriteLine("\t\tAND = {");
                    Console.WriteLine("\t\t\tbrs_check_maxskill = { b=" + (x + 1) + " }");
                    Console.WriteLine("\t\t\tbrs_check_target_setup = { a=" + x + " b=" + (x + 1) + " }");
                    Console.WriteLine("\t\t}");
                    Console.WriteLine("\t}");
                }
                Console.WriteLine("\thighlight = yes");
                Console.WriteLine("\tbrs_set_target = { a=" + x + " }");
                Console.WriteLine("\thidden_effect = { country_event = { id = brs.1010 } }");
                Console.WriteLine("\ttooltip = { country_event = { id = brs.10 } }");
                Console.WriteLine("}");
            }

            Console.WriteLine("");
            Console.WriteLine("");
            Console.WriteLine("Effect Tooltips\t\tbrsc_effect_tooltips_l_english.yml");
            for (int x = start; x <= end; x++)
            {
                Console.WriteLine(" brs_set_target_" + x + "_tt: \"§GSet Stat Target§! to §Y" + x + "§!\"");
            }

            Console.WriteLine("");
            Console.WriteLine("");
            Console.WriteLine("Events\t\t\tbrsc_events_l_english.yml");
            for (int x = start; x <= end; x++)
            {
                Console.WriteLine(" brs_change_" + x + ": \"Set to §Y" + x + "§!\"");
            }

            Console.WriteLine("");
            Console.WriteLine("");
            Console.WriteLine("Trigger Tooltips\tbrsc_trigger_tooltips_l_english");
            for (int x = start; x <= end; x++)
            {
                Console.WriteLine(" brs_has_target_" + x + "_tt: \"Has Stat Target §Y" + x + "§!\"");
            }

            Console.WriteLine("");
            Console.WriteLine("");
            var cc = new statmap(end);
            Console.WriteLine("Consort Helper\tcommon/scripted_effects/brsc_scripted_effects.txt");
            Console.WriteLine("if = { limit = { check_variable = { which = ruler_skill value = " + cc.buffer + " } } change_consort_$value$ = " + cc.buffer + " }");
            for (int i = cc.buffer - 1; i >= cc.floor; i--)
            {
                Console.WriteLine("else_if = { limit = { check_variable = { which = ruler_skill value = " + i + " } } change_consort_$value$ = " + i + " }");
            }
        }
    }

    internal class statmap
    {
        public int value;

        public statmap(int end)
        {
            value = end;
        }

        public int buffer
        {
            get {
                if (value <= 20)
                {
                    return value + 6;
                }
                else if (value <= 40)
                {
                    return value + 10;
                }
                else if (value <= 70)
                {
                    return value + 15;
                }
                else if (value <= 100)
                {
                    return value + 20;
                }
                else if (value <= 200)
                {
                    return value + 30;
                }
                else if (value <= 500)
                {
                    return value + 40;
                }
                else
                {
                    return value + 50;
                }
            }
        }
        public int floor
        {
            get {
                if (value >= 500)
                {
                    return 200;
                }
                else if (value >= 200)
                {
                    return 100;
                }
                else if (value >= 100)
                {
                    return 70;
                }
                else if (value >= 70)
                {
                    return 40;
                }
                else if (value >= 40)
                {
                    return 20;
                }
                else
                {
                    return 0;
                }
            }
        }
    }
}
```