### Patrick  
```csharp
namespace Patrickooos
{
    public struct Patrick
    {
        string Name;
        int Age;

        List<string> Languages;

        public Patrick(string name, int age, List<string> languages)
        {
            Name = name;
            Age = age;

            Languages = languages;
        }

        public override string ToString()
        {
            Console.WriteLine($"Name: {Name}");
            Console.WriteLine($"Age: {Age}");

            Console.Write("Languages: ");

            int i = 0;

            foreach (string language in Languages)
            {
                i++;

                if (i >= 2)
                {
                    Console.WriteLine($"{language}");
                }
                else
                {
                    Console.Write($"{language} - ");
                }
            }
            return "";
        }
    }

    class Github_Profile
    {
        public static void Main(string[] args)
        {
            List<string> languages = new List<string> { "C#", "C++", "Python" };

            Patrick patrick = new Patrick("Patrick", 16, languages);

            patrick.ToString();
        }
    }
}
```
![snake gif](https://github.com/Patrickooos/Patrickooos/blob/output/github-contribution-grid-snake.svg)
