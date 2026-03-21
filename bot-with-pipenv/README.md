#                            Console Bot Assistant

## How to Use
Clone
```bash
git clone https://github.com/khomasl/goit-ds-hw-01.git
```

Then
```bash
cd goit-ds-hw-01/bot-with-pipenv
```

Install dependencies with pipenv
```bash
pip install pipenv --user
```
```bash
pipenv install
```

## Run it
```bash
python main.py
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
