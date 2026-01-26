# Spotify Fetch

Command-line tool for displaying spotify artist and album information.

![](/images/example.png)

# Requirements

1. Make sure you have `python` and `pip` installed.

2. Register a [spotify app](https://developer.spotify.com/dashboard/login) and name it `sfetch` or whatever name you would like.

The redirect URI can be any valid URI such as `http://localhost`, `http://example.com`.

Once you have successfully registered an app, find your `Client ID` and `Client Secret`.

Don't share your `Client ID` and `Client Secret`.

3. Put the following variables you just got in your `.zshrc` or `.bashrc` or whatever shell you are using

```bash
export SPOTIPY_CLIENT_ID='your_client_id'
export SPOTIPY_CLIENT_SECRET='your_client_secret'
```

Remember to restart your shell!

# Installation

### Install with [pipx](https://github.com/pypa/pipx)

```bash
pipx install sfetch
```

### Development

1. Clone the repository

```bash
git clone https://github.com/mihasket/sfetch.git
cd sfetch
```

2. Make a virtual environment

```bash
python3 -m venv .venv
```

3. Activite the environment

```bash
. .venv/bin/activate
```

4. Install sfetch

```bash
pip install sfetch
```

# Usage example

For displaying artist information

```bash
sfetch --artist "C418"
```

For displaying album information

```bash
sfetch --artist "C418" --album "Volume Beta"
```

For additional help

```bash
sfetch --help
```
