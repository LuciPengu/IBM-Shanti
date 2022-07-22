<script>
  import { fade } from 'svelte/transition';
  let user = "Luci"
  let data = {
    hours:"30"
  }
</script>
  <div class="dailyHeader">
    <div class="greeting">
      These are your statistics {user}
    </div>
    <div class="greeting">
      You have spent {data.hours} meditating
    </div>
  </div>

<style>

  .dailyHeader{
    color: white;
    margin-bottom: 2em;
    line-height: 1.7em;
  }
</style>
