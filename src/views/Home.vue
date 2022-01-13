<template>
  <div class="container" id="container">
    <div id="signUpContainer" class="form-container sign-up-container">
      <form action="#">
        <h1>Create Account</h1>
        <div class="social-container">
          <a href="#" class="social">
            <i class="fab fa-facebook-f"></i>
          </a>
          <a href="#" class="social">
            <i class="fab fa-google-plus-g"></i>
          </a>
          <a href="#" class="social">
            <i class="fab fa-linkedin-in"></i>
          </a>
        </div>
        <span>or use your email for registration</span>
        <input type="text" placeholder="Name" />
        <input type="email" placeholder="Email" />
        <input type="password" placeholder="Password" />
        <button>Sign Up</button>
      </form>
    </div>
    <div id="signInContainer" class="form-container sign-in-container">
      <form action="#">
        <h1>Sign in</h1>
        <div class="social-container">
          <a href="#" class="social">
            <i class="fab fa-facebook-f"></i>
          </a>
          <a href="#" class="social">
            <i class="fab fa-google-plus-g"></i>
          </a>
          <a href="#" class="social">
            <i class="fab fa-linkedin-in"></i>
          </a>
        </div>
        <span>or use your account</span>
        <input type="email" placeholder="Email" />
        <input type="password" placeholder="Password" />
        <a href="#">Forgot Password</a>
        <button>Sign in</button>
      </form>
    </div>
    <div id="overlayContainer" class="overlay-container">
      <div class="overlay">
        <div class="overlay-panel overlay-left">
          <h1>Welcome Back!</h1>
          <p>To keep connected please login with your personal info</p>
          <button
            @click="toggleSignIn('right-panel-active')"
            class="ghost"
            id="signIn"
          >
            Sign In
          </button>
        </div>
        <div class="overlay-panel overlay-right">
          <h1>Hello, Friends</h1>
          <p>Enter Your details to journey with us</p>
          <button
            @click="toggleSignUp('right-panel-active')"
            class="ghost"
            id="signUp"
          >
            Sign Up
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: "Home",
  components: {},
  data: () => {
    return {};
  },
  methods: {
    toggleSignUp(className) {
      const container = document.getElementById("container");
      container.classList.add(className);
    },
    toggleSignIn(className) {
      const container = document.getElementById("container");
      container.classList.remove(className);
    },
  },
  // mounted() {
  //   this.toggleViews("right-panel-active");
  // },
};
</script>
<style lang="scss"></style>
