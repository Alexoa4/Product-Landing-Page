<h1>Responsive Web Design</h1>
<h2>Building A Product Landing Page</h2>

<h3>Project Objective</h3>
To Build an app that is functionally similar to https://product-landing-page.freecodecamp.rocks.
<br />


<h2>Languages Used</h2>

- <b>HTML and CSS</b> 
  
<h2>User Story:</h2>

- <b>Your product landing page should have a header element with a corresponding id="header"
You can see an image within the header element with a corresponding id="header-img" (A logo would make a good image here)
Within the #header element, you can see a nav element with a corresponding id="nav-bar"
You can see at least three clickable elements inside the nav element, each with the class nav-link
When you click a .nav-link button in the nav element, you are taken to the corresponding section of the landing page
You can watch an embedded product video with id="video"
Your landing page has a form element with a corresponding id="form"
Within the form, there is an input field with id="email" where you can enter an email address
The #email input field should have placeholder text to let users know what the field is for
The #email input field uses HTML5 validation to confirm that the entered text is an email address
Within the form, there is a submit input with a corresponding id="submit"
When you click the #submit element, the email is submitted to a static page (use this mock URL: https://www.freecodecamp.com/email-submit)
The navbar should always be at the top of the viewport
Your product landing page should have at least one media query
Your product landing page should utilize CSS flexbox at least once
Fulfill the user stories and pass all the tests below to complete this project. Give it your own personal style. Happy Coding!
</b>

<h2>Program walk-through: HTML</h2>

<!DOCTYPE html>
<html>
  <head>
   <link rel="stylesheet" href="styles.css"> 
   <script src="https://kit.fontawesome.com/ef56e69b77.js" crossorigin="anonymous"></script>
  </head>
      <body
         < id="page-wrapper">

               <header id="header">
                    <div class="logo">
                      <img id="header-img" src="https://cdn.freecodecamp.org/testable-projects-fcc/images/product-landing-page-logo.png" alt="">
                    </div>
                <nav id="nav-bar">
                    <ul>
                      <li>
                        <a class="nav-link" href="#features">Features</a>
                      </li>
                      <li>
                        <a class="nav-link" href="#how-it-works">How it works</a>
                      </li>
                      <li>
                        <a class="nav-link" href="#pricing">Pricing</a>
                      </li>
                    </ul>
                </nav>
              </header>
              <div class="container"></div>
                <section id="hero">
                  <h2>Hancrafted, Home-made Masterpieces</h2>

                  <form id="form" action="https://www.freecodecamp.com/email-submit">
                    <input id="email" type="email" name="email" placeholder="Enter email Address" required >
                    <input type="submit" id="submit" value="Get Started" class="btn">
                  </form>
              </section>
              <div class="container">
                <section id="features">
                  <div class="grid">
                    <div class="icon">
                      <i class="fa fa-3x fa-fire"></i>
                    </div>
                    <div class="desc">
                      <h2> Premium Materials</h2>
                      <p>Our trombones use the shiniest brass which is sourced locally. This will increase the longevity of your purchase.</p>
                    </div>

                  </div>
                  <div class="grid">
                    <div class="icon">
                      <i class="fa fa-3x fa-truck"></i>
                    </div>
                    <div class="desc">
                      <h2> Fast Shipping</h2>
                      <p>We make sure you receive yourtrombone.. Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum laborum magnam odio perferendis porro cum hic libero possimus, corrupti ipsam?</p>
                    </div>

                  </div>
                  <div class="grid">
                    <div class="icon">
                      <i class="fa fa-3x fa-robot"></i>
                    </div>
                    <div class="desc">
                      <h2> Quality Assurance</h2>
                      <p>For every purchase you make, we will ensure... Lorem ipsum, dolor sit amet consectetur adipisicing elit. Est consectetur quasi reiciendis culpa sequi blanditiis odio accusamus quia ullam corporis.</p>
                    </div>

                  </div>

                </section>

                <section id="how-it-works">
                    <iframe id="video" src="https://www.youtube-nocookie.com/embed/y8Yv4pnO7qc?rel=0&controls=0&showinfo=0" frameborder="0" height="315" allowfullscreen>
                      
                    </iframe>
                </section>

                <section id="pricing">
                  <div class="product" id="tenor">
                    <div class="level">Tenor Trombone</div>
                    <h2>$699</h2>
                    <ol>
                      <li>Lorem, ipsum dolor.</li>
                      <li>Lorem, ipsum dolor.</li>
                      <li>Lorem, ipsum dolor.</li>
                      <li>Lorem, ipsum dolor.</li>
                    </ol>
                    <button class="btn">Select</button> 
                  </div>
                  <div class="product" id="bass">
                    <div class="level">Bass Trombone</div>
                    <h2>$899</h2>
                    <ol>
                      <li>Lorem, ipsum dolor.</li>
                      <li>Lorem, ipsum dolor.</li>
                      <li>Lorem, ipsum dolor.</li>
                      <li>Lorem, ipsum dolor.</li>
                    </ol>
                    <button class="btn">Select</button> 
                  </div>
                  <div class="product" id="valve">
                    <div class="level">Valve Trombone</div>
                    <h2>$1299</h2>
                    <ol>
                      <li>Lorem, ipsum dolor.</li>
                      <li>Lorem, ipsum dolor.</li>
                      <li>Lorem, ipsum dolor.</li>
                      <li>Lorem, ipsum dolor.</li>
                    </ol>
                    <button class="btn">Select</button> 
                  </div>
                </section>

                  <footer >
                    <ul>
                        <li>
                          <a href="#">Privacy</a>
                        </li>
                        <li>
                          <a href="#">Terms</a>
                        </li>
                        <li>
                          <a href="#">Contact</a>
                        </li>
                    </ul>
                    <span>Copyright 2022, Original Trombones</span>
                  </footer>
    
              </div>
                        
          </div>
      </body>
</html>

<h2>Program walk-through: CSS</h2>

body{
background-color: bisque;
font-family: sans-serif;
}
*{
  margin:0;
  padding: 0;
  box-sizing: border-box;
}
 #page-wrapper{
   position:relative;
 }

 header {
   position: fixed;
   top: 0;
   min-height: 75px;
   padding: 0 20px;
   display: flex;
   justify-content: space-around;
   align-items: center;
   background-color: bisque;
 }
   

 .logo{
   margin-top: 15px;
   width:100%;
   position: relative; 
 }
 .logo > img {
   width: 100%;
   height: 100%;
   max-width: 300px;
   display: flex;
   justify-content: center;
   align-items: center;
   text-align: center;

 }

 nav{
   margin-top: 10px;
   width:100%;
   display: flex;
   flex-direction: column;
   align-items: center;
   text-align: center;
   padding: 0 50px;
 }
 nav > ul {
   width:35vw;
   display: flex;
   justify-content: space-around;
 }
 nav ul li {
   padding-bottom: 5px;
   list-style: none;
 }

 nav ul li a {
   color:black;
   text-decoration: none;
   font-weight: bold;
 }
 
 #hero input[type='email']{
   max-width: 275;
   width:100%;
   padding: 5px;
   margin-top: 20px;
 }

 #hero input[type='submit']{
   max-width: 150px;
   width: 100%;
   height: 30px;
   margin: 15px 0px;
   border: 0;
   background-color: yellowgreen;
 }

 .btn{
   padding: 0 20px;
   font-size: 1em;
   font-weight: 900;
   text-transform: uppercase;
   border-radius: 2px;
   background: transparent;
   cursor: pointer;
 }

 #hero{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  height: 200px;
  margin-top: 50px;
 }
.container{
  max-width: 1000px;
  width: 100%;
  margin: 0 auto;
}

#features{
  margin-top: 30px;
}
.grid{
  display:flex;
}
#features .icon{
  display: flex;
  align-items: center;
  justify-content: center;
  height: 125px;
  width: 20vw;
  color:rgb(134, 202, 32);
}

#features .desc {
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 125px;
  width: 80vw;
  padding: 5px;
}
#how-it-works {
  margin-top: 50px;
  display: flex;
  justify-content: center;
}

#how-it-works > iframe {
max-width: 560px;
width: 100%;
}

#pricing{
  margin-top: 60px;
  display: flex;
  justify-content: center;
}
.product{
  display: flex;
  flex-direction:column;
  align-items:center;
  text-align:center;
  border: 1px solid black;
  border-radius: 3px;
  width: 100%;
  max-width: 300;
  margin: 0 auto;
  margin-bottom: 10px;
}
.product > .level {
  background-color: #ddd;
  color: black;
  padding: 15px 0;
  width: 100%;
  text-transform: uppercase;
  font-weight: 700;
}
.product > h2 {
  margin-top: 15px;
}
.product > ol {
margin: 15px 0;
}
.product > ol > li{
  padding: 5px 0;
}

li {
list-style: none;
}
.product > button{
  border: 0;
  margin: 15px 0;
  background-color: yellowgreen;
  font-weight: 400;
}
.btn {
  height: 40px;
  padding: 0 20px;
  font-size: 1em;
  text-transform: uppercase;
  border-radius: 2px;
  background: transparent;
  cursor: pointer;
}
footer {
  margin-top: 30px;
  background-color: #ddd;
  padding: 20px;
}
footer > ul{
  display: flex;
  justify-content: flex-end;
}
footer > ul > li{
  padding: 0 10px;
}
li {
  list-style: none;
}

a{
  color: black;
  text-decoration: none;
}
footer > span {
  margin-top: 5px;
  display: flex;
  justify-content:flex-end;
  font-size: 0.9em;
  color: #444;
}
@media (max-width:800px)
.product{
  max-width:300px;
}

