- 👋 Hi, I’m @Boonk8812
- 👀 I’m interested in ... Technology and more stuff about tech!
- 🌱 I’m currently learning ... school.
- 💞️ I’m looking to collaborate on ... tech and Minecraft and software and hardware ad more!
- 📫 How to reach me ... Be nice and civil.
- My Discord Server and my Planet Minecraft:

 Planet Minecraft Community (PMC): https://www.planetminecraft.com/member/declanmurphy2023/
 Canonical Launchpad: https://launchpad.net/~declanminer86
 Discord: https://discord.gg/qAGq6Axw76

- My friend's Discord: wheezytheweasel#3486

<!---
Boonk8812/Boonk8812 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
Oh and here is a calculator script in c#:
```c
using System;

namespace Calculator
{
    class Program
    {
        static void Main(string[] args)
        {
            try
            {
                Console.WriteLine("Enter the first number:");
                double num1 = Convert.ToDouble(Console.ReadLine());

                Console.WriteLine("Enter the second number:");
                double num2 = Convert.ToDouble(Console.ReadLine());

                Console.WriteLine("Enter the operation (+, -, *, /):");
                char operation = Convert.ToChar(Console.ReadLine());

                double result = 0;

                switch (operation)
                {
                    case '+':
                        result = num1 + num2;
                        break;
                    case '-':
                        result = num1 - num2;
                        break;
                    case '*':
                        result = num1 * num2;
                        break;
                    case '/':
                        if (num2 != 0)
                        {
                            result = num1 / num2;
                        }
                        else
                        {
                            throw new DivideByZeroException("Cannot divide by zero.");
                        }
                        break;
                    default:
                        throw new ArgumentException("Invalid operation.");
                }

                Console.WriteLine("Result: " + result);
            }
            catch (FormatException)
            {
                Console.WriteLine("Invalid input. Please enter valid numbers.");
            }
            catch (DivideByZeroException ex)
            {
                Console.WriteLine(ex.Message);
            }
            catch (ArgumentException ex)
            {
                Console.WriteLine(ex.Message);
            }
            catch (Exception)
            {
                Console.WriteLine("An error occurred. Please try again.");
            }
        }
    }
}
```
