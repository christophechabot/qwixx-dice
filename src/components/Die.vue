<template>
  <span :class="color">
    <svg
      v-if="value === 1"
      class="die"
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 512 512">
      <path d="M0 0h512v512H0z" :fill="primaryColor" fill-opacity="1">
      </path>
      <g class="" transform="translate(0,0)" style="touch-action: none;">
        <path d="M302.87 255.5a47.37 47.37 0 1 1-47.37-47.37 47.37 47.37 0 0 1 47.37 47.37zM484.5 428.02a56.48 56.48 0 0 1-56.48 56.48h-344a56.48 56.48 0 0 1-56.52-56.48v-344A56.48 56.48 0 0 1 83.98 27.5h344a56.48 56.48 0 0 1 56.52 56.48zm-20-344a36.48 36.48 0 0 0-36.48-36.52h-344A36.48 36.48 0 0 0 47.5 83.98v344a36.48 36.48 0 0 0 36.48 36.52h344a36.48 36.48 0 0 0 36.52-36.48z" :fill="secondaryColor" fill-opacity="1">
        </path>
      </g>
    </svg>

    <svg
      v-if="value === 2"
      class="die"
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 512 512">
      <path d="M0 0h512v512H0z" :fill="primaryColor" fill-opacity="1">
      </path>
      <g class="" transform="translate(0,0)" style="touch-action: none;">
        <path d="M383 81.68A47.37 47.37 0 1 1 335.58 129 47.37 47.37 0 0 1 383 81.68zM81.67 383A47.37 47.37 0 1 0 129 335.59 47.37 47.37 0 0 0 81.67 383zM428 47.57H84A36.48 36.48 0 0 0 47.57 84v344A36.48 36.48 0 0 0 84 464.43h344A36.48 36.48 0 0 0 464.43 428V84A36.48 36.48 0 0 0 428 47.57m0-20A56.54 56.54 0 0 1 484.43 84v344A56.54 56.54 0 0 1 428 484.43H84A56.54 56.54 0 0 1 27.57 428V84A56.54 56.54 0 0 1 84 27.57z" :fill="secondaryColor" fill-opacity="1">
        </path>
      </g>
    </svg>

    <svg
      v-if="value === 3"
      class="die"
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 512 512">
      <path d="M0 0h512v512H0z" :fill="primaryColor" fill-opacity="1">
      </path>
      <g class="" transform="translate(0,0)" style="touch-action: none;">
        <path d="M302.87 255.5a47.37 47.37 0 1 1-47.37-47.37 47.37 47.37 0 0 1 47.37 47.37zM382.5 81.18a47.37 47.37 0 1 0 47.32 47.32 47.37 47.37 0 0 0-47.32-47.32zm-254 253.91a47.37 47.37 0 1 0 47.41 47.41 47.37 47.37 0 0 0-47.41-47.41zm356 92.94a56.48 56.48 0 0 1-56.48 56.47h-344a56.48 56.48 0 0 1-56.52-56.48v-344A56.48 56.48 0 0 1 83.98 27.5h344a56.48 56.48 0 0 1 56.52 56.48zm-20-344a36.48 36.48 0 0 0-36.48-36.53h-344A36.48 36.48 0 0 0 47.5 83.98v344a36.48 36.48 0 0 0 36.48 36.52h344a36.48 36.48 0 0 0 36.52-36.48z" :fill="secondaryColor" fill-opacity="1">
        </path>
      </g>
    </svg>

    <svg
      v-if="value === 4"
      class="die"
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 512 512">
      <path d="M0 0h512v512H0z" :fill="primaryColor" fill-opacity="1">
      </path>
      <g class="" transform="translate(0,0)" style="touch-action: none;">
        <path d="M175.91 128.5a47.37 47.37 0 1 1-47.41-47.32 47.37 47.37 0 0 1 47.41 47.32zM382.5 81.18a47.37 47.37 0 1 0 47.32 47.32 47.37 47.37 0 0 0-47.32-47.32zm-254 253.91a47.37 47.37 0 1 0 47.41 47.41 47.37 47.37 0 0 0-47.41-47.41zm253.91 0a47.37 47.37 0 1 0 47.41 47.41 47.37 47.37 0 0 0-47.32-47.41zm102 92.93a56.48 56.48 0 0 1-56.39 56.48h-344a56.48 56.48 0 0 1-56.52-56.48v-344A56.48 56.48 0 0 1 83.98 27.5h344a56.48 56.48 0 0 1 56.52 56.48zm-20-344a36.48 36.48 0 0 0-36.39-36.52h-344A36.48 36.48 0 0 0 47.5 83.98v344a36.48 36.48 0 0 0 36.48 36.52h344a36.48 36.48 0 0 0 36.52-36.48z" :fill="secondaryColor" fill-opacity="1">
        </path>
      </g>
    </svg>

    <svg
      v-if="value === 5"
      class="die"
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 512 512">
      <path d="M0 0h512v512H0z" :fill="primaryColor" fill-opacity="1">
      </path>
      <g class="" transform="translate(0,0)" style="touch-action: none;">
        <path d="M302.87 255.5a47.37 47.37 0 1 1-47.37-47.37 47.37 47.37 0 0 1 47.37 47.37zM128.5 81.18a47.37 47.37 0 1 0 47.41 47.32 47.37 47.37 0 0 0-47.41-47.32zm253.91 0a47.37 47.37 0 1 0 47.41 47.32 47.37 47.37 0 0 0-47.32-47.32zM128.5 335.09a47.37 47.37 0 1 0 47.41 47.41 47.37 47.37 0 0 0-47.41-47.41zm253.91 0a47.37 47.37 0 1 0 47.41 47.41 47.37 47.37 0 0 0-47.32-47.41zm102 92.93a56.48 56.48 0 0 1-56.39 56.48h-344a56.48 56.48 0 0 1-56.52-56.48v-344A56.48 56.48 0 0 1 83.98 27.5h344a56.48 56.48 0 0 1 56.52 56.48zm-20-344a36.48 36.48 0 0 0-36.39-36.52h-344A36.48 36.48 0 0 0 47.5 83.98v344a36.48 36.48 0 0 0 36.48 36.52h344a36.48 36.48 0 0 0 36.52-36.48z" :fill="secondaryColor" fill-opacity="1">
        </path>
      </g>
    </svg>

    <svg
      v-if="value === 6"
      class="die"
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 512 512">
      <path d="M0 0h512v512H0z" :fill="primaryColor" fill-opacity="1">
      </path>
      <g class="" transform="translate(0,0)" style="touch-action: none;">
        <path d="M175.91 128.5a47.37 47.37 0 1 1-47.41-47.32 47.37 47.37 0 0 1 47.41 47.32zM382.5 81.18a47.37 47.37 0 1 0 47.32 47.32 47.37 47.37 0 0 0-47.32-47.32zm-254 126.95a47.37 47.37 0 1 0 47.41 47.37 47.37 47.37 0 0 0-47.41-47.37zm253.91 0a47.37 47.37 0 1 0 47.41 47.37 47.37 47.37 0 0 0-47.32-47.37zM128.5 335.09a47.37 47.37 0 1 0 47.41 47.41 47.37 47.37 0 0 0-47.41-47.41zm253.91 0a47.37 47.37 0 1 0 47.41 47.41 47.37 47.37 0 0 0-47.32-47.41zm102 92.93a56.48 56.48 0 0 1-56.39 56.48h-344a56.48 56.48 0 0 1-56.52-56.48v-344A56.48 56.48 0 0 1 83.98 27.5h344a56.48 56.48 0 0 1 56.52 56.48zm-20-344a36.48 36.48 0 0 0-36.39-36.52h-344A36.48 36.48 0 0 0 47.5 83.98v344a36.48 36.48 0 0 0 36.48 36.52h344a36.48 36.48 0 0 0 36.52-36.48z" :fill="secondaryColor" fill-opacity="1">
        </path>
      </g>
    </svg>
  </span>
</template>

<script>
export default {
  name: 'die',
  props: {
    value: Number,
    color: String
  },
  computed: {
    primaryColor() {
      switch(this.color) {
        case 'red':
          return '#d73f4c';
        case 'blue':
          return '#394a8b';
        case 'green':
          return '#419f5b';
        case 'yellow':
          return '#fee44a';
        case 'neutral':
        default:
          return '#444444';
      }
    },
    secondaryColor() {
      switch(this.color) {
        case 'red':
        case 'green':
        case 'yellow':
          return '#444444';
        case 'neutral':
        case 'blue':
        default:
          return 'white';
      }
    }
  }
}
</script>

<style>
  .die {
    display: inline-block;
    vertical-align: middle;
  }
</style>
