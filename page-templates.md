# Page Templates

- In bottle a template is known as a view

- Create a view template `index.html` for your home page

```
<!DOCTYPE html>
<html>
    
    <head>
        <title>Ticket Manager</title>
    </head>
    
    <body>
        <h1>Ticket Manager Home</h1>
    </body>
    
</html>
```

- Import view

```
from bottle import run, route, view
```

- Link the index template to your index route

```
# Home Page
@route('/')
@view('index')
def index():
    return "home page"
```

- Change the function to pass instead of return

```
# Home Page
@route('/')
@view('index')
def index():
    pass
```

- Check the view template loads at `http://localhost:5000`

- Do the same for `sell-ticket` and `check-in`