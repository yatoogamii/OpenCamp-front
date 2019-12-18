<script>
  import { fly } from 'svelte/transition';
  export let category = 'quizz';
</script>

<!-- markup (zero or more items) goes here -->
<nav in:fly={{x: -200, duration: 500, opacity: 1}} out:fly={{x: -400, duration: 500, opacity: 1}}>
  <ul>
    <li> {category} </li>
    <li> {category} </li>
    <li> {category} </li>
    <li> {category} </li>
    <li> {category} </li>
    <li> {category} </li>
    <li> {category} </li>
  </ul>
</nav>

<style lang="scss">
 nav {
  position: absolute;
  background-color: #e8e8e8;
  left: 261px;
  width: 200px;
  height: 100%;
  max-height: calc(100vh - 70px);

  ul {
    margin: 0 auto;

    li {
      font-size: 1rem;
      height: 35px;
      margin: 15px 0 15px 5px;
      color: var(--main-color);
      display: flex;
      align-items: center;
    }
  }
 }
</style>
