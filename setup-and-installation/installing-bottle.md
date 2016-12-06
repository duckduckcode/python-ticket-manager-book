# Installing Bottle

Bottle is a Python module which has support for running websites with Python. It lets us do some Python processing in the background, then show those results in our HTML pages.


## Managing Modules with Pip

Pip is a module manager which comes with Python. Modules are like plugins which add extra functionality to Python. You can use Pip to install Python modules that other developers have published to the Pip database. Bottle is a Python module, so we can install it using Pip.

Pip is a command line app just like Python. You need to figure out your Pip run command just as you figured out your Python run command.

If you don't know your Python run command, see [Installing Python 3](/installing_python_3).

**If your Python run command is `python`**:<br>
Your matching Pip run command is `pip`.

**If your Python run command is `python3`**:<br>
Your matching Pip run command is `pip3`.

*Note: The examples use `pip`. You should replace with `pip3` if needed.*


## Install Bottle with Pip

In your command line:

1. Type `pip install bottle`
2. Press Enter
3. Wait for the installer to complete


## Check That It Worked

In your command line:

1. Type `python -c "import bottle"
2. Press Enter

**If the command line went to a new line with no output:**<br>
Bottle was most likely installed correctly. Congratulations! Skip the troubleshooting and go to the "What's Next" section below.

**If there was an error:**<br>
Then Bottle was not installed correctly. Here is the error for reference:

```
Traceback (most recent call last):
  File "<string>", line 1, in <module>
ImportError: No module named bottle
```

Try the troubleshooting below!



## Troubleshooting

1. **Ensure you're using the right version of Pip**<br>
  Double check whether your Pip command should be `pip` or `pip3` by following the instructions in [Installing Python 3](/installing_python_3)
2. ** You may have to install as admin**<br>
  Try running the same Pip install command again, but with `sudo` before it:<br>
  `sudo pip install bottle`<br>
  When asked for your password, type in your computer password and press Enter. The password will be invisible while you type.
  
  

## What's Next

**By now you should:**

- Have Bottle installed

**&raquo; Next Up: [Website Starter Template](website_starter_template.html)**


