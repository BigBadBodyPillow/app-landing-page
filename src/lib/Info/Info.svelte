<script>
  import Card from './Card.svelte';
</script>

<section>
  <div class="container inter">
    <!-- title -->
    <!-- <h2 class="roboto-mono-title">Info Section</h2> -->
    <!-- card display -->
    <div class="display">
      <!-- card 1-->
      <Card
        title="This is an example of a feature"
        imageSource=""
        imageAlt="functionality showcase"
        flipped={false}
      >
        <p>
          More info about this feature. it's really cool and is really impressive, im sure... maybe.
        </p>
        <p>
          Extra text to fill the space because i dont know what to say and dont want to use Lorem
          Ipsum because i think sometimes it makes things look weird.
        </p>
      </Card>
      <!-- card 2-->
      <Card title="Feature 2" imageSource="" imageAlt="functionality showcase" flipped={true}>
        <p>
          Showcase of feature2. Whoa that a really cool feature. Okay fine i give up, ill use Lorem
          Ipsum. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium illum
          repellendus dolore, sed quasi in aspernatur recusandae at esse? Dolore, vel atque. Placeat
          ratione nihil similique. Vitae reiciendis magnam dolorum, voluptates voluptatibus
          voluptatum.
        </p>
      </Card>
      <!-- card 3 -->
      <Card title="Showcase of feature 3" imageSource="" imageAlt="showcase 3 ">
        <p>
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Veniam quod nesciunt nihil
          doloribus perspiciatis officia nemo eligendi odio, voluptates minima hic libero vitae
          doloremque consectetur corrupti excepturi cumque voluptatem in ex distinctio iusto ratione
          reprehenderit sequi sunt. Facilis, itaque quaerat?
        </p>
      </Card>
    </div>
  </div>
</section>

<style>
  section {
    max-width: 1640px;
    margin-inline: auto;
    margin-block: 4rem;
    background-color: var(--text);

    .container {
      padding: 2rem 0;
      text-align: left;
      color: var(--text-invert);

      /* h2 {
        font-size: xx-large;
        margin-bottom: 5rem;
      } */

      .display {
        display: flex;
        gap: 4rem;
        flex-direction: column;

        p {
          margin: 0;
        }
      }
    }
  }
</style>
