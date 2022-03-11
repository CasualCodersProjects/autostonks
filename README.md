# AutoStonks

## Getting started.

Requires [Python 3.8 or newer](https://www.python.org/downloads/) to be installed.

Dependency management is done via [Pipenv](https://pipenv.pypa.io/en/latest/). This can be installed via Pip.

```sh
pip install pipenv
```

### Cloning and installing dependencies

```sh
git clone https://github.com/CasualCodersProjects/autostonks
cd autostonks
pipenv install
pipenv shell
```

Now you development environment is set up.

### API Keys and .env file

To generate API keys, you need to [create an account on Alpaca](https://alpaca.markets/). You don't need to create a live account if you don't want to, you can just create a paper account to test development. Once you finish creating your account, you can open up the [Paper Dashboard](https://app.alpaca.markets/paper/dashboard/overview) before adding bank account and tax information so you can get to development without using money.

From the dashboard, you can generate API Keys and populate the .env file.

```sh
# .env
BASE_URL=https://paper-api.alpaca.markets
API_KEY=abcdefghijkl
API_SECRET=abcdefghijklmnopqrstuvwxyz1234567890
```

### Running the bot

The bot is written with Fire, which generates a command line tool from Python functions. The current usage is:

```sh
python stonks.py -h
```

This will print out help information.
