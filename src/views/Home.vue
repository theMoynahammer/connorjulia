<template>
  <v-container fill-height>
    <!-- <h2>We're Getting Married!</h2> -->
    <!-- <v-row align="center" justify="center">
      <v-col align="center">
        <v-img max-width="500" src="/assets/dopebeachpic.jpg"></v-img>
      </v-col>
    </v-row> -->
    <v-row>
      <!-- <v-col sm="6"> -->
      <v-col>
        <!-- <section>
<h2>WWF History</h2>
<p>This is a testinthing
  fake fake
</p>
</section> -->
        <v-card class="card-style" shaped elevation="10">
          <!-- <v-card-title class="justify-center">TESTING THIS</v-card-title> -->
          <v-container>
            <v-row>
              <!-- <div class="d-flex flex-no-wrap justify-space-between"> -->
              <v-col sm="8">
                <v-card-text>
                  <h3>WE'RE GETTING MARRIED!</h3>
                  A year ago when the pandemic started, we thought our wedding
                  date would be safe as "everything would be fine over a year
                  from now". We were so, so wrong. We have decided not have our
                  full reception this year. Instead, we will be having a small
                  ceremony and dinner with close family and the wedding party on
                  May 15th, 2021, with the full reception to be the following
                  year, May 7th, 2022. We're hoping you all can make our
                  ceremony, and we'd love to celebrate with the most important
                  people in our lives.
                </v-card-text>
              </v-col>
              <v-col sm="4">
                <div class="d-flex justify-center">
                  <v-avatar class="ma-3" size="250" tile>
                    <v-img src="/assets/dopebeachpic.jpg"></v-img>
                  </v-avatar>
                </div>
              </v-col>
              <!-- <div>
              <v-card-title v-text="YOOOOOO"></v-card-title>

              <v-card-subtitle v-text="ARTIST"></v-card-subtitle>

              <v-card-actions>
                <v-btn
                  class="ml-2 mt-3"
                  fab
                  icon
                  height="40px"
                  right
                  width="40px"
                >
                  <v-icon>mdi-play</v-icon>
                </v-btn>

                <v-btn class="ml-2 mt-5" outlined rounded small>
                  START RADIO
                </v-btn>
              </v-card-actions>
            </div> -->
              <!-- </div> -->
            </v-row>
          </v-container>
        </v-card>
        <!-- <v-parallax height="400" src="/assets/dopebeachpic.jpg"></v-parallax> -->
      </v-col>
    </v-row>
    <v-row>
      <v-col><h2 class="text-center">Ceremony Details</h2></v-col>
    </v-row>
    <v-row>
      <v-col sm="6" lg="12">
        <!-- <v-divider></v-divider> -->
        <v-card>
          <!-- <v-card-title class="justify-center">
            When
          </v-card-title> -->
          <!-- <v-card-subtitle>connor.moynahan@gmail.com</v-card-subtitle> -->
          <v-card-title class="justify-center"> When? </v-card-title>
          <v-card-subtitle class="text-center"
            ><b>May 15, 2021</b></v-card-subtitle
          >
          <v-card-text>
            <v-timeline align-top dense>
              <v-timeline-item color="#4682B4" small>
                <v-row class="pt-1">
                  <v-col cols="3">
                    <strong>5pm</strong>
                  </v-col>
                  <v-col>
                    <strong>Guests arrive</strong>
                    <!-- <div class="caption">
                Mobile App
              </div> -->
                  </v-col>
                </v-row>
              </v-timeline-item>
              <v-timeline-item color="#4682B4" small>
                <v-row class="pt-1">
                  <v-col cols="3">
                    <strong>5:30pm</strong>
                  </v-col>
                  <v-col>
                    <strong>Ceremony Starts</strong>
                  </v-col>
                </v-row>
              </v-timeline-item>

              <v-timeline-item color="#4682B4" small>
                <v-row class="pt-1">
                  <v-col cols="3">
                    <strong>~6pm</strong>
                  </v-col>
                  <v-col>
                    <strong>Eat Dinner</strong>
                    <!-- <div class="caption">
                Web App
              </div> -->
                  </v-col>
                </v-row>
              </v-timeline-item>
              <v-timeline-item color="#4682B4" small>
                <v-row class="pt-1">
                  <v-col cols="3">
                    <strong>~10pm</strong>
                  </v-col>
                  <v-col>
                    <strong>Guests leave</strong>
                    <!-- <div class="caption">
                Web App
              </div> -->
                  </v-col>
                </v-row>
              </v-timeline-item>
            </v-timeline>
          </v-card-text>
        </v-card>
      </v-col>
      </v-row>
    <v-row>
      <v-col sm="6" lg="12">
        <!-- <v-divider></v-divider> -->
        <v-card>
          <!-- <v-card-title class="justify-center">
            When
          </v-card-title> -->
          <!-- <v-card-subtitle>connor.moynahan@gmail.com</v-card-subtitle> -->
          <v-card-title class="justify-center"> Where? </v-card-title>
          <v-card-subtitle class="text-center"
            >(click address to open in Google maps)</v-card-subtitle
          >
          <v-card-text class="text-center"
            ><h6><b>Virginia Powerboat Association</b></h6>
            <a
              href="https://www.google.com/maps?q=4051%20E%20Old%20Gun%20Rd%20Midlothian,%20VA%2023113"
              target="_blank"
              rel="noopener noreferrer"
            ><h6>
              4051 E Old Gun Rd<br />
              Midlothian, VA 23113</h6></a
            >
            <br /><br /><br /><br /><br /><br /><br /><br />
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
  <!-- <div class="home">
    <img alt="Vue logo" style="width: 150px;" src="../assets/cj.png">
    <h4>❤️ May 15, 2021 ❤️</h4>
    <strong><div id="countdown"></div></strong>
    <HelloWorld msg=""/>
  </div> -->
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue';

// Set the date we're counting down to
// const countDownDate = new Date("May 15, 2021 18:00:00").getTime();

// // Update the count down every 1 second
// const countdownFunction = () => {
//   // Get today's date and time
//   const now = new Date().getTime();

//   // Find the distance between now and the count down date
//   const distance = countDownDate - now;

//   // Time calculations for days, hours, minutes and seconds
//   const days = Math.floor(distance / (1000 * 60 * 60 * 24));
//   const hours = Math.floor(
//     (distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60)
//   );
//   const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
//   const seconds = Math.floor((distance % (1000 * 60)) / 1000);

//   // Display the result in the element with id="demo"
//   // document.getElementById("countdown").innerHTML = `${days}d ${hours}h
//   // ${minutes}m ${seconds}s `;

//   // If the count down is finished, write some text
//   // if (distance < 0) {
//   //   clearInterval(x);
//   //   document.getElementById("demo").innerHTML = 'EXPIRED';
//   // }
// };
// // const x = setInterval(countdownFunction, 1000);
// setInterval(countdownFunction, 1000);

export default {
  name: 'Home',
  components: {
    // HelloWorld,
  },
};
</script>

<style scoped>
.helper-text {
  color: #007bff;
}
html,
body,
h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Roboto", sans-serif;
}

.left-info-override {
  padding-top: 10px;
}

.text-light-blue {
  color: #4682b4;
}

.card-style {
  margin-bottom: 10px;
}

.icon-style {
  margin-right: 10px;
}

.otherFlexBox {
  height: 100%;
  padding: 0;
  margin: 0;
  display: -webkit-box;
  display: -moz-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}
</style>
