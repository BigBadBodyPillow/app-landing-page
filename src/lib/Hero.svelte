<script>
  import HeroImage from '../assets/Hero/153fd2546a293ae8e555353e54220df2.png';
</script>

<section class="hero">
  <!-- inside container (has the  max width) -->
  <div class="container">
    <!-- image -->
    <img alt="Hero" src={HeroImage} draggable="false" />

    <!-- card -->
    <div class="text-card">
      <div class="background-layer base"></div>
      <div class="background-layer hover"></div>

      <!-- text -->
      <div class="text-content">
        <h1 class="roboto-mono">Heading</h1>
        <p>
          Some text about something or something else. More words to fill the empty space, and make
          it look like this is important.
        </p>
      </div>

      <!-- buttons -->
      <div class="button-group">
        <button id="signup">Sign Up</button>
        <button id="download">Download</button>
      </div>
    </div>
  </div>
</section>

<style>
  .hero {
    .container {
      display: flex;
      justify-content: space-between;
      gap: 1.25rem;

      img {
        width: 550px;
        height: 550px;
        aspect-ratio: 1/1;

        display: flex;
        align-items: center;
        justify-content: center;
        user-select: none;

        background-color: var(--alt);
        border: 1px solid var(--alt-border);
      }

      .text-card {
        position: relative;
        display: flex;
        flex-direction: column;
        justify-content: end;
        flex: 1;

        overflow: hidden;
        text-align: left;
        padding: 2rem;
        background-color: var(--alt);
        border: 1px solid var(--alt-border);

        cursor:
          url('../assets/icons/si--star-fill.svg') 8 1,
          auto;
        isolation: isolate;

        .background-layer {
          position: absolute;
          inset: 0;
          background-position: center;
          background-repeat: no-repeat;
          transition: opacity 0.7s ease;
          z-index: 0;
        }

        .background-layer.base {
          background-image: url('../assets/Hero/pexels-kuldeep-nath-1914208466-28784153.jpg');
          background-size: 100vw 100vh;
          background-attachment: fixed;
        }

        .background-layer.hover {
          background-image: url('../assets/Hero/ball.gif');
          background-size: 150%;
          background-attachment: local;
          opacity: 0;
        }

        .text-content {
          margin-bottom: 2rem;
          position: relative;
          z-index: 1;
          filter: blur(3px);
        }

        &::after {
          content: '';
          position: absolute;
          display: flex;
          inset: 0;
          background: radial-gradient(200% 100% at top, transparent 50%, black);
          opacity: 0;
          transition: opacity 0.7s;
          z-index: 0;
        }

        &:hover {
          .background-layer.base {
            opacity: 0;
          }

          .background-layer.hover {
            opacity: 1;
          }

          .text-content {
            filter: blur(0);
          }

          &:after {
            opacity: 1;
          }
        }

        .button-group {
          position: relative;
          z-index: 1;
          display: flex;
          gap: 0.8rem;
          justify-content: center;
          button {
            transition: color 0.5s;
          }
        }

        &:hover .button-group button {
          color: var(--text);
          cursor:
            url('../assets/icons/flowbite--star-solid.svg') 8 1,
            auto;
        }
      }
    }
  }

  @starting-style {
    .text-card {
      &::before {
        content: '';
        border: none;
      }
    }
  }
</style>
