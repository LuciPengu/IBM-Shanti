

<div class="footerTopMargin"></div>
<div class="footer">

  <button class="footerButton">
    <div class="footerIcon">🌅</div>
    Today
  </button>
  <button class="footerButton">
    <div class="footerIcon">📈</div>
    Stats
  </button>
  <button class="footerButton">
    <div class="footerIcon">🔧</div>
    Settings
  </button>
</div>



<style>
  .footerTopMargin{
    margin-top: 4em;
  }
  .footer {
    bottom: 0;
    left: 0; 
    right: 0; 
    position: fixed;
    border-top: solid;
    border-width: 0.2em;
    border-color: hsla(276, 100%, 40%, 1);
    background-color: #23272a;

  }

  .footerButton {
    font-family: inherit;
    font-size: inherit;
    text-align: left;
    background-color: transparent;
    color: white;
    border: none;
    width: 6em;
    min-height: 4em;
    text-align: center;
  }

  .footerIcon{
    font-size: 1.5rem;
  }

  button:active {
    background-color: #2f3136;
  }

</style>
