<script>
  import ThirdNav from './ThirdNav.svelte';
  export let category;
</script>

<!-- markup (zero or more items) goes here -->
<nav>
  <ul>
    <li on:mouseover={e => category = 'quizz'}>
      <a href="#">
        Quizz
      </a>
    </li>
    <li on:mouseover={e => category = 'challenge'}>
      <a href="#">
        Challenge
      </a>
    </li>
    <li on:mouseover={e => category = 'leaderboard'}>
      <a href="#">
        Leaderboard
      </a>
    </li>
    <li on:mouseover={e => category = 'review'}>
      <a href="#">
        Review
      </a>
    </li>
    <li on:mouseover={e => category = 'debug'}>
      <a href="#">
        Debug
      </a>
    </li>
    <li on:mouseover={e => category = 'cursus'}>
      <a href="#">
        cursus
      </a>
    </li>
    <li on:mouseover={e => category = 'flashcard'}>
      <a href="#">
        flashcard
      </a>
    </li>
  </ul>
</nav>

<ThirdNav category={category} />

<style lang="scss">
  nav {
    position: absolute;
    background-color: #D8D8D8;
    left: 61px;
    width: 200px;
    height: 100%;
    max-height: calc(100vh - 70px);
    border-right: 1px solid var(--main-color);

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
