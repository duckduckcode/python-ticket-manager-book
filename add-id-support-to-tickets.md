# Add ID Support to Tickets


- Import count

```
from itertools import count
```

- Add a counter inside the class

```
class Ticket:

    _ids = count(0)

    def __init__(self, first_name, last_name, email):
        self.first_name = first_name
        self.last_name = last_name
        self.email = email
```

- Use the counter to create a sequential ID for each ticket

```
class Ticket:

    _ids = count(0)

    def __init__(self, first_name, last_name, email):
        self.first_name = first_name
        self.last_name = last_name
        self.email = email

        self.id = next(self._ids)
```

- Print the ID in the ticket list to check it worked


