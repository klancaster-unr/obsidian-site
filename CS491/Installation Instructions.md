# Development Environment

## Required Applications
Five applications are required for Elixir/Phoenix development:
-   Git
-   Postgresql database
-   Elixir and Erlang
-   Google Chrome
-   pgAdmin
-  Editor 
	- Any editor that supports Elixir will work. 
	- Recommended: Visual Studio Code


### Elixir

You can run elixir on any OS, however, it would be best if you use Linux or macOS as they are used the most in the community. Elixir will work on Windows, of course, however, support in the classroom will only be for Un\*x
based systems.

### Postgresql

- Linux: Follow the instructions here
https://www.postgresql.org/download/linux/ubuntu/

- macOS: The postgresapp application is by far the easiest to use on the Mac. You can download and install it here
https://postgresapp.com

### pgadmin

Install instructions can be found here: https://www.pgadmin.org

### Git

Git is available on most Linux and Mac systems pre-installed. You can download it at https://git-scm.com/downloads if needed.

## Installing and Configuring Phoenix

The steps for installing and configuring Phoenix 1.6 are slightly different from those found in the text, as 1.6 dropped `node` and `webpack`. Installation is quite easy: follow the instructions here https://hexdocs.pm/phoenix/installation.html#elixir-1-12-or-later

Note that you will need to install inotify-tools for on Linux to get live reloading working (you need this!)
