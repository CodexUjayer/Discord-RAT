## _Notice:_
_Everything in the Code is German yet... i will translate it soon, sry_

_The Code is still in the Beta, i started making it like 2 days ago._

_The Code is pretty unreadable bcs everything is one file. Thats on purpose bcs i dont want to have the pain with multiple Files in PyInstaller. I wont add a Builder or something because then tooo skiddy people are gonna use it_

_Please help me by contributing more Features and reporting issues and improvements._

# Discord-RAT
A remote administration Tool over discord. Easy to use, undetected and powerfull.

This Python Programm basically hosts a discord bot on the Computer its executed on, which allows the user who configured it to remotely control the computer via Discord commands. It supports a variety of features such as executing commands, taking screenshots, managing files, and more.

## Features

- **Ping:** Check the bot's latency.
- **Screenshot:** Take a screenshot and send it via Discord.
- **Execute Commands:** Run any CMD and PowerShell commands.
- **File Management:** Upload and download files.
- **Remote Execution:** Download and execute any Programms from a URL.
- **Notifications:** Send system notifications.
- **System Control:** Restart or shut down the computer.
- **Admin Rights:** Elevate the bot to run with admin privileges.
- **WiFi Profiles:** Export and send WiFi profiles and passwords.
- **System Info:** Retrieve system information.
- **Task Management:** List and kill processes.
- **Purge Messages:** Clear bot messages and commands in the channel.

## Requirements

- Python 3.6+
- Discord.py
- Additional Python packages (listed in `requirements.txt`)

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/truelockmc/Discord-RAT.git
    cd Discord-RAT
    ```

2. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

3. Replace placeholders in the script with your actual values:
    - `YOUR_BOT_TOKEN`: Your Discord bot token.
    - `YOUR_GUILD_ID`: Your Discord guild (server) ID.
    - `YOUR_USER_ID`: Your Discord user ID(s) who are authorized to control the bot.

## Configuration

Update the following variables in the script:
- `TOKEN`: The token for your Discord bot.
- `GUILD_ID`: The ID of the guild where the bot will operate.
- `AUTHORIZED_USERS`: A list of user IDs that are authorized to control the bot.

## Running the Bot

To run the bot, execute the script:
```sh
python your_script_name.py
```

## Commands

| Command                      | Description                                                                                         |
|------------------------------|-----------------------------------------------------------------------------------------------------|
| `!ping`                      | Shows the bot's latency.                                                                            |
| `!screenshot`                | Takes a screenshot and sends it.                                                                    |
| `!cmd <command>`             | Executes a CMD command.                                                                             |
| `!powershell <command>`      | Executes a PowerShell command.                                                                      |
| `!file_upload <target_path>` | Uploads a file to the specified path.                                                               |
| `!file_download <file_path>` | Downloads a file or folder from the specified path. (sends it to discord)                           |
| `!execute <url>`             | Downloads a Programm from the URL and executes it.                                                  |
| `!notify <title> <message>`  | Sends a notification.                                                                               |
| `!restart`                   | Restarts the PC.                                                                                    |
| `!shutdown`                  | Shuts down the PC.                                                                                  |
| `!admin`                     | Requests admin rights.                                                                              |
| `!stop`                      | Stops the bot.                                                                                      |
| `!wifi`                      | Shows WiFi profiles and passwords.                                                                  |
| `!system_info`               | Shows system information.                                                                           |
| `!cpu_usage`                 | Shows current CPU usage.                                                                            |
| `!taskkill <pid>`            | Terminates a process with the specified PID.                                                        |
| `!purge`                     | Deletes the bot messages and commands.                                                              |
| `!help`                      | Displays a list of available commands.                                                              |

### Example Usage

1. **Running a CMD command:**
    ```sh
    !cmd dir
    ```

2. **Taking a screenshot:**
    ```sh
    !screenshot
    ```

3. **Restarting the PC:**
    ```sh
    !restart
    ```

## Security

- Ensure that only trusted users have access to the bot by updating the `AUTHORIZED_USERS` list.
- Avoid sharing the bot token publicly.

## Contributing

Feel free to submit issues or pull requests if you have suggestions or improvements.

## License

This project is licensed under the GNU Affero General Public License v3.0 (AGPL-3.0)
