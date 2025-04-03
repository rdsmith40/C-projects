using System;
using System.Linq;

class CharacterCounter
{
    static void Main()
    {
        Console.WriteLine("Enter a string:");
        string input = Console.ReadLine();

        var charCounts = input
            .Where(char.IsLetter) // Filter alphabetic characters
            .Select(char.ToLower) // Convert to lowercase
            .GroupBy(c => c) // Group by character
            .ToDictionary(g => g.Key, g => g.Count()); // Count occurrences

        Console.WriteLine("Character counts:");
        foreach (var pair in charCounts)
        {
            Console.WriteLine($"{pair.Key}: {pair.Value}");
        }
    }
}
