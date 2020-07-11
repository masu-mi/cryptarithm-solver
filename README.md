# Cryptarithm-solver

Example code: wrap tool of [or-tools](https://google.github.io/or-tools/) for cryptarithm.
Now I've not make setup.py for creating a pip package.

## Usage

```sh
$ docker run masumi/cryptarithm-solver
NAME
    main.py

SYNOPSIS
    main.py COMMAND

COMMANDS
    COMMAND is one of the following:

     server
       start `cryptarithm solve` server with `/docs`

     solve
       solve cryptarithm problem
```

## Requirements

## Installation
Executing it  with docker is easy.

```sh
# solve a problem locally
docker run -it masumi/cryptarithm-solver solve 'SEND + MORE = MONEY'

# start solver server
docker run -p 8000:8000 -it masumi/cryptarithm-solver server
```


## License

See LICENSE.


## Development

```
$ pipenv sync -d
Installing dependencies from Pipfile.lock (bc16db)...
  __   ________________________________ 88/88 _ 00:00:48
To activate this project's virtualenv, run pipenv shell.
Alternatively, run a command inside the virtualenv with pipenv run.
All dependencies are now up-to-date!

$ pipenv run typecheck
Success: no issues found in 7 source files

$ pipenv run test
======================================== test session starts ========================================
platform darwin -- Python 3.8.1, pytest-5.4.3, py-1.9.0, pluggy-0.13.1
rootdir: /Users/masumi/dev/src/github.com/masu-mi/cryptarithm
collected 6 items

tests/test_lexer.py ......                                                                    [100%]

========================================= 6 passed in 0.09s =========================================
```

## Author
Masumi Kanai
