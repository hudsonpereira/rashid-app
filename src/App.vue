<template>
  <div id="app" class="container">
    <img class="my-5" alt="Rashid logo" src="./assets/rashid.png">

    <div class="row">
      <div class="col-md-9">
        <div class="card bg-dark light">
          <div class="card-header">Party Maker</div>
          <div class="card-body">
            <PartyMaker />
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card bg-dark light">
          <div class="card-header">Party Level Calculator</div>
          <div class="card-body">

            <PartyLevel />
          </div>
        </div>

        <div class="card bg-dark light mt-2">
          <!-- <div class="card-header">Party Level Calculator</div> -->
          <div class="card-body">

            <RashidLocation />
          </div>
        </div>
      </div>
    </div>


    <footer class="my-5">
      <p>Created with LOVE by Sonata Moonlight @ Gentebra</p>
    </footer>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import PartyLevel from './components/PartyLevel/PartyLevel.vue'
import PartyMaker from './components/PartyMaker/PartyMaker.vue'
import RashidLocation from './components/RashidLocation.vue';

export default {
  name: 'app',
  components: {
    HelloWorld,
    PartyLevel,
    RashidLocation,
    PartyMaker
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
}

body {
  background: url('./assets/background.jpg') no-repeat;
  background-size: cover;
}
</style>
