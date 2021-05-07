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

body{
    margin: 0px;
}
@font-face {
    font-family: 'JosefinSans';
    src: url(Fonts/JosefinSans-Bold.ttf);
    font-weight: 600;
    font-style: normal;
}
@font-face {
    font-family: 'JosefinSans';
    src: url(Fonts/JosefinSans-SemiBold.ttf);
    font-weight: 400;
}
@font-face {
    font-family: 'JosefinSans';
    src: url(Fonts/JosefinSans-Light.ttf);
    font-weight: 300;
}

.first-column{
    width: 60%;
    float: left;
    background-image: url(bg-pattern-desktop.png);
    background-position: bottom;
    background-repeat: no-repeat;
    background-size: cover;
    height: 100vh;
    

}
.second-column{
    width: 40%;
    float: right;
    height: 100vh;
    background-image: url(hero-desktop.jpg);
    background-repeat: no-repeat;
    background-size: cover;

}

h1{
    font-family: JosefinSans;
    font-weight: 400;
    font-size: 60px;
    color: hsla(0, 6%, 24%, 0.925);
    margin: 0px;
  
}
h2{
    font-family: JosefinSans;
    font-weight: 300;
    font-size: 55px;
    color: hsl(0, 41%, 71%);
    margin: 0px;

}
p{
    font-family: JosefinSans;
    font-weight: 300;
    font-size: 15px;
    color: hsl(0, 36%, 70%);
    
    
    
}
#word{
    padding-top: 120px;
    padding-left: 150px;
}
.logo{
    padding-top: 50px;
    padding-left: 150px;

}
.form-control{
    position: relative;
}
label{
    color: hsl(0, 84%, 64%);
    font-family: JosefinSans;
    font-weight: 300;
    font-size: 15px;
}
input[type=email]{
    border:2px solid;
    width: 280px;
    font-family: JosefinSans;
    font-weight: 300;
    color: hsl(0, 97%, 76%);
    border-radius: 40px;
    border-color: hsl(0, 41%, 71%);
    padding: 12px;
    border-width: 1px;  
}
button{
    border-radius: 40px;
    background-color: hsl(0, 75%, 89%);
    background-image: url(icon-arrow.png);
    background-repeat: no-repeat;
    background-position: center;
    padding: 20px;
    border: 2px solid;
    border-color: hsl(0, 75%, 89%);
    width:80px;
    position: relative;   
    right: 65px;
    bottom:3px;   

}
:focus{
    outline: none;
}
.form-control i {
	position: relative;;
	right: 180px;
    top: 7px;
    
}
.form-control.error i{
	visibility: visible;
}
.arrow{
    background-color: hsl(0, 78%, 75%);
    height: 42px;
    position: relative;
    top: 17px;  
    right: 50px;
    border-radius: 40px;
    width: 80px;

   
   
}
@media only screen and (max-width:550px){
    
    .second-column{
        width: 100%;
        position: absolute;
        top: 55px;
        background-image: url(hero-mobile.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        height: 350px;
        
    }
    
    .first-column{
        width: 100%;

    }   
     .logo{
         position: relative;
         bottom: 50px;
    }
    #word{
        position: relative;
        top: 210px;
        padding-left: 30px;
    }
    h1{
        font-size: 45px;
        text-align: center;
    } 
    h2{
        font-size: 40px;
        text-align: center;
    }
    p{
        text-align: center;
    }
    label{
        visibility: hidden;
    }
    .form-control{
        left: 40px;
        top: 20px;
    }

}
