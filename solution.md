# javascript Project Related To DOM 
## BackgroundColor Changer 
## Solution
background has change when button clicked
```Html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link rel="stylesheet" href="style.css" />
    <title>JavaScript Background Color Switcher</title>
  </head>
  <body>
    <nav class="nav">
      <a href="/" aria-current="page">Home</a>
      <a href="/page2.html">Other Page</a>
      
    </nav>
    <div class="canvas">
      <h1>Color Scheme Switcher</h1>
      <span class="button" id="grey"></span>
      <span class="button" id="white"></span>
      <span class="button" id="blue"></span>
      <span class="button" id="yellow"></span>
      <span class="button" id="red"></span>
      <span class="button" id="green"></span>
      <span class="button" id="orange"></span>

      <h2>
        Try clicking on one of the colors above
        <span>to change the background color of this page!</span>
      </h2>
    </div>
    <script src="changer.js"></script>
  </body>
</html>
```
```css
html {
    margin: 0;
  }
  
  span {
    display: block;
  }
  .canvas {
    margin: 200px auto 100px;
    width: 80%;
    text-align: center;
    
    
  }
  
  .button {
    width: 100px;
    height: 100px;
    border: solid black 2px;
    display: inline-block;
    transition: all ease-in 1s
  }
  *{
    margin: 0;
    padding: 0;
  }
  .nav{
    position: sticky;
    margin-top: 0px;
    display: flex;
    justify-content: center;
    align-items: center;
    background:linear-gradient(red,orange);
    height: 6.5rem;
  }
  .nav a{
    font-size: 2.8rem;
    font-weight: 700;
    text-decoration: none;
    color: black;
    border: 5px solid black;
    box-shadow: 5px 5px 5px black ;
    display: block;
    margin-right: 4rem;
    width: fit-content;
    padding: 0.5rem 1rem;
    border-radius: 10px;
  }
  
  #grey {
    background: grey;
  }
  
  #white {
    background: white;
  }
  #blue {
    background: blue;
  }
  #yellow {
    background: yellow;
  }
  #red {
    background:red;
  }
  #orange {
    background: orange;
  }
  #green {
    background: green;
  }
  .button:hover{
    height: 110px;
    width: 110px;
  }
  h2{
    margin-top: 40px;
  }
  h1{
    margin-bottom: 20px;
  }

  

```






```javascript
const buttons = document.querySelectorAll('.button')
const body= document.querySelector("body")
buttons.forEach((button) => {
    button.addEventListener('click' ,(event) => {
      if(event.target.id==="grey"){
        body.style.backgroundColor= event.target.id;
      }
      if(event.target.id==='white'){
        body.style.backgroundColor=event.target.id
      }
      if(event.target.id==='blue'){
        body.style.backgroundColor=event.target.id
      }
      if(event.target.id==='yellow'){
        body.style.backgroundColor=event.target.id
      }
      if(event.target.id==='red'){
        body.style.backgroundColor=event.target.id
      }
      if(event.target.id==='green'){
        body.style.backgroundColor=event.target.id
      }
      if(event.target.id==='orange'){
        body.style.backgroundColor=event.target.id
      }

      

    })
});
  



```