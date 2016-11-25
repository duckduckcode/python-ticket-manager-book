# Create a Shared Head

- Create a new folder called `shared`

- In the folder, create a file `html-head.html`

```
<head>

    <title>My Event Manager</title>
    
</head>
```

- Include the head in every html page

```
% include('shared/html-head.html')
```

- Add viewport meta to allow it to work on mobile

```
<head>

    <title>My Event Manager</title>

    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
    
</head>
```

- Check the title shows in the tab bar on every page