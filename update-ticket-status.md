# Update Ticket Status


- Get the ticket id as an integer
 
```
# Check In Confirmation Page
@route('/check-in-confirmation/<ticket_id>')
@view('check-in-confirmation')
def check_in_confirmation(ticket_id):

    ticket_id_to_check_in = int(ticket_id)
    
    pass
 ```
 
 - Find the ticket with that ID

```
# Check In Confirmation Page
@route('/check-in-confirmation/<ticket_id>')
@view('check-in-confirmation')
def check_in_confirmation(ticket_id):

    ticket_id_to_check_in = int(ticket_id)

    for ticket in tickets:
        if ticket.id == ticket_id_to_check_in:
            print("found ticket!")
 ```
 
 
- Store the ticket in a variable

```
# Check In Confirmation Page
@route('/check-in-confirmation/<ticket_id>')
@view('check-in-confirmation')
def check_in_confirmation(ticket_id):

    ticket_id_to_check_in = int(ticket_id)
    checked_in_ticket = None

    for ticket in tickets:
        if ticket.id == ticket_id_to_check_in:
            checked_in_ticket = ticket
 ```
 
 - Make the ticket status 'checked in'

```
# Check In Confirmation Page
@route('/check-in-confirmation/<ticket_id>')
@view('check-in-confirmation')
def check_in_confirmation(ticket_id):

    ticket_id_to_check_in = int(ticket_id)
    checked_in_ticket = None

    for ticket in tickets:
        if ticket.id == ticket_id_to_check_in:
            ticket.checked_in = True
            checked_in_ticket = ticket
 ```
 
 - Send the ticket to the view

```
# Check In Confirmation Page
@route('/check-in-confirmation/<ticket_id>')
@view('check-in-confirmation')
def check_in_confirmation(ticket_id):

    ticket_id_to_check_in = int(ticket_id)
    checked_in_ticket = None

    for ticket in tickets:
        if ticket.id == ticket_id_to_check_in:
            ticket.checked_in = True
            checked_in_ticket = ticket
    
    data = dict(
        ticket = checked_in_ticket
    )

    return data
 ```
