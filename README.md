# APCS_Szabo_Boggle

## Feb 15: Current Approach
For each word in the dictionary list (Let's use the word "Liver" as an example), initialize a boolean return as "false":
1. For each Tile, check if it matches the first letter of the given word ("L"). If so, move to Step 2.
2. Examine each neighboring Tiles to check if they match the next letter of the given word ("I"). If so, move to Step 3.
3. Mark the Tile that was just examined to indicate that one cannot return to that tile. Do Step 2 for the neighboring tile that matches.
4. Base case: If an equal number of un-returnable tiles exist as the length of the word, the word has been constructed; the boolean can be set to "true".
To accomodate the possibility of several tile combinations of "LI", for example, recursion is required.
