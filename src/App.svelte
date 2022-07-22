<script>
  import Daily from './lib/Daily.svelte'
  import Footer from './lib/Footer.svelte'
  import Stats from './lib/Stats.svelte'
  import Login from './lib/Login.svelte'


</script>

<main>
  <Daily/>
  <Footer/>
</main>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Mulish:wght@300;600&display=swap');
  :root {
    font-family: 'Mulish', sans-serif;
    background: #2f3136;
  }

  main {
    text-align: center;
    padding: 1em;
    margin: 0 auto;
  }

  img {
    height: 16rem;
    width: 16rem;
  }

  h1 {
    color: white;
    text-transform: uppercase;
    font-size: 4rem;
    font-weight: 100;
    line-height: 1.1;
    margin: 2rem auto;
    max-width: 14rem;
  }

  p {
    max-width: 14rem;
    margin: 1rem auto;
    line-height: 1.35;
  }

  @media (min-width: 480px) {
    h1 {
      max-width: none;
    }

    p {
      max-width: none;
    }
  }
</style>
