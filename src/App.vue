<template>
  <div id="app" class="container">
    <img class="my-5" alt="Rashid logo" src="./assets/rashid.png">

    <div class="row">
      <div class="col-md-9">
        <div class="card bg-dark light">
          <div class="card-body">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vitae modi nihil quisquam quasi consequatur, autem repellat quaerat officia dolorem id? Sequi, laboriosam iusto non magnam expedita vitae. Vitae, quam eum fugiat numquam accusamus nisi odit quo. Cumque assumenda, qui eligendi pariatur rem adipisci inventore voluptates, quo beatae obcaecati architecto officia eius, nisi a. Ratione fugit aut placeat veniam dolores odio ut iusto perspiciatis praesentium fuga, mollitia enim corporis facere nesciunt unde reprehenderit repellat amet, voluptate sequi repellendus, quidem recusandae. Minima, culpa. Ullam aliquam fugit perferendis ea doloribus, nihil deserunt dolores delectus quas corporis sed eligendi ipsam aperiam quam dolorem molestias?
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

export default {
  name: 'app',
  components: {
    HelloWorld,
    PartyLevel
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
