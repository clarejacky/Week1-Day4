# Week 1 day 4 - Function Prototyping
##Assignment Overview

In this assignment you will create your own Git repository, and learn about Objects and Function Prototypes. To do this you will be creating a very simple application for the recording of statistics for players and monsters in the game Dungeon and Dragons, and storing those in an array. 

**Instructions:**

- Create a brand new repository under your GitHub account. Give it a descriptive name such as "Week1-Day4", and a description such as "Week 1 day 4 - Function Prototyping".
- Create a new HTML file named `index.html`.
- Inside of the HTML file, create a simple HTML document. Add the following to the document:
    * A title, description and author metadata.
    * An HTML label with `Name:` as the text.
    * A textbox (an HTML input of type `text`) that has an id of `name`. 
    * Create six more label/textboxes for the six monster/player statistics: Strength, Dexterity, Constitution, Wisdom, Intelligence and Charisma. Be sure to give the text boxes unique IDs as well.
    * A third label with `Player Class (Optional)`.
    * A textbox with the id `class`.
    * A button with the text `Add Player/Monster to Records` and an the id `addMonster`.
    * Finally, add a table with eight columns, with the headers `Name`, `Strength`, `Dexterity`, `Constitution`, `Wisdom`, `Intelligence`, `Charisma` and `Player Class (Optional)`.
- Create a new CSS file named `styles.css`.
    * Add a reference to this file in `index.html`.
    * Add any styles you want to make this app look nicer. Look at W3 School's [CSS Tables](http://www.w3schools.com/css/css_table.asp). 
- Create a new JavaScript file named `app.js`.
    * Add a reference to this file in `index.html`.
    * Create an object called `Monster` that has the properties `name`, `strength`, `dexterity`, `constitution`, `wisdom`, `intelligence`, and `charisma`.
    * Create an object called `Player` that inherits from `Monster`, and has the additional property `playerClass`.
    * Create a constructor for `Player` as well as a prototype to correctly pass reference to `this`.
    * Create an empty array to serve as storage.
    * Next, write an function that will act as a click handler for the button. It should call the appropriate constructor using the values the user typed into the textboxes, add the object to the array, append it to the table for visual representation, and clear out the textboxes. Hint: Use `document.getElementById('addMonster').addEventListener('click', <functionNameGoesHere>);`
- Add a prototypical function to the Monster class called `Attack`. When called, it will roll a 20 sided die and add that to the object's strength value. Hint: return `Math.floor(Math.random() * 20) + 1` added to the object's strength value. 
    -For the player class override the function using prototypes to return the same thing, but use dexterity value instead of strength.
- Make the player/monster's name a hyperlink or button, and when it is clicked it should output the value of `Monster.Attack()` or `Player.Attack()` to an alert or to the DOM. Use the array and the objects in the array, looking them up from the array using the name.
 
## Bonus:

- Instead of using a textbox for Player Class, try creating a radio button (HTML input of type `radio`) that has the values `None`, `Cleric`, `Fighter`, `Rogue`, and `Wizard`. 
- Change the application to use your favorite RPG's system, classes, add in other stats like race, hit point, or what ever!
  
####Be sure to commit your changes to your development branch frequently!
=======
# Week 1 Weekend Challenge - Function Prototyping
Group members: Clare, Michael, Michelle, Rom

### A short explanation of RPG terminology from a gamer (Rom)

In an RPG, short for role-playing game, you play a **class** like a cleric, who heals injured people, or a fighter, who beats up monsters. The class represents your abilities and role in the game. Our weekend assignment is basically to build a miniature RPG, which I think is pretty cool, but it might not be everyone's cup of tea.

Other RPG terms that show up in the text:

- Strength, Dexterity, Constitution, Wisdom, Intelligence, and Charisma are player **statistics**. They represent aspects of the player's character, such as how physically strong they are (strength), how much damage they can take before becoming unconscious (constitution), and how likeable they are (charisma).
- Races, as mentioned in the bonus question, are fantasy creatures like **elves** and **dwarves**. And humans, in the context of these systems.
- Hit points (HP) are a numeric representation of how much health your character has. Typically, when your HP reaches 0, you die or fall unconscious.

We don't have to include all these things, but I thought I'd write an explanation so everyone is clear on what they mean, so we're all on the same page.

Check out Rom's project and contributors here: https://github.com/romstevens/prime_week1_day4
