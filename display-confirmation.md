# Display Confirmation

- Create `check-in-confirmation.html`

```
<!DOCTYPE html>
<html>

    % include('shared/html-head.html')

    <body class="center-align">

        <div class="container pink-text">

            % if ticket == None:

                <h1>Check-In Failed</h1>

                <strong>Sorry, that ticket wasn't found :(</strong>

            % else:

                <h1>Success!</h1>

                <strong>{{ ticket.first_name }} {{ ticket.last_name }}</strong>
                <p>has been checked in.</p>

            % end


        </div>

        <div class="container padded">

            <a class="btn grey lighten-5 pink-text pink-darken-3" href="/check-in">
                Done
            </a>

        </div>
        
    </body>

</html>
```