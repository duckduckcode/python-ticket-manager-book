# Create a Ticket Class

- Create a new class called Ticket

```
# CLASSES ######################

class Ticket:

    def __init__(self, first_name, last_name, email):
        self.first_name = first_name
        self.last_name = last_name
        self.email = email
```

- Update the ticket list to use Tickets not just names

```
tickets = [
    Ticket("Fred", "Flintstone", "fred@flintstone.com"),
    Ticket("Wonder", "Woman", "wonderwoman@heroes.org"),
    Ticket("Justin", "Bieber", "justin@thebeebs.com")
]
```

- Update the view to loop over Tickets not strings

```
<ul>
    % for ticket in ticket_list:
        <li>{{ ticket.first_name }}</li>
    % end
</ul>
```

- Preview at `http://localhost:5000/check-in`

- Make the list display first and last name
