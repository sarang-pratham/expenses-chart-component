<script>
  import Logo from './assets/logo.svg'
  // import Counter from './lib/Counter.svelte'
</script>

<main>
  <div class="sec1">
    <div class="balance">
      <p>My balance</p>
      <p>$921.48</p>
    </div>
    <img src={Logo} alt="logo" id="logo">
  </div>

  <div class="sec2">
    <h3>Spending - Last 7 days</h3>
    <div id="bar-chart"></div>
    <hr>
    <div class="total">
      <div class="total-1">
        <small>Total this month</small>
        <p>$478.33</p>
      </div>
      <div class="total-2">
        <p>+2.4%</p>
        <small>from last month</small>
      </div>
    </div>
  </div>
</main>

<style>
  
</style>
