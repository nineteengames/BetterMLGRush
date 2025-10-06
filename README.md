🚀 MLGRush Plugin for Minecraft 1.8.9

📝 Overview

This MLGRush plugin implements the popular minigame mode often used for BedWars training. The goal is to destroy the opponent's "bed" by rapidly building bridges and knocking the enemy off with a knockback stick. The plugin is specifically developed for Minecraft Version 1.8.9 (Spigot/Bukkit).

This repository contains the full source code and is released to the community for maintenance, bug fixes, and future development. I will no longer be actively maintaining or developing this project.

✨ Key Features

    Dedicated 1.8.9 Support: Optimized for the classic 1.8 PvP experience.

    Arena System: Easy setup for multiple arenas (e.g., 1v1).

    Dynamic Gameplay: Instant respawn, automatic block reset, includes knockback stick and sandstone inventory items.

    Lobby/Queue: Players can join the queue or challenge others.

    Statistics System: [Mention if stats are included (MySQL/Flatfile): e.g., Tracks Kills, Deaths, Wins, and Winrate.]

    Configurable: [Mention what is customizable: e.g., Messages, inventory layouts, win conditions.]

🛠️ Installation & Setup (For Server Owners)

Requirements

    A Minecraft server (Spigot, Paper, or a fork)

    Minecraft Version: 1.8.9

    Java 8

Plugin Installation

    Download the latest MLGRush.jar file from https://www.spigotmc.org/resources/better-mlgrush.116870/.

    Stop your Minecraft server.

    Place the MLGRush.jar file into your server's plugins/ folder.

    Start the server to generate the initial configuration files.

Arena Setup (Admin Commands)

Ensure you have the necessary permission (mlgrush.admin or Operator privileges).

    Set Lobby: Teleport to the main lobby location.

    /mlgrush setlobby

    Create Arena:

    /mlgrush create <arenaName>

    Set Spawn Points: Teleport to the respective spawn points in the arena.

    /mlgrush setspawn <arenaName> <red/blue>

    Set Bed Locations: Place the block foundation where the beds should appear.

    /mlgrush setbed <arenaName> <red/blue>

    Enable Arena: The arena must be enabled after setup.

    /mlgrush enable <arenaName>

⚙️ Commands and Permissions

Command	Description	Permission (Optional)
/mlgrush join	Join the game queue.	None
/mlgrush leave	Leave the current game or queue.	None
/mlgrush stats [Player]	Show your own or another player's statistics.	None
/mlgrush build	Enable/Disable build mode (for Admins/Staff).	mlgrush.build
/mlgrush setup	Open the setup GUI (if applicable).	mlgrush.admin
/mlgrush setlobby	Set the global lobby spawn.	mlgrush.admin

💻 For Developers (Building the Source)

This section explains how to import the source code and compile the plugin to apply your own bug fixes or features.

Requirements

    Java Development Kit (JDK) 8

    Git

    Maven (or an IDE like IntelliJ/Eclipse with integrated Maven support)

1. Clone the Repository

Clone the code locally to your machine:
Bash

git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME

2. Compiling (Building)

Execute the following command in the project's root directory, where the pom.xml file is located:
Bash

mvn clean package

    clean: Deletes previous build artifacts.

    package: Compiles the source code and creates the final MLGRush.jar file.

The compiled plugin file will be located in the /target/ folder.

🤝 Contributing and Bugfixes

Since the project is no longer actively maintained by me, I encourage Pull Requests (PRs) from the community that introduce bug fixes or small, relevant improvements.

    Fork this repository.

    Create a branch for your fix (git checkout -b bugfix/your-description).

    Implement the fix and commit your changes.

    Create a Pull Request with a clear description of your bugfix.

📄 License

This project is licensed under the MIT License. See the LICENSE file for more details.
