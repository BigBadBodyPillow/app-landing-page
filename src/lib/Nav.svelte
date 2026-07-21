<!-- svelte-ignore a11y_invalid_attribute -->
<div class="navbar container">
  <!-- logo -->
  <div class="logo roboto-mono">
    <a href="#">Logo</a>
  </div>

  <!-- quick access navigation -->
  <nav>
    <li><a href="#">Home</a></li>
    <li><a href="#">About</a></li>
    <li><a href="#">Contact</a></li>
  </nav>

  <!-- download -->
  <button id="download">Download </button>
</div>

<style>
  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 3rem;

    /* prettier-ignore */
    .logo {
      font-size: 3rem;
      line-height: 4rem;
      &:hover {color: var(--accent)}
      a:hover {text-decoration: none}
    }

    /* prettier-ignore */
    a {text-decoration: none;}
    a:hover {
      text-decoration: underline;
      color: var(--accent);
    }

    nav {
      display: flex;
      gap: 1rem;
      flex: 1;
      /* prettier-ignore */
      li {list-style: none}
    }
  }
</style>
