# Console Bot Assistant

## How to Use

Clone

```bash
git clone https://github.com/khomasl/goit-ds-hw-01.git
```

Then

```bash
cd goit-ds-hw-01/bot-with-poetry-docker
```

## Create docker image

```bash
docker build . -t console-bot
```

## Run it

```bash
docker run -it console-bot /bin/bash
```

or (if container is already running)

```bash
docker exec -it <container-id> /bin/bash
```

## The bot supports the following list of commands:

<div class="termy">

Add either a new contact with name and phone number, or a phone number to an existing contact:

```bash
add [name] [phone]
```

Change the phone number for the specified contact:

```bash
change [name] [old phone] [new phone]
```

Show phone numbers for the specified contact:

```bash
phone [name]
```

Show all contacts in the address book:

```bash
all
```

Add a birthday for the specified contact:

```bash
add-birthday [name] [birthdate]
```

Show the birthday for the specified contact:

```bash
show-birthday [name]
```

Show birthdays for the next 7 days with the dates when they should be congratulated:

```bash
birthdays
```

Receive a greeting from the bot:

```bash
hello
```

Close the program:

```bash
close
```

Close the program:

```bash
exit
```

</div>

## License

This project is licensed under the terms of the MIT license.
