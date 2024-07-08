# DNA-profiling-program
This Python script analyzes a DNA sequence to identify a potential match in a database for profiling purposses
## Background
DNA is really just a sequence of molecules called nucleotides, arranged into a particular shape (a double helix). Every human cell has billions of nucleotides arranged in sequence. Each nucleotide of DNA contains one of four different bases: adenine (A), cytosine (C), guanine (G), or thymine (T). Some portions of this sequence (i.e., genome) are the same, or at least very similar, across almost all humans, but other portions of the sequence have a higher genetic diversity and thus vary more across the population.

## Functionality<br>
Reads a database of known DNA profiles from a CSV file. The CSV file should have:<br>

A header row containing the name of each Short Tandem Repeat (STR) sequence analyzed.<br>
Subsequent rows containing individual profiles, with the first column specifying the person's name and the remaining columns containing the number of repeats found for each STR in that person's DNA.<br>
Reads a DNA sequence from a separate text file.<br>

Analyzes the DNA sequence for the longest run of each STR sequence listed in the database.<br>

Compares the number of repeats found in the DNA sequence for each STR to the corresponding values in the database profiles.<br>

If a profile in the database matches the number of repeats found for all STRs in the DNA sequence, the script prints the name of that person as a potential match.<br>

Otherwise, the script prints "No match" indicating no match was found in the database.<br>
