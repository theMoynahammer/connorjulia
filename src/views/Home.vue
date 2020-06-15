<template>
  <div class="home">
    <img alt="Vue logo" style="width: 150px;" src="../assets/cj.png">
    <h4>❤️ May 15, 2021 ❤️</h4>
    <strong><div id="countdown"></div></strong>
    <HelloWorld msg=""/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';

// Set the date we're counting down to
const countDownDate = new Date('May 15, 2021 18:00:00').getTime();

// Update the count down every 1 second
const countdownFunction = () => {
  // Get today's date and time
  const now = new Date().getTime();

  // Find the distance between now and the count down date
  const distance = countDownDate - now;

  // Time calculations for days, hours, minutes and seconds
  const days = Math.floor(distance / (1000 * 60 * 60 * 24));
  const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  const seconds = Math.floor((distance % (1000 * 60)) / 1000);

  // Display the result in the element with id="demo"
  document.getElementById('countdown').innerHTML = `${days}d ${hours}h 
  ${minutes}m ${seconds}s `;

  // If the count down is finished, write some text
  // if (distance < 0) {
  //   clearInterval(x);
  //   document.getElementById("demo").innerHTML = 'EXPIRED';
  // }
};
// const x = setInterval(countdownFunction, 1000);
setInterval(countdownFunction, 1000);

export default {
  name: 'Home',
  components: {
    HelloWorld,
  },
};
</script>
