
Moda



namespace ConsoleApp5
{
    internal class Program
    {
        static void Main(string[] args)
        {
            List<string> list = Console.ReadLine().Split(' ').ToList();

            var mode = list.GroupBy(v => v)
                .OrderByDescending(g => g.Count())
                .First()
                .Key;

        }
    }
}


