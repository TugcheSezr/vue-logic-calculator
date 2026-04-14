//Wat we gaan op de website zien
<template>

<div class="calculator">
  <div class="display"> {{current || 0}} </div>
  <div class="btn"> C </div>
  <div class="btn"> +/- </div>
  <div class="btn"> % </div>

  <div class="btn operator"> ÷ </div>

  <div class="btn"> 7 </div>
  <div class="btn"> 8 </div>
  <div class="btn"> 9 </div>
  <div class="btn operator"> x </div>

  <div class="btn"> 4 </div>
  <div class="btn"> 5 </div>
  <div class="btn"> 6 </div>
  <div class="btn operator"> - </div>

  <div class="btn"> 1 </div>
  <div class="btn"> 2 </div>
  <div class="btn"> 3 </div>
  <div class="btn operator"> + </div>
  
  <div class="btn zero"> 0 </div>
  <div class="btn"> . </div>
  <div class="btn operator"> = </div>

</div>
</template>

<script>
export default {
}
</script>

<style scoped>
.calculator {
  margin: 0 auto;
  margin-top: 15vh;
  font-size: 40px;
  display: grid;
  grid-template-columns: repeat(4, 100px);
  grid-auto-rows: minmax(80px, auto);
  justify-content: center;
}

.display {
  grid-column: 1 / 5;
  display: center;
  background: #ffffff;
  color: #000000;
  border: 1px solid black;
}
.zero {
  grid-column: 1 / 3;
}

.btn {
  background-color: #ffe4ec;
  border: 1px solid black;
}

.btn:hover {
  background-color: #f497b5;
}

.operator{
  background-color: #cb2e62;
  color: white;
  justify-content: center;
}

</style>