# Display a List

- In `check-in.html` create a list with one list item

```
<ul>
    <li>Person Name</li>
</ul>
```

- Check that it shows up at `http://localhost:5000/check-in`

- Modify the check in route to pass the tickets to the view

```
# Check In Page
@route('/check-in')
@view('check-in')
def check_in():

    data = dict(
        ticket_list = tickets
    )

    return data
```

- In `check-in.html` create a loop to repeat the list items

```
<ul>
    % for name in ticket_list:
        <li>Person Name</li>
    % end
</ul>
```

- Preview to ensure it has run one for every ticket

- Replace Person Name with each name in the ticket list

```
<ul>
    % for name in ticket_list:
        <li>{{ name }}</li>
    % end
</ul>
```

- Preview at `http://localhost:5000/check-in`