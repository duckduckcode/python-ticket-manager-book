# Creating a Site

- Create file `website.py`

- From bottle import run
- From bottle import route

```
from bottle import run, route
```

- Create home page route:

```
# PAGES ########################

# Home Page
@route('/')
def index():
    return 'hello'

```

- Add launcher

```
# START THE WEBSITE ###########

run(host='0.0.0.0', port=8080, reloader=True, debug=True)
```


- Run using `python website.py`

- View in browser at `http://0.0.0.0:5000`
