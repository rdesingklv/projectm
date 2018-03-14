<!doctype html>
<html>
<head><title>Bootstrap page</title>
<style>
*, *:before, *:after {
  box-sizing: border-box;
}
html {
  overflow-y: scroll;
}
body {
  background: #c1bdba;
  font-family: 'Titillium Web', sans-serif;
}
a {
  text-decoration: none;
  color: #1ab188;
  transition: 0.5s ease;
}
a:hover {
  color: #179b77;
}
.form {
  background: rgba(19, 35, 47, .9);
  padding: 40px;
  max-width: 600px;
  margin: 40px auto;
  border-radius: 4px;
  box-shadow: 0 4px 10px 4px rgba(19, 35, 47, .3);
}
.tab-group {
  list-style: none;
  padding: 0;
  margin: 0 0 40px 0;
}
.tab-group:after {
  content: "";
  display: table;
  clear: both;
}
.tab-group li a {
  display: block;
  text-decoration: none;
  padding: 15px;
  background: rgba(160, 179, 176, .25);
  color: #a0b3b0;
  font-size: 20px;
  float: left;
  width: 50%;
  text-align: center;
  cursor: pointer;
  transition: 0.5s ease;
}
.tab-group li a:hover {
  background: #179b77;
  color: #fff;
}
.tab-group .active a {
  background: #1ab188;
  color: #fff;
}
.tab-content > div:last-child {
  display: none;
}
h1 {
  text-align: center;
  color: #fff;
  font-weight: 300;
  margin: 0 0 40px;
}
label {
  position: absolute;
  transform: translateY(6px);
  left: 13px;
  color: rgba(255, 255, 255, .5);
  transition: all 0.25s ease;
  -webkit-backface-visibility: hidden;
  pointer-events: none;
  font-size: 22px;
}
label .req {
  margin: 2px;
  color: #1ab188;
}
label.active {
  transform: translateY(50px);
  left: 2px;
  font-size: 14px;
}
label.active .req {
  opacity: 0;
}
label.highlight {
  color: #fff;
}
input, textarea {
  font-size: 22px;
  display: block;
  width: 100%;
  height: 100%;
  padding: 5px 10px;
  background: none;
  background-image: none;
  border: 1px solid #a0b3b0;
  color: #fff;
  border-radius: 0;
  transition: border-color 0.25s ease, box-shadow 0.25s ease;
}
input:focus, textarea:focus {
  outline: 0;
  border-color: #1ab188;
}
textarea {
  border: 2px solid #a0b3b0;
  resize: vertical;
}
.field-wrap {
  position: relative;
  margin-bottom: 40px;
}
.top-row:after {
  content: "";
  display: table;
  clear: both;
}
.top-row > div {
  float: left;
  width: 48%;
  margin-right: 4%;
}
.top-row > div:last-child {
  margin: 0;
}
.button {
  border: 0;
  outline: none;
  border-radius: 0;
  padding: 15px 0;
  font-size: 2rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  background: #1ab188;
  color: #fff;
  transition: all 0.5s ease;
  -webkit-appearance: none;
}
.button:hover, .button:focus {
  background: #179b77;
}
.button-block {
  display: block;
  width: 100%;
}
.forgot {
  margin-top: -20px;
  text-align: right;
}

</style>
<body>
<div class="form">
      
      <ul class="tab-group">
        <li class="tab active"><a href="#signup">Sign Up</a></li>
        <li class="tab"><a href="#login">Log In</a></li>
      </ul>
      
      <div class="tab-content">
        <div id="signup">   
          <h1>Sign Up here</h1>
          
          <form action="/" method="post">
          
          <div class="top-row">
            <div class="field-wrap">
           
              <input type="text" placeholder="First Name"required autocomplete="off" />
            </div>
        
            <div class="field-wrap">
           
              <input type="text"placeholder="Last Name"required autocomplete="off"/>
            </div>
          </div>

          <div class="field-wrap">
            
            <input type="email"placeholder="E-Mail"required autocomplete="off"/>
          </div>
          
          <div class="field-wrap">
            <label>
          
            </label>
            <input type="password"placeholder="Password"required autocomplete="off"/>
          </div>
          
          <button type="submit" class="button button-block"/>Create Account</button>
          
          </form>

        </div>
        
        <div id="login">   
          <h1>Welcome Back!</h1>
          
          <form action="/" method="post">
          
            <div class="field-wrap">
            <label>
              
            </label>
            <input type="email"placeholder="E-Mail"required autocomplete="off"/>
          </div>
          
          <div class="field-wrap">
            <label>
              Password
            </label>
            <input type="password"required autocomplete="off"/>
          </div>
          
          <p class="forgot"><a href="#">Forgot Password?</a></p>
          
          <button class="button button-block"/>Log In</button>
          
          </form>

        </div>
        
      </div><!-- tab-content -->
      
</div> <!-- /form -->
</body>
</html>
