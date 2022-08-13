<script>
  import Logo from './assets/logo.svg'
  import BarChart from './lib/BarChart.svelte'
</script>

<main>
  <div class="sec1">
    <p class="balance">My balance <br/> <span>$921.48</span></p>
    <img src={Logo} alt="logo" id="logo">
  </div>

  <div class="sec2">
    <h3>Spending - Last 7 days</h3>
    <BarChart/>
    <hr/>
    <div class="total">
      <p class="total-1">Total this month <br/> <span>$478.33</span></p>
      <p class="total-2"><span>+2.4%</span> <br/> from last month</p>
    </div>
  </div>
</main>

<style>
  
</style>
