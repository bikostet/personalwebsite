<svelte:head>
  <title>Bilal Kostet</title>
  <meta name="description" content="Bilal Kostet's homepage" />
</svelte:head>

<div class="stage">
  <section class="card">

<div class="card__details">
      <h1 class="title">About ❀</h1>

      <div class="about">
        <p>
          I’m a postdoctoral researcher interested in combining mechanistic models, inspired by physical processes, with statistical data analysis methods. These models can be used to investigate how heterogeneous spatial structures (such as population density, contact patterns) modify the propagation of an epidemic, how environmental forcing (such as temperature or seasonality) alters transmission rates, and under which conditions the system undergoes qualitative changes in behaviour, for instance through the emergence of waves or regime shifts between extinction and endemic persistence.
        </p>

        <p>
        Beyond prediction, they provide a framework to interpret data, identify key drivers, and assess the potential impact of interventions in order to inform decision-makers.
        </p> 

      </div>
    </div>

    <nav class="menu">
      <a class="menu__item" href="/">Home</a>
      <a class="menu__item" href="/about">About</a>
      <a class="menu__item" href="/cv_Kostet.pdf" target="_blank">CV</a>
      <a class="menu__item" href="https://scholar.google.com/citations?user=pGbCGogAAAAJ">Publications</a>
      <a class="menu__item" href="https://github.com/bikostet">GitHub</a>
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
    grid-template-rows: 1fr auto;
    gap: clamp(0.6rem, 2cqi, 1rem);
    container-type: inline-size;

    background-image: url("/textures/paper.png");
    background-size: cover;
    background-position: center;
    text-shadow:
    2px 2px 0 rgba(255,255,255,0.15),
   -0px -0px 3px rgba(0,0,0,0.35);
  }

  
  .about {
    font-size: clamp(0.95rem, 2.9cqi, 1.25rem);
    line-height: 1.55;
    font-family: "Garamond", "EB Garamond", serif;
  }

  .about p {
    margin: 0;
  }

  .about p + p {
    margin-top: 0.9em;
  }

  .menu {
    display: flex;
    width: 100%;
    align-items: baseline;
    justify-content: center;
    gap: clamp(0.8rem, 5cqi, 4rem);
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