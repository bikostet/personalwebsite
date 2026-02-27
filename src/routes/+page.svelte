<svelte:head>
  <title>Bilal Kostet</title>
  <meta name="description" content="Bilal Kostet's homepage" />
</svelte:head>


<header class="card__top">
  <div class="email">bikostet at berkeley dot edu</div>
  <div class="employer">UC Berkeley</div>
</header>

<div class="card__details">
    <div class="name">Bilal Kostet</div>
    <div class="role">Postdoctoral researcher</div>
    <div class="role2">in Demography</div>
</div>

<style>
  .card__top {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
  }

  .name {
    font-size: clamp(1.4rem, 6.5cqi, 2.6rem);
    font-weight: 400;
    background: linear-gradient(
    to bottom,
    #2a1f00 0%,
    #6b4f1a 30%,
    #8a6520 50%,
    #5c4015 70%,
    #2a1f00 100%
    );
    filter:
    drop-shadow(0px 1.5px 0px rgba(255, 255, 255, 0.8))
    drop-shadow(0px -0.5px 0px rgba(0, 0, 0, 0.25));
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
  }

  .email,
  .employer {
    flex: 1;
    min-width: 0;
  }

  .email {
    text-align: left;
    font-size: clamp(0.6rem, 2.8cqi, 1rem);
  }

  .employer {
    text-align: right;
    font-family: "University Old Style", serif;
    font-size: clamp(0.8rem, 4.5cqi, 1.8rem);
  }
  .role {
    margin-top: 0.2rem;
    font-size: clamp(0.75rem, 3.8cqi, 1.35rem);
  }
  .role2 {
    margin-top: -0.4rem;
    font-size: clamp(0.65rem, 2.8cqi, 1.1rem);
  }

  .role, .role2 {
    font-weight: 300;
    background: linear-gradient(
    to bottom,
    #2e2210 0%,
    #926b23 50%,
    #2e2210 100%
  );
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
}

  .card__details {
    display: grid;
    align-content: center;
    gap: 0.35rem;
    text-align: center;
    letter-spacing: 0.02em;
  }

  .role, .role2, .email, .employer {
  filter:
    drop-shadow(0px 1px 0px rgba(255, 255, 255, 0.75))
    drop-shadow(0px -0.5px 0px rgba(0, 0, 0, 0.2));
}
</style>