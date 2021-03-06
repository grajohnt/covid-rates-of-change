<div class="container" style="width: 100%">

<div class="row">
  <div class="column">

<p>Demo: <a href="https://stml.github.io/covid-rates-of-change/">https://stml.github.io/covid-rates-of-change/</a></p>

<p>Data is from the <a href="https://www.ecdc.europa.eu/en/publications-data/download-todays-data-geographic-distribution-covid-19-cases-worldwide">European Centre for Disease Prevention and Control</a> /  <a href="https://github.com/stml/covid-rates-of-change">Code at GitHub</a> / To update, download ECDPC .csv and rename <code>data/covid.csv</code>.</p>

  </div>
</div>

<script src="scripts/jquery.js" type="text/javascript"></script>
<script src="scripts/d3.min.js"></script>
<script src="scripts/d3-scale-chromatic.v1.min.js"></script>
<script src="scripts/d3-time-format.v2.min.js"></script>
<script src="scripts/graphs.js?=<?=rand()?>" type="text/javascript"></script>
<link rel="stylesheet" type="text/css" href="css/normalize.css" />
<link rel="stylesheet" type="text/css" href="css/skeleton.css" />
<link rel="stylesheet" type="text/css" href="css/styles.css?=<?=rand()?>" />

  <div class="row">
    <div class="column">
    <p>Cumulative number of cases, by number of days since
      <select id="first_limit">
        <option value="1">1st</option>
        <option value="10">10th</option>
        <option value="100" selected>100th</option>
        <option value="1000">1000th</option>
      </select> case.</p>
    <p>Data last updated <span id="latest_update">..</span>.</p>
  </div>
  </div>

  <div class="row">
    <div class="column">
      <div id="graph" class="u-full-width">
    </div>
  </div>

  <div class="row">
    <div class="column">
      <button id="toggle-axes">Toggle Axes</button>
      <button id="toggle-labels">Toggle Labels</button>
      <button id="toggle-colours">Toggle Colours</button>
    </div>
  </div>

  <div class="row">
    <div class="column">
      <button id="select-all">Select All</button>
      <button id="deselect-all">Deselect All</button>
      <button id="personal">Personal Interest</button>
    </div>
  </div>

  <div class="row">
    <div class="column">
      <h5>Countries (Total Cases / Total Deaths)</h5>
      <ul id="selectors"></ul>
    </div>
  </div>

</div>  
