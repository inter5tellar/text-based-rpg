# text-based-rpg

19 .java files, 1 .txt file

Created using jdk-14 and VSCode.

This program is very much a work in progress. There are many aspects that have been inserted for future use that are not completely functional yet, and there are also many aspects currently in place for testing purposes that will be removed eventually. I will update this repository from time to time whenever I make significant progress on it. The purpose of uploading is to receive critique/suggestions/corrections from other members of the coding community.

Note: notes.txt are notes to myself about what I'm working on/need to do and code snippets I want to save. I am including it so others can know what I've already marked as needing to be edited before suggesting it.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Current Class Hierarchy:

  **App.java** - Contains the main method which creates an instance of Adventurer.java to act as the 'player', then calls the 'event' methods which make up the 'adventure'.
  
  **Adventurer.java** - Describes the 'player', their attributes and which actions they can take in the 'adventure'.
  
  **LootList.java** - Holds the ArrayList which contains 1 each of all of the items in the program which can potentially be obtained by the Adventurer. (Created for future use)
  
  **Item.java**
  ```
  -> Consumable.java
      * May delete and extend Consumable directly. These classes previously had unique methods but I reorganized.
      * Keeping for now as I add to the program in case they need unique methods or fields in the future.
      -> Food.java
      -> Beverage.java
      -> Magics.java
          -> MinorHealingPotion.java
          -> MinorManaPotion.java
  -> Container.java
      -> Chest.java
      -> DeadBody.java
  -> Currency.java
      -> Gold.java
      -> Token.java
  -> Wearable.java
  ```
  
  **Enemy.java**
  ```
      -> Goblin.java
  ```
