# Adding Pages

- Add a new route for `sell ticket`

```
# Sell Ticket Page
@route('/sell-ticket')
def sell_ticket():
    return "sell ticket"
```

- Check that it shows at `http://localhost:5000/sell-ticket`

- Add a new route for `check-in`

```
# Check In Page
@route('/check-in')
def check_in():
    return "check in"
```

- Check that it shows at `http://localhost:5000/check-in`
