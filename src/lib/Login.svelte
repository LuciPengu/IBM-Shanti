<script>
  import { fade } from 'svelte/transition';
  import Logo from './Logo.svelte'

</script>


<Logo/>
<div class="login">
  <div class="loginTitle">
    Login
  </div>
  <input placeholder="Email" class="loginInput">
  <input placeholder="Password" class="loginInput">
  <button class="loginButton">
    Login
  </button>  
</div>

<style>
  .loginTitle {
    color: white;
    font-size: 2rem;
    font-weight: bold;
  }
  .loginInput {
    font-family: inherit;
    font-size: inherit;
    border: none;
    border-radius: 0.75em;
    text-align: center;
    width: 100%;
    height: 3em;

  }
  .loginButton {
    font-family: inherit;
    font-size: inherit;
    color: white;
    padding: 0em;
    width: 100%;
    border: none;
    border-radius: 0.75em;
    height: 3em;
    text-align: center;
    background: linear-gradient(90deg, hsla(276, 100%, 40%, 1) 0%, hsla(264, 68%, 40%, 1) 100%);  
  }
  .login {
    line-height: 4em;
    font-family: inherit;
    font-size: inherit;
    color: white;
    padding: 2em;
    border: none;
    border-radius: 0.75em;
    width: 70%;
    height: 17em;
    background: transparent;
    position: absolute;
    background-color: #23272a;
    max-width: 25em;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  button:active {
    filter: brightness(85%);
  }
</style>
