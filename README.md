# Neptune's Hooks
[![Issues](https://img.shields.io/github/issues/Macro303/Neptunes-Hooks.svg?style=flat-square)](https://github.com/Macro303/Neptunes-Hooks/issues)
[![Contributors](https://img.shields.io/github/contributors/Macro303/Neptunes-Hooks.svg?style=flat-square)](https://github.com/Macro303/Neptunes-Hooks/graphs/contributors)
[![License](https://img.shields.io/github/license/Macro303/Neptunes-Hooks.svg?style=flat-square)](https://opensource.org/licenses/MIT)

A simple app that sends Neptune's Pride Stats to a Teams Channel via webhook.

## Built Using
 - [Python: 3.9.1](https://www.python.org/)
 - [pip: 21.0](https://pypi.org/project/pip/)
 - [requests: 2.25.1](https://pypi.org/project/requests/)
 - [PyYaml: 5.4.1](https://pypi.org/project/PyYaml/)

## Execution
1. Execute the following to generate the default files:
   ```bash
   $ pip install -r requirements.txt
   $ python -m Teams -h
   ```
2. Update the generated `config.yaml` with your:
    - Game Number: *Can be found in the url of the game*
    - API Code: *Can be found in the options' menu of the game*
    - Tick Rate
    - Player Aliases, names and Teams 
    - MS Teams Webhook
3. Run the following:
   ```bash
   $ python -m Teams
   ```

## Arguments
*You can find all these by using the `-h` or `--help` argument*

| Argument | Type | Default | Example | Description |
| -------- | ---- | ------- | ------- | ----------- |
| Poll Rate | int | 30 | `python -m Teams 30` | Used to determine how long between polls to the Neptune's Pride API *(value in Minutes)* |
| Testing | bool | False | `python -m Teams --testing` | Used to skip the tick check and use test config |

## Socials
[![Discord | The Playground](https://discord.com/api/v6/guilds/618581423070117932/widget.png?style=banner2)](https://discord.gg/nqGMeGg)  