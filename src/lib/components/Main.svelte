<script lang="ts">
  import { myWork } from "../myWork/myWork.js";
</script>

<div class="content-container">
  <h3 id="myWork">My work</h3>
  <div class="flex-container"> 
    {#each myWork as card}
      <div class="card">
      <div class="img-container" style="background-image: url('{card.img}')">
      </div>
      <div class="text-container">
        <h4>{card.title}</h4>
        <p>{card.descrition}</p>
      </div>
      <div class="link-container">
        <a href='{card.github}' class="button">Github</a>
        <a href='{card.page}' class="button" >Visit</a>
      </div>
    </div>
    {/each}
  </div>
</div>

<style lang="scss">
  .content-container{
    max-width: 1200px;
    margin: auto;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  h3 {
    text-align: center;
  }

  .flex-container {
    display: flex; 
    flex-wrap: wrap;
    max-width: 1000px;
    justify-content: center;
    margin: auto;
    gap: var(--spacing-m);
  }

  .img-container {
    height: 300px;
    width: 100%;
    background-size: cover;
    background-repeat: no-repeat;
    margin: 0;
  }

  .card {
    border: solid 0.5px var(--primary);
    width: 300px;
    height: 550px;
    display: flex;
    flex: 1fr 1fr auto;
    flex-direction: column;
    justify-content:space-between;
    box-shadow: 6px -2px 20px -7px rgba(1,21,19,0.50);
    transition: all ease 0.5s;
  }

  .card:hover {
    box-shadow: 6px -2px 20px -7px rgba(1,21,19,1);
  }

  @media only screen and (max-width: 600px){
    .card{
      margin: var(--spacing-s);
    }
  }
</style>