**Milestones:** 
- 10 stars. ✅
- 50 stars. ✅
- 69 stars. ✅
- 100 stars. ✅ ([ArchGryphon9362](https://github.com/ArchGryphon9362)).
- 250 stars. ❌
- 420 stars. ❌
- 1000 stars. ❌

---
**⚠️ Warning ⚠️** 

These tools are made for educational purposes. **By using these tools, you agree that you hold responsibility and accountability of any consequences caused by your actions.**

---
# Discord Raidkit

[Introduction](#discord-raidkit) | [Anubis Guide](#anubis-guide) | [Qetesh Guide](#qetesh-guide) | [Osiris Guide](#osiris-guide) | [Ghost Guide](#ghost-guide)
![Discord Raidkit v1.5.4 Image](https://media.discordapp.net/attachments/833694868248985673/834936090086735892/image0.jpg?width=1440&height=232)
Discord Raidkit is a free collection of programs designed raid servers and accounts as effectively as possible. The following is a list of all the programs currently included:

- **Anubis** is a discord multi-purpose nuker bot. However, unlike several other nuker bots, Anubis is designed to resemble a trojan horse by including many helpful features, with malicious commands hidden inside.  

- **Qetesh** is a custom version of Anubis, designed to be a trojan of a porn bot - it has the full capabilities of a porn bot with the same hidden commands of Anubis, allowing you to prey on those lost within their own lust (which is 99% of the discord community).
- **Osiris** is a redesign of the "Jajaja Account Nuker" created by [@azaelgg](https://github.com/azaelgg) (permission granted). It contains a fresh new look and provides a few usability improvements, as the original had some issues.

- **Ghost** is a discord token grabber made by contributer [@ytsix](https://github.com/ytsix).


These tools' full potential will be discussed in seperate guides further down the README.md file, along with an analysis on how they work and tips for getting the best results.


---
### Installation Guide
[Introduction](#discord-raidkit) | [Anubis Guide](#anubis-guide) | [Qetesh Guide](#qetesh-guide) | [Osiris Guide](#osiris-guide) | [Ghost Guide](#ghost-guide)

**(Currently working on update video guide).**


In order to make the most of this installation guide, please follow the instructions *exactly* as they say.
1. These tools require Python, which can be downloaded [here.](https://www.python.org/downloads/release/python-390/) When installing python, remember to check, "Add Python to PATH" - **this is vital**.

2. **Anubis** requires PostreSQL, which can be downloaded [here.](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads) When installing PostreSQL, do not uncheck any of the checkboxes except the checkbox asking to install Stack Builder. Furthermore, when installing PostreSQL, it will ask you to create a master password. **This password is important, remember it.** **If you have no plans on using the Anubis tool, then you can skip step three.** Step three will cover how to set up PostreSQL for Anubis after installed.

3. Search for **pgAdmin 4** in the windows search and run it. Enter the master password whenever it prompts you to enter it. Right click 'databases' at the side and create a new database named `levels_db`. **It must be named levels_db or it fails.** Within the side-explorer for the new, levels_db database, right click 'tables' and create a new table. Name the table `users`. **Again, all naming in this guide must be exact.** Then, move to the columns section. Here, you want to create four new columns; `user_id` should be set to the 'character_varying' datatype and 'Not NULL?'' should be set to yes; `guild_id` should be set to the 'character_varying' datatype as well - you must leave 'Not NULL?' alone for this column and the next two; `lvl` should be set to the 'integer' datatype; `xp` should be set to the 'integer' datatype as well. After these four columns are created, you can click 'save' to save the table, then exit pgAdmin 4.

4. To download the tools, visit the [releases page.](https://github.com/Catterall/discord-pedo-hunting-tools/releases)

5. After downloading the tools, remember to run `install_requirements.cmd` - it will install all Python requirements needed to use the tools without errors.

6. **If you wish to use Osiris, you must follow this extra step:** 
 Download this specific chrome browser version [here.](https://drive.google.com/file/d/1qg-cjHqEoUODARL6hL9-IT7OrjsSq-wZ/view?usp=sharing) After downloading the zip file, place it inside the Osiris folder and extract it. There should now be a browser folder within the Osiris folder, which will be used by Osiris. At this point, you can delete the zip file. If you've been following this guide correctly, you should now be ready to use the tools (for those of you wondering, I no longer use LFS/Cloning because 10GB of free broadband transfer a month is nothing). 

---
### Anubis Guide
[Introduction](#discord-raidkit) | [Anubis Guide](#anubis-guide) | [Qetesh Guide](#qetesh-guide) | [Osiris Guide](#osiris-guide) | [Ghost Guide](#ghost-guide)

To first use Anubis, run the `main.py` file. You should be greeted with a warning screen - simply press the return (enter) key. You should now notice a new file, named `run_settings.json`. Within this file, there are three settings that you must determine before using Anubis (Open the JSON file with notepad if you have no default program):
1. Replace the default password text with your PostreSQL master password.
2. You must set a bot prefix. Any prefix will do, but try to avoid exceptionally common prefixes, such as !
3. Replace the default token text with your discord bot's token.

Remember to save the file! What's that? You don't currently have a discord bot? Well, luckily for you, setting one up is extremely easy and does not require any downloads. 

Head to the discord developers page [here](https://www.discord.com/developers) and click, "New Application". Name the application with the same name that you will name your bot. After creating the application, look to the left side and click 'Bot'. From here, click 'Add Bot'. Before copying the token, first turn on both privileged gateway intents - you can now copy your bots token and place it in the run_settings.json file. To get the invite link, head to the OAuth2 section, scroll down and check the "Bot" checkbox, then check the "Administrator" checkbox underneath - the link generated will allow anyone to invite the bot and will give the bot administrator permissions.

##### **Using Anubis:**
Anubis works in a simple way. Each of the malicious commands, only visible to you, is diplayed on the main terminal screen. A command in Anubis is made up of two or three things:
1. **The prefix and command name**: For example, `a!nuke`.

2. **The command code**: For example, `2812`. This is to prevent people testing if the bot is this bot immediatly by just running a command found here.
3. **The command arguments**: For example, `<message>`. These are used by the command to carry out their task and can be used by simply appending it to the end of a command (e.g. `a!spam 2812 hello!` - `hello!` is the `<message>` parameter).

Anubis has the following commands (the commands will be represented here with a prefix of 'a!'):
- `a!leave <code> <server>`: This command will make Anubis leave a given server (`<server>`).

- `a!mass_leave <code>`: This command will make Anubis leave every server it is currently in.

- `a!mass_nick <code> <nickname>`: This command will give every member in any given server a nickname of your choice.

- `a!mass_dm <code> <message>`: This command will make Anubis message everyone in any given server with a given message (`<message>`).

- `a!spam <code> <message>`: This command will make Anubis spam every text channel in any given server with a given message (`<message>`) until stopped.

- `a!cpurge <code>`: This command will delete every communication channel in any given server.

- `a!admin <code> <role_name>`: This command will grant you, in any given server, an administrator role with a given name (`<role_name>`).

- `a!nuke <code>`: This command will make Anubis ban all members, delete all channels, delete all roles and delete all of the emojis in any given server.

- `a!mass_nuke <code>`: This command will make Anubis run the nuke command in any server it is in (*one by one, not at the same time*).

- `a!raid <code> <role_name> <nickname> <channel_name> <channel_num> <message>`: This command will make Anubis create a new role with a given name (`<role_name>`), assign all members in any given server with that role, then run the nickname command with a given nickname (`<nickname>`), then create `<channel_num>` number of channels (use an integer) with a given name (`<chanel_name>`) then run the spam command on said channels with a given message (`<message>`).

All of these commands are usable without permissions, as long as the bot is in the server. However, there are some important rules to take note of:
- When the bot is invited, it will create its own role. In order for the bot to directly affect a member (mass_dm, nuke, mass_nuke, raid) its role must be above any given member's role. **TL;DR, move the bots role as high as possible by utilising the admin command to give you the permissions to do so and/or by manipulating the higher members to do it for you.**

- Commands must be used like regular commands - in other words, in a text channel. Pretty much every server has a text channel, although it is best to find one that your sure no one is currently watching. Commands will delete themselves after being entered to help you go further undetected. 

"**But Catterall!**" You shout, "**However will I convince people to add the bot?!**" Well, it's up to you. You can try bribing, you can try bargaining, you can create senses of emergancy - anything, just don't be *too* over-the-top. Remember, whilst you will spend your time reading their psychology, they'll be reading you.

However, there *are* a few resources I haved provided in a Social Engineering folder to help you gain **trust**, the most important thing to possses.
- Multiple .txt files containing all the bots code without any malicious functions.

- A random image of a database screenshot. This is in-case the question the somewhat lack-luster 'add_db' fake command; show them this and they might believe it *more* (Personally, I've never had this occur to me, but I guess it's there if it does).

If word ever gets out about this bot, note that you can always tweak the code itself to make it appear different - the only thing that is needed is some basic Python knowledge. However, if you are to release your own custom made version, please credit me.

---
### Qetesh Guide
[Introduction](#discord-raidkit) | [Anubis Guide](#anubis-guide) | [Qetesh Guide](#qetesh-guide) | [Osiris Guide](#osiris-guide) | [Ghost Guide](#ghost-guide)

To first use Qetesh, run the `main.py` file. You should be greeted with a warning screen - simply press the return (enter) key. You should now notice a new file, named `run_settings.json`. Within this file, there are two settings that you must determine before using Qetesh (Open the JSON file with notepad if you have no default program):

1. You must set a bot prefix. Any prefix will do, but try to avoid common prefixes, such as `!`.
2. Replace the default token text with your discord bot's token.

Remember to save the file! What's that? You don't currently have a discord bot? Well, luckily for you, setting one up is extremely easy and does not require any downloads. 

Head to the discord developers page [here](https://www.discord.com/developers) and click, "New Application". Name the application with the same name that you will name your bot. After creating the application, look to the left side and click 'Bot'. From here, click 'Add Bot'. Before copying the token, first turn on both privileged gateway intents - you can now copy your bots token and place it in the run_settings.json file. To get the invite link, head to the OAuth2 section, scroll down and check the "Bot" checkbox, then check the "Administrator" checkbox underneath - the link generated will allow anyone to invite the bot and will give the bot administrator permissions.

##### **Using Qetesh:**
Qetesh works in a simple way. Each of the malicious commands, only visible to you, is diplayed on the main terminal screen. A command in Qetesh is made up of two or three things:
1. **The prefix and command name**: For example, `q!nuke`.

2. **The command code**: For example, `2812`. This is to prevent people testing if the bot is this bot immediatly by just running a command found here.
3. **The command arguments**: For example, `<message>`. These are used by the command to carry out their task and can be used by simply appending it to the end of a command (e.g. `q!spam 2812 hello!` - `hello!` is the `<message>` parameter).

Qetesh has the following commands (the commands will be represented here with a prefix of 'q!'):
- `q!leave <code> <server>`: This command will make Qetesh leave a given server (`<server>`).

- `q!mass_leave <code>`: This command will make Qetesh leave every server it is currently in.

- `q!mass_nick <code> <nickname>`: This command will give every member in any given server a nickname of your choice.

- `q!mass_dm <code> <message>`: This command will make Qetesh message everyone in any given server with a given message (`<message>`).

- `q!spam <code> <message>`: This command will make Qetesh spam every text channel in any given server with a given message (`<message>`) until stopped.

- `q!cpurge <code>`: This command will delete every communication channel in any given server.

- `q!admin <code> <role_name>`: This command will grant you, in any given server, an administrator role with a given name (`<role_name>`).

- `q!nuke <code>`: This command will make Qetesh ban all members, delete all channels, delete all roles and delete all of the emojis in any given server.

- `q!mass_nuke <code>`: This command will make Qetesh run the nuke command in any server it is in (*one by one, not at the same time*).

- `q!raid <code> <role_name> <nickname> <channel_name> <channel_num> <message>`: This command will make Qetesh create a new role with a given name (`<role_name>`), assign all members in any given server with that role, then run the nickname command with a given nickname (`<nickname>`), then create `<channel_num>` number of channels (use an integer) with a given name (`<chanel_name>`) then run the spam command on said channels with a given message (`<message>`).

All of these commands are usable without permissions, as long as the bot is in the server. However, there are some important rules to take note of:
- When the bot is invited, it will create its own role. In order for the bot to directly affect a member (mass_dm, nuke, mass_nuke, raid) its role must be above any given member's role. **TL;DR, move the bots role as high as possible by utilising the admin command to give you the permissions to do so and/or by manipulating the higher members to do it for you.**

- Commands must be used like regular commands - in other words, in a text channel. Pretty much every server has a text channel, although it is best to find one that your sure no one is currently watching. Commands will delete themselves after being entered to help you go further undetected. 

"**But Catterall!**" You shout, "**However will I convince people to add the bot?!**" Well, it's up to you. Unlike Anubis, Qetesh is a porn bot - meaning it will be a lot easier to convince people on discord to add it, as most people on discord are degenerates. However, if you are having trouble with trust issues, there are a few resources I haved provided in a Social Engineering folder to help you gain **trust**, the most important thing to possses.

- A .txt file containing all the bots code without any malicious functions.

- A list of every porn image's link.


If word ever gets out about this bot, note that you can always tweak the code itself to make it appear different - the only thing that is needed is some basic Python knowledge. However, if you are to release your own custom made version, please credit me.


---
### Osiris Guide
[Introduction](#discord-raidkit) | [Anubis Guide](#anubis-guide) | [Qetesh Guide](#qetesh-guide) | [Osiris Guide](#osiris-guide) | [Ghost Guide](#ghost-guide)

To use Osiris, run the `main.py` file. The usage of Osiris is straight-forward, so I'll quickly cover it, then spend most of this guide linking various resources to gaining that crucial holy-grail; the targets Auth token.
- Nuking the targets account will remove their friends, servers, change their language to symbols and, whilst active at least, flick between dark and light mode (although this stops when Osiris is exited). When Osiris asks you for the number of threads, just put **10** or something.

- Finding information on the target will display a few things, but the two most important things are the email and phone number (they may not have a phone number connected). **This discord raidkit has taken the descision to NOT include banking information/home addresses of nitro users... mainly a legal decision rather than a moral deicision, but a decision nevertheless.**
- Logging into their account will, guess what, log into their account. Just remember to give the selenium browser some time - don't just close it because it didn't login one second to reaching the login page.

---
### Ghost Guide
[Introduction](#discord-raidkit) | [Anubis Guide](#anubis-guide) | [Qetesh Guide](#qetesh-guide) | [Osiris Guide](#osiris-guide) | [Ghost Guide](#ghost-guide)

To use Ghost, edit the `main.pyw` file and place a webhook URL in Webhook class initalisation on line 40 (e.g. `hook = Webhook("https://xxx.xxx")`).

After doing this, there are several other things you can do:
- You can use a Python to executable converter to allow the user to run the program without installing Python.

- You can edit the HEX of the executable to change its file size and change its signatures to evade certain anti-malware programs (or, if you have the money, use an premium encryptor).

**As with most tools in this raidkit, it will require a little bit of social engineering!**

---
## 🌟 Remember to star this repository if it has helped you! 🌠

[Introduction](#discord-raidkit) | [Anubis Guide](#anubis-guide) | [Qetesh Guide](#qetesh-guide) | [Osiris Guide](#osiris-guide) | [Ghost Guide](#ghost-guide)
