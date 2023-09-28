# Kyse CLI

[![version](https://img.shields.io/github/tag/kyselabs/cli.svg)](https://github.com/kyselabs/cli/releases/latest)

Kyse Command Line Interface

## Install Kyse CLI

```bash
sudo curl -L "https://github.com/kyselabs/cli/releases/latest/download/kyse-$(uname -s)-$(uname -m)" -o /usr/local/bin/kyse
sudo chmod +x /usr/local/bin/kyse
```

## Authenticating

```bash
kyse login
```

## Kyse CLI

```
kyse-cli audits your code and environment.

Usage:
  kyse [command]

Available Commands:
  help        Help about any command
  login       Authentication
  test        When providing no params it performs a SCA scan
  version     Print the version number of kyse-cli

Flags:
  -h, --help   help for kyse

Use "kyse [command] --help" for more information about a command.
```

## Auditing your project

```bash
kyse test

# Providing a custom [-L | --max-level] recursion (default: 3)
kyse test --max-level 10
```

## Auditing your system

```bash
kyse test --system
```

## Auditing your source code

```bash
kyse test --code
```
