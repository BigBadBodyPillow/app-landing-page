<script lang="ts">
  import ListItem from './ListItem.svelte';
</script>

<section class="container">
  <h2 class="roboto-mono-title">Frequently Asked Questions</h2>
  <ul>
    <ListItem
      question="A question thats asked a lot?"
      answer="An answer that answers the question that was asked above"
    />
    <ListItem
      question="Whoa look at that a second question.What about it?"
      answer="Well its kind hard to think of things to say about something that doesnt exist and thats entirely made up of placeholders"
    />

    <ListItem
      question="Lorem ipsum dolor sit?"
      answer="Lorem ipsum dolor sit amet, consectetur adipisicing elit."
    />
    <ListItem
      question="Lorem ipsum dolor sit?"
      answer="Lorem ipsum dolor sit amet, consectetur adipisicing elit. At nemo magnam velit facere quaerat corrupti, saepe ab earum mollitia dolore quia voluptatibus. Possimus at, rem atque minima ducimus facere eligendi!"
    />
    <ListItem
      question="Lorem ipsum dolor sit?"
      answer="Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur repellat voluptas reiciendis."
    />
    <ListItem
      question="Lorem ipsum dolor sit?"
      answer="Lorem ipsum dolor sit amet, consectetur adipisicing elit."
    />
    <ListItem
      question="Lorem ipsum dolor sit?"
      answer="Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur repellat voluptas reiciendis."
    />
    <ListItem
      question="Lorem ipsum dolor sit?"
      answer="Lorem ipsum dolor sit amet, consectetur adipisicing elit."
    />
    <ListItem
      question="Lorem ipsum dolor sit?"
      answer="Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur repellat voluptas reiciendis."
    />
  </ul>
</section>

<style>
  .container {
    text-align: left;
    padding: 2rem 0;

    h2 {
      font-size: xx-large;
      margin: 0 0 2rem 0;
    }

    ul {
      margin: 0;
      padding: 0;
      padding-block: 1rem;
      column-count: 2;
      column-gap: 1.5rem;
    }
  }
</style>
