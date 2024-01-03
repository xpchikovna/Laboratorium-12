public static class Program
{
    public static void Main(string[] args)
    {
        Console.Write("Wprowadź początek zakresy: ");
        int pocz = Int32.Parse(Console.ReadLine());
        Console.Write("Wprowadź konies zakresy: ");
        int kon = Int32.Parse(Console.ReadLine());
        for (int i = pocz; i <= kon; i++)
        {
            int sil = Silnia(i);
            Console.WriteLine($"{i}! = {sil}");
        }
    }
    static int Silnia(int n)
    {
        if (n == 1)
        { 
            return 1; 
        }
        return n * Silnia(n - 1);
    }
}
