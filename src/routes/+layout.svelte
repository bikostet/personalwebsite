<script lang="ts">
import "../app.css";
import { afterNavigate } from "$app/navigation";
	let { children } = $props();
	let cardEl: HTMLElement;
	afterNavigate(() => {
    cardEl?.scrollTo({ top: 0 });
  });
</script>

<div class="stage">
  <section class="card" bind:this={cardEl}>
	{@render children()}
    <nav class="menu">
      <a class="menu__item" href="/">Home</a>
      <a class="menu__item" href="/about">About</a>
      <a class="menu__item" href="/cv_Kostet.pdf" target="_blank">CV</a>
      <a class="menu__item" href="https://scholar.google.com/citations?user=pGbCGogAAAAJ" target="_blank" rel="noopener noreferrer">Publications</a>
      <a class="menu__item" href="https://github.com/bikostet" target="_blank" rel="noopener noreferrer">GitHub</a>
      <a class="menu__item" href="https://www.linkedin.com/in/bilal-kostet-8b88691b6/" target="_blank" rel="noopener noreferrer">LinkedIn</a>
    </nav>
  </section>
</div>

<style>
	.menu {
    display: flex;
    width: 100%;
    align-items: baseline;
    justify-content: center;
    gap: clamp(0.2rem, 2.1cqi, 4rem);
    padding-top: clamp(0.2rem, 0.5cqi, 0.6rem);
    font-size: clamp(0.65rem, 3.2cqi, 1.1rem);
    flex-wrap: wrap;
  }

  .menu__item {
    color: var(--ink);
    text-decoration: none;
    padding: 0.4rem 0.2rem;
    border-bottom: 1px solid transparent;
	filter:
    drop-shadow(0px 1px 0px rgba(255, 255, 255, 0.75))
  	drop-shadow(0px -0.5px 0px rgba(0, 0, 0, 0.2));
  }

  .menu__item:hover {
    border-bottom-color: rgba(0,0,0,0.35);
  }

  .menu__item:focus-visible {
    outline: 2px solid rgba(0,0,0,0.35);
    outline-offset: 3px;
    border-radius: 4px;
  }

.card {
  width: min(780px, calc(100% - 6rem));
  aspect-ratio: 3.5 / 2;
  max-height: 90vh;
  overflow: auto;
  border: 1px solid var(--paper-edge);
  box-shadow:
    0 1px 0 rgba(0,0,0,0.04),
    0 18px 45px rgba(0,0,0,0.10);
  padding: clamp(1.2rem, 3vw, 2.2rem);
  padding-left: 2.2rem;
  padding-right: 2.0rem;
  display: grid;
  grid-template-rows: auto 1fr auto;
  gap: clamp(0.6rem, 2cqi, 1rem);
  container-type: inline-size;

  background-image: url("/textures/paper.png");
  background-size: cover;
  background-position: center;
}

  .stage {
  min-height: 100%;
  display: grid;
  place-items: center;
} 
</style>