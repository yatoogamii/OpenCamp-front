<script>
  export let category = 'quizz';
</script>

<!-- markup (zero or more items) goes here -->
<nav>
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
  background-color: #cccccc;
  left: 261px;
  width: 200px;
  height: 100%;
  max-height: calc(100vh - 70px);
  border-right: 1px solid var(--main-color);

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
