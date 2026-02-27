<svelte:head>
  <title>Bilal Kostet</title>
  <meta name="description" content="Bilal Kostet's homepage" />
</svelte:head>

<div class="stage">
  <section class="card">

    <header class="card__top">
      <div class="email">bikostet at berkeley dot edu</div>
      <div class="employer">UC Berkeley</div>
    </header>

    <div class="card__details">
        <div class="name">Bilal Kostet</div>
        <div class="role">Postdoctoral researcher</div>
        <div class="role2">in Demography</div>
    </div>

    <nav class="menu">
      <a class="menu__item" href="/">Home</a>
      <a class="menu__item" href="/about">About</a>
      <a class="menu__item" href="/cv_Kostet.pdf" target="_blank">CV</a>
      <a class="menu__item" href="https://scholar.google.com/citations?user=pGbCGogAAAAJ">Publications</a>
      <a class="menu__item" href="https://github.com/bikostet">GitHub</a>
      <a class="menu__item" href="https://www.linkedin.com/in/bilal-kostet-8b88691b6/">LinkedIn</a>
    </nav>
  </section>
</div>


<style>
  .stage {
    min-height: 100%;
    display: grid;
    place-items: center;
  }

  .card {
    width: min(780px, calc(100% - 10rem));
    aspect-ratio: 3.5 / 2;
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
    text-shadow:
    2px 2px 0 rgba(255,255,255,0.15),
   -0px -0px 3px rgba(0,0,0,0.35);
  }

  .card__top {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
  }

  .name {
    font-size: clamp(1.25rem, 7.0cqi, 2.75rem);
    font-weight: 400;
    background: linear-gradient(
    to bottom,
    #000000 0%,
    #524c40 22%,
    #68582b 45%,
    #664f16 62%,
    #000000 100%
    );
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
    text-shadow:
    2px 2px 0 rgba(255,255,255,0.15),
   -0px -0px 3px rgba(0,0,0,0.35);
  }

  .email,
  .employer {
    flex: 1;
    min-width: 0;
  }

  .email {
    text-align: left;
    font-size: clamp(0.5rem, 3.3cqi, 1.6rem);
  }

  .employer {
    text-align: right;
    font-family: "University Old Style", serif;
    font-size: clamp(0.8rem, 4.5cqi, 1.8rem);
  }
  .role {
    margin-top: 0.2rem;
    font-size: clamp(0.8rem, 4.5cqi, 1.8rem);
    font-weight: 300;
  }
  .role2 {
    margin-top: -0.4rem;
    font-size: clamp(0.7rem, 3cqi, 1.5rem);
    font-weight: 300;
  }

  .card__details {
    display: grid;
    align-content: center;
    gap: 0.35rem;
    text-align: center;
    letter-spacing: 0.02em;
  }

  .menu {
    display: flex;
    width: 100%;
    align-items: baseline;
    justify-content: center;
    gap: clamp(0.2rem, 2.1cqi, 4rem);
    padding-top: clamp(0.4rem, 1.6cqi, 0.8rem);
    font-size: clamp(0.5rem, 3.8cqi, 2rem);
    flex-wrap: wrap;
  }
  
  .menu__item {
    color: var(--ink);
    text-decoration: none;
    padding: 0.4rem 0.2rem;
    border-bottom: 1px solid transparent;
  }

  .menu__item:hover {
    border-bottom-color: rgba(0,0,0,0.35);
  }

  .menu__item:focus-visible {
    outline: 2px solid rgba(0,0,0,0.35);
    outline-offset: 3px;
    border-radius: 4px;
  }
</style>