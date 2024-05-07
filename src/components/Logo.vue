<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
  <div class="greetings">
    <span class="deans-racket">
      dean's racket
    </span>
    <div class="center-cirles"><div class="circles"></div></div>
  </div>
</template>

<style scoped>

.greetings {

  background-color: aliceblue;

  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: center;
  align-items: center;
}

/* .dean {
background-image: linear-gradient(45deg, #f2f0f5 25%, #05010a 25%, #05010a 50%, #f2f0f5 50%, #f2f0f5 75%, #05010a 75%, #05010a 100%);
background-size: 28.28px 28.28px;
} */

/* @media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
} */

/* h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
} */

/* .birthday {
  font-size: 2rem;
  color:#358cd9;
  text-align: center;
} */

.deans-racket {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: center;
  align-content: stretch;
  align-items: center;

  z-index: 30;
  margin-bottom: 10px;
  padding: 25px;
  font-size: 5rem;
  color:#358cd9;
  color: black;
}

.center-cirles {
  position: absolute;
  z-index: 20;

  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: center;
  align-content: stretch;
  align-items: center;
}
.circles,
.circles:before,
.circles:after {
  border-radius: 50%;
  width: 200px;
  height: 200px;
  content: '';
  display: block;
}

.circles {
  background-color: #358cd9;
  position: relative;
  top: 20px;
  left: 10px;
  bottom: 50px;
  mix-blend-mode: lighten;
}

.circles:before,
.circles:after {
  position: absolute;
}

.circles:before {
  left: -80px;
  top: 110px;
  background-color: #ed740b;
  mix-blend-mode: lighten;
}

.circles:after {
  left: 90px;
  bottom: 125px;
  background-color: #22e978;
  mix-blend-mode: overlay;
}
</style>
