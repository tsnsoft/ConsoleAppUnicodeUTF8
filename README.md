# ConsoleAppUnicodeUTF8
Пример консольной программы с UTF-8 на C# (Net 6.0)

![srcreenshot](screenshot.png)

```
using System.Runtime.InteropServices;
using System.Text;

if (RuntimeInformation.IsOSPlatform(OSPlatform.Windows))
{
    Console.InputEncoding = Encoding.Unicode;
    Console.OutputEncoding = Encoding.Unicode;
}
Console.WriteLine("Замечательно! Das ist großartig! Wonderful! 精彩的！ رائع! ");
var line = Console.ReadLine();
Console.WriteLine(line);
Console.Write("Press any key to continue . . . ");
Console.ReadKey(true);

```