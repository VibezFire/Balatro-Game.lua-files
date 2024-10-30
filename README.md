# Balatro-Game.lua-files
From reddit:
This is one of the few games that I've really latched onto enough, and absolutely love the base game. HOWEVER, if you're like me and wondered "man, I wish I could mod this game, but I have a Mac, and it's usually impossible to do that kind of thing" you've stumbled onto the right post! 

Disclaimer: DO AT YOUR OWN RISK, I do not claim to be a pro at coding, and I barely found a method that worked for me. editing the game.lua file can BREAK the game if not done correctly. if you understand this risk, here are some steps to "hack" the game:
1. Go into the Hard disk (if you don't already have it enabled, click finder at the top, finder settings, enable Hard Disk)
2. Open the Applications folder, and find the Balatro game
3. Right click and click "Show Package contents" (this is the equivalent of Steams "Show Game Folder" button)
4. Click into the "Contents" folder, Then into the "Resources" file, Then finally into the "Game" file
5. you should see an option for a "game.lua" file. Using a preferred code/text editor (either VSCode or mac's built-in TextEdit) click into the file. this method works best with the TextEdit application.
6. This particular file has thousands of lines of code, and each line defines what a particular object in the game does. for example, it defines the different Deck parameters, like how the yellow deck gives $10, etc.
Once in this file, there are plenty of things to mess with. here are some steps to change what the yellow deck does (but this works for any deck if done correctly):
1. hit command+F and search for "backs" in the search bar and press enter. this should show a list of all of the different decks in-game, as well as all of the parameters.
2. you should see somewhere in the lines of code that it lists " name=[red, green, blue, black, yellow, etc.] deck" each of these is the initial code line for all of the decks of cards. find the "name= yellow deck"
3. there should be a line labeled "config= {dollars=10}". you can change the 10 value here to whatever number you'd like.
4. When editing this file, it may say that you "don't have permission to modify" and then it should give you an option to duplicate the game.lua file. Do this, and save the updated game.lua somewhere you can find. DON'T LOSE THE ORIGINAL game.lua FILE!!
5. replace the game.lua file with your modified game.lua file. boot up the game.
6. now you should see the game will start, and when you go to the yellow deck, it will have whatever number you set the money to!
