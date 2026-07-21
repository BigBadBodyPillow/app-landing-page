# New things learned in this project

- Svelte config option to force svelte5 syntax :
  compilerOptions: {
  runes: true
  }

- CSS @functions (not broadly supported) :
  @function --invert-colour(--colour) {
  result: hsl(from var(--colour) calc(h + 180) s calc(100 - l));
  }
