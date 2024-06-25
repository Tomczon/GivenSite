
<template style = "scroll-behavior = smooth;">
  <body>
    <div>
      <header>
          <img src="~assets/Given_logo.png" alt="Logo" class="logo" />
          <div class = "nav">
            <button class="button1" onclick="document.getElementById('banner').scrollIntoView();">Home</button>
            <button class="button1" onclick="document.getElementById('About').scrollIntoView();">About</button>
            <button class="button1" onclick="document.getElementById('Members').scrollIntoView();">Members</button>
            <button class="button1" onclick="document.getElementById('Music').scrollIntoView();">Music</button>
            <button class="button1" onclick="document.getElementById('Contact').scrollIntoView();">Contact</button>
        </div>
      </header>
      <slot />
      <footer>
        <p>&copy; 2024 Given. All rights reserved.</p>
      </footer>
    </div>
  </body>
  </template>
  
  <style scoped>
* {
  font-family: Arial, Helvetica, sans-serif;
}

  body{
    background-image: -webkit-linear-gradient(top, rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url(assets/group_photo.png);
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-size: cover; 
    background-position: top center;
    scroll-behavior: smooth;
    }

  header {
    display: flex;
    justify-content: left;
    align-items: center;
    background: #333;
    color: #fff;
    position: fixed;
    width: 98.5%;
    scroll-behavior: smooth;
  }
  
  nav {
    display: flex;
    align-items: center;
  }
  
  .logo {
    max-height: 50px;
    margin-right: 20px;
    margin-left: 10px;
    padding: 10px 10px;
  } 
  
  a {
    color: #fff;
    text-decoration: none;
  }
  
  a:hover {
    text-decoration: underline;
  }
  
  footer {
    text-align: center;
    padding: 10px 0;
    background: #333;
    color: #fff;
    position: fixed;
    width: 98.5%;
    bottom: 0;
  }

  .button1
  {
    background-color: #333;
    border: none;
    padding: 25px 25px;
    font-size: 1vw; 
    color: white;
    height: 100%;
    transition: background-color 0.3s ease;
    cursor: pointer;

  }

  button:hover {
    color: #923131;
    background-color: #292828;
  }
  </style>