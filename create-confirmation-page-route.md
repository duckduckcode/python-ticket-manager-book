# Create Confirmation Page Route

```
# Sale Confirmation Page
@route('/ticket-sold', method='POST')
@view('sale-confirmation')
def ticket_sold():
    
    first_name = request.forms.get('first_name')
    last_name = request.forms.get('last_name')
    email = request.forms.get('email')

    new_ticket = Ticket(first_name, last_name, email)
    tickets.append(new_ticket)

    data = dict(
        ticket = new_ticket
    )

    return data
```