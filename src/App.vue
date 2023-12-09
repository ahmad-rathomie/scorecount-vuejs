<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <div id="MyApp">
    <p>My Score is {{count}}</p>
    <button v-on:click="ScoreIncre(1)">Increase my Score</button>
    <button v-on:click="ScoreDecre(-1)">Decrease my Score</button>
  </div>

</template>

<script>


export default {
 
  name: '#MyApp',
  data() {
    return{
    count: 10,
    }
  },
  methods: {
    ScoreIncre: function() {
      this.count++;
    },
    ScoreDecre: function() {
      this.count--;
    }
  }
};


</script>

<style>
#MyApp{
  background-color: aqua;
  margin: 50px;
  padding-top: 50px;
  padding-bottom: 50px;
  text-align: center;
  font-size: 80px;
  border: solid black 5px;
}
button{
  margin: 5px;
  padding: 10px 10px;
  cursor: pointer;
  font-size: 20px;
}
</style>
