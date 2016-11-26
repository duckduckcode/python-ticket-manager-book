# Check In Page Design

- Make the header a `nav` 
- Make the back button an icon
- Put the list in a div with class `container`
- Make the list a `collection` with `left-align`
- Make each list item a `collection-item`

```
<!DOCTYPE html>
<html>

    % include('shared/html-head.html')

    <body class="center-align">

        <nav>
            <div class="nav-wrapper">
            <a href="#" class="brand-logo center">Check In</a>
            <ul class="left">
                <li><a href="/"><i class="material-icons">arrow_back</i></a></li>
            </ul>
            </div>
        </nav>
        
        <div class="container">
            <ul class="collection left-align">

                % for ticket in ticket_list:
                    <li class="collection-item">
                        <strong>{{ ticket.first_name}} {{ ticket.last_name }}</strong>
                    </li>
                % end
                
            </ul>
        </div>

    </body>

</html>
```