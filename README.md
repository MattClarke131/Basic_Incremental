# bee_Incremental
Minimal incremental game for learning purposes.
Inspired by kittens game: http://www.bloodrizer.ru/games/kittens/

Resources Used:
http://reddit.com/r/incremental_games
http://dhmholley.co.uk/incrementals.html

Thanks to:
github.com/Zack

Minimum Viable Product:
1. Button to increment pollen
2. Button to refine pollen to honey
3. Button to purchase bee
  1. Increasing bee cost
4. Bee increases pollen collected automatically

Improvements:
1. Keeping track of in game time
 	* One year should be 10-60 minutes
	1. Create nav bar at top for displaying time
	2. Create time variable in main.js
	3. Integrate time variable with window.setInterval function
2. Create an upgrade
	1. Make "Science Honey" a craftable resource
	2. Create button for crafting Science Honey"
	3. Create upgrades array to store upgrades
		* Write in a readable style
	4. Rewrite makeHoney function to check for upgrade
	5. Create a science tab
	6. Create purchase upgrade button
3. Create save feature
  1. Create save button in index.html
  2. Create save function in main.js
	3. Create clear save option on page
		* Create a confirmation for clearing save

Bugs/reformating:
1. upgrade buttons do not return if upgrades are no longer unlocked
2. rewrite updateHTML function to remove "continue;"
3. possibly break up updateHTML() function

Improvements II
1. Create wax resource
    1. Add wax resource to var game
    2. Create refine wax button
    3. Add wax gathering to workerBees
2. Create maximum amount of workerBees
    1. Create an object for structures in var game
    2. Create an honeycomb property in game.structures.
    3. Add relevant HTML for structures and honeycomb
    4. Create a make honeycomb button
    5. Set increasing cost to make honeycomb
    6. Create a "maxWorkerBees" variable
    7. Create a calculate maxWorkerBees function
    8. Create HTML for maxWorkerBees
    9. modify spawnWorkerBee function to include conditional for <= maxWorkerBees
