<script>
  import SecondNav from './SecondNav.svelte';
  let secondNavVisible = false;
  let category;

</script>

<!-- markup (zero or more items) goes here -->
<div on:mouseover={e => secondNavVisible = true} on:mouseleave={e => secondNavVisible = false}>
  <nav>
    <ul>
      <li on:mouseover={e => category = 'quizz'}>
        <a href="#">
          <i class="fas fa-chess-queen"></i>
        </a>
      </li>
      <li on:mouseover={e => category = 'challenge'}>
        <a href="#">
          <i class="fas fa-chess-queen"></i>
        </a>
      </li>
      <li on:mouseover={e => category = 'leaderboard'}>
        <a href="#">
          <i class="fas fa-chess-queen"></i>
        </a>
      </li>
      <li on:mouseover={e => category = 'review'}>
        <a href="#">
          <i class="fas fa-chess-queen"></i>
        </a>
      </li>
      <li on:mouseover={e => category = 'debug'}>
        <a href="#">
          <i class="fas fa-chess-queen"></i>
        </a>
      </li>
      <li on:mouseover={e => category = 'cursus'}>
        <a href="#">
          <i class="fas fa-chess-queen"></i>
        </a>
      </li>
      <li on:mouseover={e => category = 'flashcard'}>
        <a href="#">
          <i class="fas fa-chess-queen"></i>
        </a>
      </li>
    </ul>
  </nav>

  {#if secondNavVisible }
    <SecondNav category={category} />
  {/if}
</div>

<style lang="scss">
  nav {
    position: fixed;
    background-color: #e8e8e8;
    width: 61px;
    border-right: 1px solid var(--main-color);
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    height: 100%;
    max-height: calc(100vh - 70px);
    transition: .4s;
    z-index: 1;

    ul {
      width: 100%;

      li {
        text-align: center;
        font-size: 1.8rem;
        margin: 15px 0 15px 0;
        color: var(--main-color);
      }
    }
  }
</style>
