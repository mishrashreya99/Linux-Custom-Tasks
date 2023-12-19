# internsctl - A System Information and User Management Tool

`internsctl` is a command-line utility designed to provide system information and basic user management functionalities. It offers commands to display CPU and memory information, create new users, list existing users, and obtain file information.

## Commands:

- **CPU Information:**
- 
  internsctl cpu getinfo
Display detailed CPU information.

## Memory Information:

internsctl memory getinfo
Display information about system memory.

# User Management:

## Create User:

internsctl user create <username>
Create a new user with the specified username.

## List Users:


internsctl user list [--sudo-only]
List regular users (optionally, list only users with sudo permissions).

## File Information:


internsctl file getinfo [OPTIONS] <file-name>
Get detailed information about a file.

## Options:
--version: Display the command version.
--help: Display the help message.
Examples:
Display CPU information:


internsctl cpu getinfo


Create a new user:


internsctl user create john_doe


List all users:


internsctl user list
Get file information:

internsctl file getinfo sample.txt


## Diagram:

+---------------------+       +------------------+
|   Command Line     | ----> |    internsctl    |
|      Interface      |       |                  |
+---------------------+       +------------------+
                                 |          |
           +---------------------+  +------------------------+
           |                         |                        |
           v                         v                        v
      +---------+             +-----------+           +-------------------+
      |  cpu    |             |  memory   |           |      user         |
      +---------+             +-----------+           +-------------------+
      |  getinfo|             |  getinfo  |           |  create           |
      +---------+             +-----------+           |  list [--sudo-only]|
                                 |                     +-------------------+
                                 |
                        +-------------------+
                        |       file        |
                        +-------------------+
                        |  getinfo [OPTIONS]|
                        +-------------------+
Note: Replace [OPTIONS] and <file-name> with appropriate options and file name.

## How to Use:
Clone the repository:


git clone https://github.com/your_username/internsctl.git
cd internsctl

Execute the script:


bash internsctl <command> [options]
For more details and examples, refer to the --help option.

Feel free to contribute or report issues on GitHub.
