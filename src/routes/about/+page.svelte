<svelte:head>
  <title>About Bilal Kostet</title>
  <meta name="description" content="Bilal Kostet's homepage" />
</svelte:head>



<div class="card__details">
  <div class="abouttitle">About <span class="mirror">❧</span></div>

  <div class="about">
    <p>
      I’m a postdoctoral researcher interested in combining mechanistic models, inspired by physical processes, with statistical data analysis methods. These models can be used to investigate how heterogeneous spatial structures (population density, contact patterns) modify the propagation of an epidemic, how environmental factors alters transmission rates, and under which conditions the system undergoes qualitative changes in behaviour, such as emergence of waves or sudden regime shifts between extinction and endemic persistence.<br>
    Beyond prediction, they provide a framework to interpret data, identify key drivers, and assess the potential impact of interventions in order to inform decision-makers.
    </p> 
  </div>
</div>

<div class="seal">❀</div> 

<style>
.abouttitle {
    font-size: clamp(1.25rem, 7.0cqi, 2.75rem);
    display: block;
    margin-top: 0.67em;
    margin-bottom: 0.67em;
    margin-left: 0;
    margin-right: 0;
    font-weight: bold;
    filter:
    drop-shadow(0px 1.5px 0px rgba(255, 255, 255, 0.8))
    drop-shadow(0px -0.5px 0px rgba(0, 0, 0, 0.25));
  }

  .about {
    font-size: clamp(0.8rem, 2.4cqi, 1.05rem);
    line-height: 1.6;
    font-family: "Garamond", "EB Garamond", serif;
    filter:
    drop-shadow(0px 1px 0px rgba(255, 255, 255, 0.75))
    drop-shadow(0px -0.5px 0px rgba(0, 0, 0, 0.2));
  }

  .about p {
    margin: 0;
  }

  .seal {
    margin-top:0.3em;
    text-align: center;
    font-size: clamp(0.5rem, 3.8cqi, 2rem);
  }

  .mirror {
  display: inline-block;
  transform: rotate(90deg);
  font-size: clamp(1.2rem, 3.3cqi, 1.6rem);
}

.card__details {
  height: 100%;
  display: grid;
  align-content: start;
  overflow: auto;
}
</style>