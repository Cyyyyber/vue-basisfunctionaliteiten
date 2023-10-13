<script>

export default{
  data(){
    return{
      naam: "Tessa",
      achternaam: "Brzyk",
      url: "https//:google.com",
      number: 0,
    }
  },
  methods:{
    showFullName(){
      return "Tessa Brzyk";
    },
    showName(){
      this.naam = this.naam + "Brzyk";
      return this.naam;
    },
    addNumber(nr){ //verwacht dat getal wordt meeggegeven
      this.number = this.number + nr;  //getal wordt hiermee opgeteld ()
    }
  },
}
</script>

<template>
  
  <h1>Welkom in het project</h1>
  <p>{{ naam }}</p>
  <h2>{{ showFullName() }}</h2>
  <p>{{ showName }}</p>
  <a :href="url">google</a><br>


  <p>{{ number }}</p>
  <button @:click="addNumber(0)">Click</button>  <!-- addNumber(11): on click 11 + 11 ....-->





</template>

<style>
</style>
