# Bottle Starter App

This guide will help you set up and run a basic Bottle app. These instructions can be followed to start any new Bottle project, as they will be the same for any app you make using Bottle.



## Create an index page

* Create a new file called \`index.html\`
* Add HTML to the file just like a normal HTML page
* Starter code is included below

```
<!DOCTYPE html>
<html>

    <head>
        <title>My Bottle App</title>
    </head>

    <body>
        <h1>Hello!</h1>
    </body>

</html>
```


## Create the Python app

* Create a new file called \`website.py\`
* Import \`route\` and \`run\`
* Create a route for the index page
* Add the run command
* Starter code is included below, called \`website.py\`

```
from bottle import run, route, view


# PAGES ########################

# Home Page
@route('/')
@view('index')
def index():
    pass
    

# START THE WEBSITE ###########

run(host='0.0.0.0', port=8080, reloader=True, debug=True)

```

## Run the Python app

* In the shell type \`python3 website.py\` and press enter
* In your web browser open the address \`http://0.0.0.0:8080\`
* You should see "Hello!" on your website
* Once the site is running you can just refresh to see changes
* Make sure not to run two copies of the app at the same time

Bottle websites need to run on a **local server**. Plain HTML and CSS websites can be opened directly in a web browser, but Bottle needs a web server so that the Python parts can run.

Running your Bottle app automatically starts a web server.



## Extras

Here are some extra bits you may like to know:

### Stopping the Site

Most of the time you can just leave the site running. You can stop the site if something goes wrong or if you want to change some launch settings.

In your command line:

* Press Ctrl + C

This will shut down the web server, so your website will no longer load in a web browser.

### Reloading Changes

Bottle automatically updates your site with any changes you make. You will need to press the "Refresh" button in your browser to see the changes.

If your changes are not updating, try stopping your web server and starting it again.

