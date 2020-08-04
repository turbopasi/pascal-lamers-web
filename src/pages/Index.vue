<template>
  <Layout>

    <section class="start-section">
      <div class="container-1">

        <div class="container-2">
          <h1>
            Komm<br>zum<br>Punkt.
          </h1>
          <h2>
            SAG SCHON WAS DU BRAUCHST
          </h2>
          <button>
            MACHS
          </button>
        </div>

        <div class="container-3">
          <g-image class="image" src="~/assets/salzburg_land.jpg" />
        </div>

      </div>
    </section>

    <section class="section-1">
      
    </section>

  </Layout>
</template>

<script>
export default {
  metaInfo: {

  }
}
</script>

<style scoped>

  .start-section {
    height : 100vh;
    width : 80%;
    margin : 0 auto;
    display: flex;
    align-items: center;
  }

  .container-1 {
    height : 400px;
    flex: 1;
    display : flex;
  }

  .container-2 {
    width : 450px;
    display : flex;
    flex-direction: column;
  }

  .container-2 h1 {
    font-size:90px;
    font-weight: 500;
    letter-spacing: 0;
    line-height: 0.9em;
    text-transform: uppercase;
    flex:1;
  }

  .container-2 h2 {
    font-size:20px;
    font-weight: 500;
    color: orangered;
    flex:0.5;
  }

  .container-2 button {
    border : none;
    background : teal;
    color : white;
    font-family: 'Rubik';
    width: 200px;
    padding : 20px;
    letter-spacing: 2px;
    font-size: 20px;
    border-radius: 4px;
    font-weight: 100;
  }

  .container-3 {
    flex: 1;
    overflow:hidden;
    border-radius:10px;
  }

  .container-3 .image {
    object-position: 50% 50%;
    object-fit:cover;
    width:100%;
    height:100%;
  }

  .section-1 {
    height : 100vh;
    background : teal;
    width : 80%;
    margin : 0 auto;
  }

</style>
