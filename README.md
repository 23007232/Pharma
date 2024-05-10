# Project Responsive Web Design using Bootstrap
## Date:10/5/24

## AIM:
To design a responsive website for a Pharmaceutical Company using Bootstrap.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="style.css">
    <title>TATA MOTORS</title>
    <style>
      *{
    margin: 0px;
    padding: 0px;
    font-family: century;
}
header{
    background-image: url(bg.png);
    height: 100vh;
    background-size: cover;
    min-height: 100px;
    background-position: center;
    background-blend-mode: lighten;
    opacity: 50px;
    filter: brightness(60px);
}
ul{
    float: right;
    list-style-type: none;
    margin-top: 30px;
    min-height: 400px;
    margin-right: 60px;
    font-size: 17px;
}
ul li{
    display: inline-block;
}
ul li a{
    text-decoration: double;
    color: rgb(160, 162, 4);
    padding: 5px 50px;
    border: 1px solid transparent;
    transition: 0.5 ease;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    font-size: larger;
}

ul li a:hover{
    background-color: black;
    color: white;
}
.search{
    width: 330px;
    float:right;
    margin-right: 20px;
}
.srch{
    font-family: 'Times New Roman';
    width: 200px;
    height: 40px;
    background: rgb(237, 234, 234);
    border: 1px solid rgb(21, 21, 21);
    margin-top: 13px;
    color: rgb(22, 22, 21);
    border-right: none;
    font-size: 16px;
    float: left;
    padding: 10px;
    border-bottom-left-radius: 5px;
    border-top-left-radius: 5px;

}
.btn{
    width: 100px;
    height: 40px;
    background: #120f0f;
    border: 2px solid#141313;
    margin-top: 13px;
    color:rgb(241, 237, 237);
    font-size: 15px;
    border-bottom-right-radius: 5px;
    border-bottom-right-radius: 5px;
}
.btn:focus{
    outline: none;
}
.srch:focus{
    outline: none;

}
.logo img{
    float: inline-start;
    padding: 0px;
}
.title{
    position: absolute;
    left: 5%;
    top: 40%;
    color:#120f0f(187, 61, 3);
    font-size:20px;
}
 b{
    color:rgb(33, 33, 33);
    border-color:black;
    font-size: 50px;
    font-family: 'Gill Sans', 'Gill Sans MT',  'Trebuchet MS', sans-serif;
}
.button {
    position: absolute;
    left: 30%;
    top: 95%;   
    width: 500px;
    border-radius: 50px;
    border: 2px;
    font-weight: 600;
    font-size: 20px;
}
.button .button{
transition: 0.5s;
}
.form
{
    width: 250px;
    height: 380px;
    background: linear-gradient(to top, rgba(214, 202, 202, 0.8)50%,rgba(210, 202, 202, 0.8)50%);
    position: absolute;
    top: 200px;
    left: 1150px;
    border-radius: 10px;
    padding: 25px;
}
.form h2{
    width: 220px;
    font-family: sans-serif;
    color: black;
    text-align: center;
    color: rgb(248, 241, 241);
    font-size: 22px;
    background-color: rgb(21, 21, 21);
    border-radius: 10px;
    margin: 2px;
    padding: 8px;
}
.form input{
    width: 240px;
    height: 35px;
    background: transparent;
    border-bottom: 1px solid white;
    border-top: none;
    border-right: none;
    border-left: none;
    color: black;
    font-size: 15px;
    letter-spacing: 1px;
    margin-top: 30px;
    font-family: sans-serif;
}
.t{
    position: absolute;
    left: 10%;
    top: 75%;
    font-size:smaller;
}
.t b{
    color: rgb((255, 255, 255)55, 255, 255);
    font-size: 20px;
    font-family: Arial, Helvetica, sans-serif;
}
.form input:focus{
    outline: none;
}
::placeholder{
    color: black;
    font-family: Arial;
}
.btnn{
    width: 240px;
    height: 40px;
    background: white;
    border: none;
    margin-top: 30px;
    font-size: 18px;
    border-radius: 10px;
    cursor: pointer;
    color: black;
}
.btnn:hover{
    background: black;color: #fff   ;
}
.form .link{
    font-family: Arial, Helvetica, sans-serif;
    font-size: 17px;
    padding-top: 20px;
    text-align: center;

}
.liw{
    padding-top: 15px;
    padding-bottom: 10px;
    text-align: center;
}
.wrapper .icon{
    position: relative;
    background-color: #ffffff;
    border-radius: 50%;
    margin: 5px;
    width: 30px;
    height: 30px;
    line-height: 30px;
    font-size: 20px;
    display: inline-block;
    align-items: center;
    box-shadow: 0 10px 10px rgba(0, 0, 0, 0.1);
    cursor: pointer;
    transition: all 0.2s cubic-bezier(0.68, -0.55, 0.265, 1.55);
    color: #333;
    text-decoration: none;
  }
  .wrapper .tooltip {
    position: absolute;
    top: 0;
    line-height: 1.5;
    font-size: 14px;
    background-color: #ffffff;
    color: #ffffff;
    padding: 5px 8px;
    border-radius: 5px;
    box-shadow: 0 10px 10px rgba(0, 0, 0, 0.1);
    opacity: 0;
    pointer-events: none;
    transition: all 0.3s cubic-bezier(0.68, -0.55, 0.265, 1.55);
  }
  .wrapper .tooltip::before {
    position: absolute;
    content: "";
    height: 8px;
    width: 8px;
    background-color: #ffffff;
    bottom: -3px;
    left: 100%;
    transform: translate(-50%) rotate(45deg);
    transition: all 0.3s cubic-bezier(0.68, -0.55, 0.265, 1.55);
  }
  .wrapper .icon:hover .tooltip {
    top: -45px;
    opacity: 1;
    visibility: visible;
    pointer-events: auto;
  }
  .wrapper .icon:hover span,
  .wrapper .icon:hover .tooltip {
    text-shadow: 0px -1px 0px rgba(0, 0, 0, 0.1);
  }
  .wrapper .facebook:hover,
  .wrapper .facebook:hover .tooltip,
  .wrapper .facebook:hover .tooltip::before {
    background-color: #3b5999;
    color: #ffffff;
  }
  .wrapper .twitter:hover,
  .wrapper .twitter:hover .tooltip,
  .wrapper .twitter:hover .tooltip::before {
    background-color: #46c1f6;
    color: #ffffff;
  }
  .wrapper .instagram:hover,
  .wrapper .instagram:hover .tooltip,
  .wrapper .instagram:hover .tooltip::before {
    background-color: #e1306c;
    color: #ffffff;
  }
  .wrapper .github:hover,
  .wrapper .github:hover .tooltip,
  .wrapper .github:hover .tooltip::before {
    background-color: #333333;
    color: #ffffff;
  }
  .wrapper .youtube:hover,
  .wrapper .youtube:hover .tooltip,
  .wrapper .youtube:hover .tooltip::before {
    background-color: #de463b;
    color: #ffffff;
  }
  h1{
    color:rgb(255, 102, 0);
  }
    </style>
<link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/css/all.min.css'>
</head>
<body>
    <header>
        <div class="main">
            <ul>
                <li><a href="index.html">HOME</a></li>
                <li><a href="people.html">PEOPLE</a></li>
                <li><a href="products.html">PRODUCTS</a></li>
                <li><a href="contact.html">CONTACT</a></li>
            </ul>
        </div>
        <div class="search" >
            <input class="srch" type="search" name="" placeholder="type to search">
            <a href="#"><button class="btn">Search</button></a>
        </div>
        <div class="logo">
            
        </div>
        <div class="title" >
            <h1><b>Driving Tommorow: Tata Motors,<br>where innovation meets the open road</b></h1>
        </div>
        <div class="form">
            <h2>Login Here</h2>
            <input type="email" name="email" placeholder="Enter Your Mail ID">
            <input type="password" name=" " placeholder="Enter Your password">
            <button class="btnn"><a href="#">Login</a></button>
            <p class="Link">Don't have an account<br>
            <a href="#">Sign Up</a> Here</p>
            <p class="liw">Login with email</p>
        
        <div class="wrapper">
            <a href="#" class="icon facebook">
              <div class="tooltip">Facebook</div>
              <span><i class="fab fa-facebook-f"></i></span>
            </a>
            <a href="#" class="icon twitter">
              <div class="tooltip">Twitter</div>
              <span><i class="fab fa-twitter"></i></span>
            </a>
            <a href="#" class="icon instagram">
              <div class="tooltip">Instagram</div>
              <span><i class="fab fa-instagram"></i></span>
            </a>
            <a href="#" class="icon github">
              <div class="tooltip">Github</div>
              <span><i class="fab fa-github"></i></span>
            </a>
            <a href="#" class="icon youtube">
              <div class="tooltip">Youtube</div>
              <span><i class="fab fa-youtube"></i></span>
            </a>
          </div>
          </div>

        <div class="t">
            <h1><b>“Innovation is taking two things that <br>already exist and putting them together in a new way<br>-Ratan Tata”<br>developed by pavitra p(212223110035)</b></h1>
        </div>
       
</body>
</html>
```

## OUTPUT:
![image](https://github.com/23007232/Pharma/assets/139115574/a75159cd-b3d9-42f5-8263-66f02fee7a65)


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
