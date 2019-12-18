<script>
  import ThirdNav from './ThirdNav.svelte';
  import { fly } from 'svelte/transition';
  export let category;
  let thirdNavVisible = false;
</script>

<!-- markup (zero or more items) goes here -->
<nav transition:fly={{ x: -200, duration: 500, opacity: 1}}>
  <ul>
    <li on:click={e => category = 'quizz'} on:click={e => thirdNavVisible = true}>
      <a href="#">
        Quizz
      </a>
    </li>
    <li on:click={e => category = 'challenge'} on:click={e => thirdNavVisible = true}>
      <a href="#">
        Challenge
      </a>
    </li>
    <li on:click={e => category = 'leaderboard'} on:click={e => thirdNavVisible = true}>
      <a href="#">
        Leaderboard
      </a>
    </li>
    <li on:click={e => category = 'review'} on:click={e => thirdNavVisible = true}>
      <a href="#">
        Review
      </a>
    </li>
    <li on:click={e => category = 'debug'} on:click={e => thirdNavVisible = true}>
      <a href="#">
        Debug
      </a>
    </li>
    <li on:click={e => category = 'cursus'} on:click={e => thirdNavVisible = true}>
      <a href="#">
        cursus
      </a>
    </li>
    <li on:click={e => category = 'flashcard'} on:click={e => thirdNavVisible = true}>
      <a href="#">
        flashcard
      </a>
    </li>
  </ul>
</nav>

{#if thirdNavVisible}
  <ThirdNav category={category} />
{/if}
<style lang="scss">
  nav {
    position: absolute;
    background-color: #e8e8e8;
    left: 61px;
    width: 200px;
    height: 100%;
    max-height: calc(100vh - 70px);

    ul {
      margin: 0 auto;

      li {
        font-size: 1.3rem;
        height: 35px;
        margin: 15px 0 15px 5px;
        color: var(--main-color);
        display: flex;
        align-items: center;
      }
    }
  }
</style>
