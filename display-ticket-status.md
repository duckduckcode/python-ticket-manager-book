# Display Ticket Status

- On the check in page

```

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

```