# Create Confirmation Page Route

- Create a new route, with the view

```
# Check In Confirmation Page
@route('/check-in-confirmation')
@view('check-in-confirmation')
def check_in_confirmation():
    pass
```
 
- Expect a ticket id to be passed in the URL

```
# Check In Confirmation Page
@route('/check-in-confirmation/<ticket_id>')
@view('check-in-confirmation')
def check_in_confirmation(ticket_id):
    pass
```