# Sell Ticket Page Design

- Create header containing nav and back button
- Make back button an icon
- Put content in a container
- Make the form a 12-column container
- Put each input+label in an input-field div
- Make each one a row
- Style the submit button

```
<!DOCTYPE html>
<html>

    % include('shared/html-head.html')

    <body>
        
        <nav>
            <div class="nav-wrapper">
                <a href="#" class="brand-logo center">Sell Ticket</a>
                <ul class="left">
                    <li><a href="/"><i class="material-icons">arrow_back</i></a></li>
                </ul>
            </div>
        </nav>


        <div class="container">

            <form class="col s12" action="/ticket-sold" method="POST">

                <div class="row">
                    <div class="input-field col s12">
                        <input name="first_name" type="text" class="validate">
                        <label for="first_name">First Name</label>
                    </div>
                </div>

                <div class="row">
                    <div class="input-field col s12">
                        <input name="last_name" type="text" class="validate">
                        <label for="last_name">Last Name</label>
                    </div>
                </div>

                <div class="row">
                    <div class="input-field col s12">
                        <input name="email" type="email" class="validate">
                        <label for="email">Email</label>
                    </div>
                </div>

                <div class="row">
                    <button class="btn pink pink-text text-lighten-5" type="submit" name="action">
                        Submit
                    </button>
                </div>

            </form>

        </div>

    </body>

</html>
```