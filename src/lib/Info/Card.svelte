<script lang="ts">
  let { children, title = '...', imageSource, imageAlt = '...', flipped = false } = $props();
</script>

<div class="card" class:flipped>
  <img alt={imageAlt} src={imageSource} draggable="false" />
  <div class="text">
    <h3>{title}</h3>
    {@render children()}
  </div>
</div>

<style>
  .card {
    display: flex;
    gap: 1.25rem;
    &.flipped {
      flex-direction: row-reverse;
    }

    img {
      aspect-ratio: 16/9;
      display: flex;
      flex: 1;
      justify-content: center;
      align-items: center;
      color: var(--text);
      background-color: var(--alt);
      border: 1px solid var(--alt-border);
    }
    .text {
      flex: 1;
      display: flex;
      flex-direction: column;
      justify-content: center;
      gap: 0;
    }

    h3 {
      font-family: var(--space-grotesk);
      font-weight: bold;
      font-size: 1.25rem;
    }
  }
</style>
