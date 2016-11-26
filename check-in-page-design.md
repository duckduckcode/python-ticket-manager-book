# Check In Page Design

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

                        % if ticket.checked_in:
                            <i class="material-icons green-text secondary-content right">check_circle</i>
                        % else:
                            <a href="/check-in-confirmation/{{ ticket.id }}">
                                <i class="material-icons grey-text text-lighten-2 secondary-content right">panorama_fish_eye</i>
                            </a>
                        % end

                    </li>
                % end
                
        </ul>
        </div>

    </body>

</html>
```