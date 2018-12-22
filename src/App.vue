<template>
  <div id="app">
    <div id="left-column">
      <div id="left-column-content">
        <Die :value="values[0]" color="neutral"/>
        <Die :value="values[2]" color="red"/>
        <Die :value="values[3]" color="blue"/>
        <Die :value="values[1]" color="neutral"/>
        <Die :value="values[4]" color="green"/>
        <Die :value="values[5]" color="yellow"/>
        <button @click="roll">Roll</button>
      </div>
    </div>
    <div id="right-column">
      <div id="right-column-content">
        <div class="right-column-row">
          <Die :value="values[0]" color="neutral"/>
          <span>+</span>
          <Die :value="values[1]" color="neutral"/>
          <span>=</span>
          <span class="total neutral">{{ values[0] + values[1] }}</span>
        </div>
        <div class="right-column-separator"></div>
        <div class="right-column-row">
          <span>
            <Die :value="values[0]" color="neutral"/>
            <span>+</span>
            <Die :value="values[2]" color="red"/>
            <span>=</span>
            <span class="total red">{{ values[0] + values[2] }}</span>
          </span>
          <span
            v-if="values[0] !== values[1]"
            class="right-column-row-right">
            <Die :value="values[1]" color="neutral"/>
            <span>+</span>
            <Die :value="values[2]" color="red"/>
            <span>=</span>
            <span class="total red">{{ values[1] + values[2] }}</span>
          </span>
        </div>
        <div class="right-column-row">
          <span>
            <Die :value="values[0]" color="neutral"/>
            <span>+</span>
            <Die :value="values[3]" color="blue"/>
            <span>=</span>
            <span class="total blue">{{ values[0] + values[3] }}</span>
          </span>
          <span
            v-if="values[0] !== values[1]"
            class="right-column-row-right">
            <Die :value="values[1]" color="neutral"/>
            <span>+</span>
            <Die :value="values[3]" color="blue"/>
            <span>=</span>
            <span class="total blue">{{ values[1] + values[3] }}</span>
          </span>
        </div>
        <div class="right-column-row">
          <span>
            <Die :value="values[0]" color="neutral"/>
            <span>+</span>
            <Die :value="values[4]" color="green"/>
            <span>=</span>
            <span class="total green">{{ values[0] + values[4] }}</span>
          </span>
          <span
            v-if="values[0] !== values[1]"
            class="right-column-row-right">
            <Die :value="values[1]" color="neutral"/>
            <span>+</span>
            <Die :value="values[4]" color="green"/>
            <span>=</span>
            <span class="total green">{{ values[1] + values[4] }}</span>
          </span>
        </div>
        <div class="right-column-row">
          <span>
            <Die :value="values[0]" color="neutral"/>
            <span>+</span>
            <Die :value="values[5]" color="yellow"/>
            <span>=</span>
            <span class="total yellow">{{ values[0] + values[5] }}</span>
          </span>
          <span
            v-if="values[0] !== values[1]"
            class="right-column-row-right">
            <Die :value="values[1]" color="neutral"/>
            <span>+</span>
            <Die :value="values[5]" color="yellow"/>
            <span>=</span>
            <span class="total yellow">{{ values[1] + values[5] }}</span>
          </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Die from './components/Die.vue'

export default {
  name: 'app',
  components: {
    Die
  },
  data: function() {
    return {
      values: [1, 2, 3, 4, 5, 6]
    };
  },
  methods: {
    roll() {
      this.values = [1, 2, 3, 4, 5, 6]
        .map(() => Math.floor(Math.random() * 6) + 1);
    }
  },
  mounted() {
    this.roll();
  }
}
</script>

<style>
body {
  margin: 0;
  padding: 0;
}
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
  }
  #left-column,
  #right-column {
    box-sizing: border-box;
    display: inline-block;
    vertical-align: middle;
    position: relative;
    width: 50%;
    height: 100vh;
    padding: 4px;
    text-align: center;
  }
  #left-column-content,
  #right-column-content {
    position: absolute;
    width: 100%;
    top: 50%;
    left: 0;
    transform: translate(0, -50%);
    text-align: center;
  }
  #left-column {
    border-right: 2px solid #2c3e50;
  }
  #left-column .die {
    box-sizing: border-box;
    width: 33%;
    height: auto;
    padding: 8px;
  }
  #left-column button {
    background: none;
    border: 2px solid #2c3e50;
    border-radius: 4px;
    padding: 9px 16px;
    margin-top: 32px;
    font-size: 24px;
  }
  #right-column .die {
    width: 5vw;
    height: auto;
    padding: 8px;
  }
  .right-column-row {
    padding: 0 8px;
  }
  .right-column-row-right { 
    padding-left: 2vw;
  }
  .right-column-row span {
    display: inline-block;
    vertical-align: middle;
    font-size: 3vw;
    font-weight: bold;
  }
  .right-column-row .total {
    padding: 0 8px;
    font-size: 4vw;
  }
  .right-column-row .total.red {
    color: #d73f4c;
  }
  .right-column-row .total.blue {
    color: #394a8b;
  }
  .right-column-row .total.green {
    color: #419f5b;
  }
  .right-column-row .total.yellow {
    color: #d8a352;
  }
  .right-column-separator {
    margin: 16px 32px;
    height: 1px;
    border-bottom: 2px solid #2c3e50;
  }
</style>
