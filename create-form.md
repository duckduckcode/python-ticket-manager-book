# Create Form

- Create a ticket sale form

```
<form>
  
  <label>First Name</label>
  <input type="text">
  
  <label>Last Name</label>
  <input type="text">
  
  <label>Email</label>
  <input type="email">
  
  <button type="submit">Submit</button>
  
</form>
```

- Make sure you have the right input 'name' and label 'for' values

```
<form>
  
  <label for="first_name">First Name</label>
  <input name="first_name" type="text">
  
  <label for="last_name">Last Name</label>
  <input name="last_name" type="text">

  <label for="email">Email</label>
  <input name="email" type="email">

  <button type="submit">Submit</button>
  
</form>
```

- Check the form at `http://localhost:5000`


