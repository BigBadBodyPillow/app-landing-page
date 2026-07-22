<script>
  import profilePicture from '../assets/profile/n-i-x-e-u-blood-or-blush-b-tt.jpg';
</script>

<!-- svelte-ignore a11y_invalid_attribute -->
<section class="navbar container">
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

  <!-- rightmost side -->
  <div class="rightmost">
    <!-- download -->
    <button id="download">Download </button>

    <!-- profile -->
    <div class="profile">
      <img alt="profile" src={profilePicture} draggable="false" />
    </div>
  </div>
</section>

<style>
  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 3rem;
    margin-block: 1rem;

    /* prettier-ignore */
    .logo {
      font-size: 3rem;
      line-height: 4rem;
      &:hover {color: var(--accent)}
      a:hover,a:focus-visible {text-decoration: none}
    }

    /* prettier-ignore */
    a {text-decoration: none; }
    a:hover,
    a:focus-visible {
      text-decoration: underline;
      color: var(--accent);
    }

    nav {
      display: flex;
      gap: 1rem;
      flex: 1;
      li {
        list-style: none;
        transform-origin: bottom bottom;
      }
    }

    .rightmost {
      display: flex;
      align-items: center;
      gap: 1rem;

      .profile {
        border-radius: 100%;
        border: 2px solid var(--alt-border);

        img {
          width: 3rem;
          height: 3rem;
          aspect-ratio: 1/1;
          object-fit: cover;
          overflow: hidden;
          display: flex;
          justify-content: center;
          align-items: center;
          border-radius: inherit;
          user-select: none;

          font-size: 0.7rem;
          cursor: pointer;
          background-color: var(--alt);
        }
      }
    }
  }
</style>
