# Note

this is a modified version of the [EpicGamesDowngrader](https://github.com/whichtwix/EpicGamesDowngrader/tree/main) by [whichtwix](https://github.com/whichtwix)

# Download

|Version|Link|
|---|---|
|v2024.6.18|[Unavaible](link)|
|v2024.6.4|[Download](https://github.com/whichtwix/EpicGamesDowngrader/releases/download/2024.6.4-1/DowngradeEpic.ps1)|
|v2024.3.5|[Unavaible](link)|
|v2023.11.28|[Download](https://github.com/whichtwix/EpicGamesDowngrader/releases/download/2023.11.28-1/DowngradeEpic.ps1)|
|v2022.2.24|[Unavaible](link)|
|v2021.7.20|[Unavaible](link)|
|v2021.6.30|[Unavaible](link)|
|v2021.6.15|[Unavaible](link)|
|v2021.5.25|[Unavaible](link)|
|v2021.12.15|[Unavaible](link)|
I will add more versions soon

# Downgrade tool for Among Us

this repository contains a script that is used by epic players to download a older version of among us during times when mods are uncompatible
with the latest version of the game. The third party tool [legendary](https://github.com/derrod/legendary) is used.

# Common issues

1. The script may sometimes not create EpicGamesStarter.exe or it may not work due to your computer environment
   <br> Solution:
      - Download the exe from [here](https://github.com/whichtwix/EpicGamesStarter/releases/latest). <br>
      - If it does not work download the cmd file in the releases tab, place that with the legendary.exe, use that to start the game.
3. The script may instantly close.
   <br> Solution:
    - search powershell in your windows search bar and open it <br>
    - navigate to the folder the script is in, by doing for example ```cd downloads``` or ```cd desktop``` <br>
    - write ```Set-ExecutionPolicy Unrestricted -Scope Process``` and click enter <br>
    - write ```./DowngradeEpic.ps1``` and click enter <br>
4. "Access to the path '<>' is denied".
   <br> solution: If the error mentions Legendary.exe it means it cannot find the file and it likely wasnt able to be downloaded. Install it manually [here](https://github.com/derrod/legendary/releases/latest).
   If it mentions the path it is installing Among us to you may have to do this:
     - open legendary.exe from the folder the script is
     - write ```legendary uninstall 963137e4c29d4c79a81323b8fab03a40 --keep-files``` and click enter
     - retry the powershell script
5. Variations of "Invalid credentials, Please login again".
   <br> Solution:
     - open legendary.exe from the folder the script is
     - write ```legendary auth --delete``` and click enter
     - write ```legendary auth``` and click enter
6. "the game `963137e4c29d4c79a81323b8fab03a40` could not be found, did you spell it correctly?"
   <br> Solution:
     - the current signed in account does not have Among Us then which may occur from having multiple epic accounts
     - follow guidance from number 4 above and login to the account that has the game

Extra Note: number 3 may also occur because of antivirus quarantining legendary so you may want to turn it off temporarily if youve tried downloading it manually
