<script lang="ts">
  let { children, title = '...', imageSource, imageAlt = '...', flipped = false } = $props();
</script>

<div class="card" class:flipped>
  <img alt={imageAlt} src={imageSource} draggable="false" />
  <div class="text">
    <h3>{title}</h3>
    <!-- usually p tags -->
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
      display: block;
      width: 100%;
      max-width: 100%;
      height: auto;
      aspect-ratio: 16/9;
      flex: 1 1 0;
      min-width: 0;
      color: var(--text);
      background-color: var(--alt);
      border: 1px solid var(--alt-border);
      object-fit: cover;
      user-select: none;
      -moz-user-select: none;
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
