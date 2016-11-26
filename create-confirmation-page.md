# Create Confirmation Page

- Create `sale-confirmation.html`

```
<!DOCTYPE html>
<html>

    % include('components/html-head.html')

    <body class="center-align">

        <div class="container pink-text">

            <h1>Ticket Sold!</h1>

            {{ ticket.first_name }} {{ ticket.last_name }}


        </div>

        <div class="container padded">

            <a class="btn grey lighten-5 pink-text pink-darken-3" href="/">
                Done
            </a>

        </div>
        
    </body>

</html>
```