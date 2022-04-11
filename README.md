# Zicron API Documentation

## Introduction

Hey! Welcome to the official documentation of the Zicron API!
This documentation should **NOT** be shared with anyone else which isn't in the developer team!
We love you guys, let's get started!

## What is the Zicron API?

**Zicron API** is an API used for quick functions for our developers. Some of them are important for use.
There will be functions used for specific tasks, we will explain everything.

## Discord functions

Fyi (for your information), we are using DiSky V4, so syntaxes might be confusing. Don't worry, if you need any help, contact Cerial.

### Option types (and what they mean):

|Type|What it means|
|----|-------------|
|string|You can enter any character in there. This is the default if you don't enter the `optionType` argument in the `newOption_Slash` function.|
|integer|You can enter any number (including decimals), for example `3.21`.|
|number|You can enter any **rounded** number (without decimals), for example `3`.|
|user|You can specify a user in the Discord server. It will show you a list of the users, and if you want you can enter a username in there and it will search it (technology yay).|
|role|Pretty much the same thing with the `user` option, but it shows roles instead.
|boolean|You will be shown a menu with `True` and `False`.

### The actual functions (wow):

|Function name|What it does|Example|Notes|
|-------------|------------|-------|-----|
|newSlash("commandName", "commandDescription")|Makes a new slash command. Use it on the `on load` event.|set {_c} to newSlash("giveBunny", "Gives you a fine bunny.")|None|
|newOption_Slash({_variable}, "optionname", "optionDescription", "optionType", "isOptional")|Adds a new option to the slash command. Options are basically arguments you can enter information into.|newOption_Slash({_c}, "name", "What will be the name for your bunny?")|1. For the `optionType` argument, you don't have to enter anything in there, it will default to `string` option. |
