<script>
  import { fade } from 'svelte/transition';
  let user = "Luci"
  let data = [
    {
      title:"No Strings Attatched",
      preview:"https://www.smashbros.com/images/og/toon_link.jpg",
      time: "12 mins",
      type: "meditaion"

    },
    {
      title:"Treat Yourself to 5 Gentle Breaths",
      preview:"https://www.smashbros.com/images/og/toon_link.jpg",
      time: "5 mins",
      type: "breathing"
    },
    {
      title:"tHEY sAY yEAT kEEP on ",
      preview:"https://www.smashbros.com/images/og/toon_link.jpg",
      time: "40 mins",
      type: "YEATING"

    },
    {
      title:"STRAIGHT UP MUrdalicious",
      preview:"https://www.smashbros.com/images/og/toon_link.jpg",
      time: "2 mins",
      type: "holding"
    }
  ]
</script>
  <div class="dailyHeader">
      Good Evening, {user}
  </div>

	{#each data as lesson, i}
    <div class="lessonGeneralTime">
      
      {#if i == 0}
      	Morning
      {:else if i == 1}
      	Afternoon
      {:else if i == 3}
      	Evening
      {/if}
    </div>
		<div class="lesson">
      <button class="lessonButton" transition:fade>
        <img src={lesson.preview} class="lessonPreview" alt="background image" />
        <div class="lessonTitle">
          {lesson.title}          
        </div>
        <div class="lessonTime">🕑 {lesson.time}</div>
        <div class="lessonType">🎤 {lesson.type}</div>
		  </button>  
    </div>
	{/each}

<style>
  .lessonGeneralTime{
    color: white;
    font-size: 1.1rem;
    font-weight: bold;
  }
  .dailyHeader{
    color: white;
    margin-bottom: 2em;
    font-size: 1.2rem;
    line-height: 1.7em;
    font-weight: bold;
    padding: 1em;    
    border-radius: 0.75em;
    background: linear-gradient(90deg, hsla(276, 100%, 40%, 1) 0%, hsla(264, 68%, 40%, 1) 100%);

  }
  .lessonButton {
    font-family: inherit;
    font-size: inherit;
    color: white;
    text-align: left;
    padding: 0.7em;
    border: none;
    border-radius: 0.75em;
    width: 18em;
    margin: 0.7em;
    min-height: 4em;
    background: linear-gradient(90deg, hsla(276, 100%, 40%, 1) 0%, hsla(264, 68%, 40%, 1) 100%);  
  }

  .lessonPreview {
    width: 5em;
    object-fit: fill;
    float: right;
    border-radius: 0.75em;
    margin-left: 0.3em;
  }
  .lessonTitle{
    font-weight: bold;
  }

  button:active {
    filter: brightness(85%);
  }
</style>
