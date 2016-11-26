# Home Page Design

- Add classes `pink` and `center-align` to the body
- Put the `h1` heading in a div with style classes
- Put the buttons in a container
- Put each button in its own row

```
<!DOCTYPE html>
<html>

    % include('shared/html-head.html')

    <body class="pink center-align">

        <div class="container pink-text text-lighten-5">
            <h1>My Event</h1>
        </div>

        <div class="container padded">

            <div class="row">
                <a class="btn grey lighten-5 pink-text pink-darken-3" href="/sell-ticket">
                    Sell Ticket
                </a>
            </div>

            <div class="row">
                <a class="btn grey lighten-5 pink-text pink-darken-3" href="/check-in">
                    Check In
                </a>
            </div>

        </div>
        
    </body>

</html>
```