<script>
  let getData = async () => {
    let response = await fetch('../../data.json')
    return await response.json()
  }

  let data = getData()

</script>

{#await data then value}
<div id="bar-chart">
  <div class="bar">
    <div class="t" style="height: {value[0].amount * 2}px;"></div>
    <span>mon</span>
  </div>
  <div class="bar">
    <div class="t" style="height: {value[1].amount * 2}px;"></div>
    <span>tue</span>
  </div>
  <div class="bar">
    <div class="t" style="height: {value[2].amount * 2}px; background-color: var(--cyan);"></div>
    <span>wed</span>
  </div>
  <div class="bar">
    <div class="t" style="height: {value[3].amount * 2}px;"></div>
    <span>thu</span>
  </div>
  <div class="bar">
    <div class="t" style="height: {value[4].amount * 2}px;"></div>
    <span>fri</span>
  </div>
  <div class="bar">
    <div class="t" style="height: {value[5].amount * 2}px;"></div>
    <span>sat</span>
  </div>
  <div class="bar">
    <div class="t" style="height: {value[6].amount * 2}px;"></div>
    <span>sun</span>
  </div>
</div>
{/await}

<style>
  #bar-chart{
  display: flex;
  justify-content: space-between;
  height: 12rem;
}

.bar{
  width: 30px;

  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: auto;
}
.t{
  width: 100%;
  background-color: var(--soft-red);
  border-radius: 0.2rem;
}
.bar span{
  text-align: center;
  font-size: 14px;
  margin: 0.5rem 0 1rem 0;
  color: var(--medium-brown);
  font-weight: 400;
}
</style>