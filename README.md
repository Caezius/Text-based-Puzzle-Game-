# Text-based Puzzle-Game
A puzzle game similar to the one with sharply dressed waifus by Vanripper!
Uses text and arrays to display the visuals. 

General structure:

1. The user selects a level by inputting a number (the level number).
2. The level is found in an array of levels, and generateObjects(level_array) is run.
3. for(): each index in the level_array array, if there should be an object at that index/coordinate, a Rock() object is initialized, with x and y attributes. The x attribute will be set to the column the coordinate is in, and the y position set to the row the coordinate is in. Then the Rock() object is also assigned a value to its Id attribute, and then the object is added to the objects_in_Play array.
4. The level_array itself is then printed to the screen. 

6. The user is then prompted to input a character to represent their avatar. If more than one character is put in, the first non-whitespace character will be used as the user's avatar.
7. A Player() object is initialized, using their avatar value as an attribute.
8. The Player() object is given the x and y positions associated with the level.
9. The user's Id attribute will be set to their avatar string instead of a number. This helps to distinguish the player from the rest of the Rock()s later.

10. The function synthesizeMap(objects_in_Play); is run. 
11. The returned Value is printed to the screen.

12. The game starts. While the user does not enter the sentinel (the string "quit") the program will:
13. Take a move from the user-either the arrow presses on the keyboard, W/A/S/D, or the words "up", "down", "left", "right" (not case sensitive)
14. 


Bonus features:
1. Use matplotlib or some sort of 


generateObjects(level_array)
: generateObjects(level_array) takes a 2-D array, which represents all the coordinates in the level. The level array represents these positions as strings. For each position there will be a whitespace ("") value for an empty coordinate or an "O" (or some string value) to represent an object being at that position.
