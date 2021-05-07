<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- displays site properly based on user's device -->

  <link rel="icon" type="image/png" sizes="32x32" href="./images/favicon-32x32.png">
  <link rel="stylesheet" href="style.css" >  
  <title>Frontend Mentor | Base Apparel coming soon page</title>
</head>
<body onload='document.form.email.focus()'>
  <div class="row">
    <div class="first-column">
      <img src="logo.png" class="logo">
      <div id="word">
        <h2> W E ' R E</h2> 
        <h1> C O M I N G <br> S O O N</h1>
        <p> Hello fellow shoppers! We're currently building our new <br> fashion store.
          Add your email below to stay up-to-date with <br> announcements and our launch deals.
        </p>
          <form id=form name="form">
            <div class="form-control">
              <input type="email" placeholder="Email Address" id="email" name="email" class="email" reguired>
              <button  onclick="Validate(email)" type="submit"  class="validate" ></button>
              <i> <img src="icon-error.png"> </i>
              <br>
              <label id="lb1text">Please provide a valid email</label> 
            </div>
          </form>
          
      </div>
    </div>
    

    <div class="second-column">
      
    </div>
  
  

</body>
</html>
