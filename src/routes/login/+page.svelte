
  <h2>Test Login with Session #1: Sign in/up Form</h2>
  <div class="container" id="container">
    <div class="form-container sign-up-container">
      <form action="#">
        <h1>Create Account</h1>
        <div class="social-container">
          <a href="" class="social">
            <i class="fab fa-facebook-f"></i>
          </a>
          <a href="" class="social">
            <i class="fab fa-google-plus-g"></i>
          </a>
          <a href="" class="social">
            <i class="fab fa-linkedin-in"></i>
          </a>
        </div>
        <span>Or use your email for registration</span>
        <input id="nome" type="text" placeholder="Name" />
        <input id="email" type="email" placeholder="Email" />
        <input id="password" type="password" placeholder="Password" />
        <button id="signUp2">Sign Up</button>
      </form>
    </div>


    <div class="form-container sign-in-container">
      <form action="#">
        <h1>Sign in</h1>
        <div class="social-container">
          <a href="" class="social"><i class="fab fa-facebook-f"></i></a>
          <a href="" class="social"><i class="fab fa-google-plus-g"></i></a>
          <a href="" class="social"><i class="fab fa-linkedin-in"></i></a>
        </div>
        <span>Or use your account</span>
        <input type="email" id="email2" placeholder="Email" />
        <input type="password" id="password2" placeholder="Password" />
        <a href="">Forgot your password?</a>
        <button id="signInEnter">Sign In</button>
      </form>
    </div>


    <div class="overlay-container">
      <div class="overlay">
        <div class="overlay-panel overlay-left">
          <h1>Welcome Back!</h1>
          <p>To keep connected with us please login with your personal info</p>
          <button class="ghost" id="signIn">Sign In</button>
        </div>
        <div class="overlay-panel overlay-right">
          <h1>Hello, Friend!</h1>
          <p>Enter your personal details and start journey with us</p>
          <button class="ghost" id="signUp">Sign Up</button>
        </div>
      </div>
    </div>
  </div>

  <footer>
    <p>
      Created <i class="fa fa-fire"></i> by
      <a target="_blank" href="https://www.linkedin.com/in/fabio-arrivabene-92a846243/">Fabio Arrivabene</a>
    </p>
  </footer>
<script src="script.js"></script>