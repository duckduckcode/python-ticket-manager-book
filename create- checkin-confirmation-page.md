# Create Confirmation Page

- Create `check-in-confirmation.html`

```
<!DOCTYPE html>
<html>

    % include('shared/html-head.html')

    <body class="center-align">

        <div class="container pink-text">


                <h1>Check-In Failed</h1>

                <strong>Sorry, that ticket wasn't found :(</strong>

                <h1>Success!</h1>

                <strong>Person Name</strong>
                <p>has been checked in.</p>

        </div>

        <div class="container padded">

            <a class="btn grey lighten-5 pink-text pink-darken-3" href="/check-in">
                Done
            </a>

        </div>
        
    </body>

</html>
```