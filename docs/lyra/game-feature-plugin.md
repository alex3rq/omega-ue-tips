# Game Features Plugin

> Game Features allows developers to create **modular** and **plug-and-play content** for their games.

## Features

### Modular Content Creation

Instead of modifying the core game code, you can build functionalities as separate **plugins**. These plugins are self-contained units with their own assets, data, and logic.
This modular approach promotes cleaner code organization and easier maintenance, especially for large projects.

### Plug-and-Play Functionality

Game Features allows you to **enable or disable** these plugins at any time during development or even within the final game. This offers a high degree of flexibility.
You can add new features, gameplay mechanics, or even entire game modes without touching the core game code. This simplifies iteration and testing of new ideas.

## Benefits of Using Game Features

* **Improved Code Maintainability:** By separating functionalities into modules, the codebase becomes easier to understand, modify, and debug.
* **Faster Development:** New features can be developed and integrated into the game more efficiently.
* **Content Experimentation:** The ability to easily enable and disable features allows for quicker testing and iteration during development.
* **Potential for Marketplace Assets:** Developers can create and share Game Feature plugins as Marketplace assets, promoting reusability and collaboration within the Unreal Engine community.

## Create a Game Feature plugin

1. First go to `Edit > Plugins`.
2. Click on the `+Add` button.
3. Select `Game Feature (with C++)` from the list.
4. Give your plugin a `name`.
5. Click the `Create plugin` button.

![Create new plugin](lyra-images/create-new-plugin.jpg)

## Setting up the Game Feature

1. Under `Actions` add an item to `Add Input Mapping`.
2. Expand the item and select `IMC_Default`.
3. Next under `Game Feature > Asset Manager` add 3 elements.
4. Expand the first one and set it to:
   * Primary Asset Type: `LyraExperienceDefinition`
   * Asset Base Clas: `LyraExperienceDefinition`
   * Has Blueprint Classes: [x] checked
   * Directories: Add an entry and set it to your plugin's folder.
5. Next set it to:
   * Primary Asset Type: `LyraUserFacingExperienceDefinition`
   * Asset Base Clas: `LyraUserFacingExperienceDefinition`
   * Has Blueprint Classes: [x] checked
   * Directories: Add an entry and set it to your plugin's folder.
6. Lastly for the Map set it to:
   * Primary Asset Type: `Map`
   * Asset Base Clas: `World`
   * Directories: Add an entry and set it to the `Maps` folder inside your plugin.

> **Note:** You can set these before creating them but be sure to save them in the correct location.

## Resources

[Unreal official documentation for Game Features and Modular Gameplay](https://docs.unrealengine.com/5.3/en-US/game-features-and-modular-gameplay-in-unreal-engine/)

[Bastian Dev - YouTube > Lyra Map creation](https://youtu.be/hO8OWLWLD6o?si=Z_qkSje1nfb1ndEW&t=151s)
