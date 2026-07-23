<script lang="ts">
  type ListItemTypes = {
    question: string;
    answer: string;
  };

  let { question, answer }: ListItemTypes = $props();
</script>

<li>
  <p class="question space-grotsk">{question} :</p>
  <p class="answer">{answer}</p>
</li>

<style>
  p {
    margin: 0;
  }
  p:first-child {
    margin-bottom: 2px;
  }
  li {
    margin-block: 1rem;
    break-inside: avoid;
  }

  .question {
    font-weight: bold;
    font-family: var(--space-grotesk);
    /* font-size: 1.25rem; */
  }
  .answer {
    color: hsl(from var(--text) h s calc(l * 0.8));
  }
</style>
