<script>
  // your script goes here
</script>

<style lang="scss">
  nav {
    background-color: var(--main-color);
    display: flex;
    height: 70px;
    border-bottom: 1px solid var(--main-color);

    div {
      background-color: #fff;
      display: flex;
      justify-content: flex-start;
      align-items: center;
      padding: 10px;
      width: 60px;
      position: relative;

      h2 {
        position: absolute;
        left: 80px;
        white-space: nowrap;
        color: var(--main-color);
      }

      img {
        width: 40px;
        height: 45px;
      }
    }

    ul {
      margin-left: auto;
      margin: 0 20px 0 auto;
      display: flex;
      align-items: center;
      color: white;

      li {
        margin: 5px 8px;
      }
    }
  }
</style>

<!-- markup (zero or more items) goes here -->
<nav>
  <div>
    <img src="./logo-dark.png" alt="Open camp logo">
    <h2>Open Camp</h2>
  </div>
  <ul>
    <li>
      <a href="#"> À propos </a>
    </li>
    <li>
      <a href="#"> Contact </a>
    </li>
  </ul>
</nav>
