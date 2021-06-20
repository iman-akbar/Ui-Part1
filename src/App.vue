<template>
  <v-app>
    <v-container class="full">
      <v-toolbar class="mt=0" color="white">
        <v-row>
          <v-col cols="2"></v-col>
          <v-col cols="auto">
            <v-avatar tile color="blue">
              <v-img
                src="./assets/bitmap.jpg"
                srcset="./assets/bitmap@2x.jpg 2x, ./assets/bitmap@3x.jpg 3x"
              ></v-img>
            </v-avatar>
          </v-col>
          <v-col>
            <p
              style="width: 82px;
  height: 14px;
  margin: 0 0 0 13px;
  font-family: WorkSans;
  font-size: 12px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: normal;
  color: #000000;"
            >
              Good Morning
              <span
                style="width: 47px;
  height: 19px;
  margin: 14px 35px 0 13px;
  font-family: WorkSans;
  font-size: 16px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: normal;
  color: #000000;"
              >Fellas</span>
            </p>

            <!-- <v-row></v-row> -->
          </v-col>
        </v-row>
      </v-toolbar>
      <!-- <v-card class="full"> -->
      <!-- src custom
       srcset="./assets/bg-1@2x.png 2x,
      ./assets/bg-1@3x.png 3x"-->

      <!-- <v-img
      class="white--text align-end"
      height="200px"
      src="./assets/bg-1.svg"
      ></v-img>-->
      <!-- <v-img
      class="BG_1"
      srcset="./assets/bg-1@2x.png 2x,
             ./assets/bg-1@3x.png 3x"
      src="./assets/bg-1.svg"
     
    >
     <v-card-title>Top 10 Australian beaches</v-card-title>
      </v-img>-->
      <v-img class="white--text BG_1" src="./assets/bg-1.svg">
        <!-- <v-card-title> -->
        <div>
          <p class="text">WEEKEND FROM HOME</p>
          <v-img
            src="./assets/bitmap.png"
            srcset="./assets/bitmap@2x.png 2x, ./assets/bitmap@3x.png 3x"
            class="Bitmap"
          >
           <v-container class="containerLets" dense border rounded-xl style="background: white">
     <p>Let`s go</p>
    </v-container>
          </v-img>
        </div>
        <!-- </v-card-title> -->
      </v-img>
      <v-img
        contain
        class="ml-auto"
        src="./assets/group-4.png"
        srcset="./assets/group-4@2x.png 2x, ./assets/group-4@3x.png 3x"
        style="width: 159px;
  height: 158px;
  margin: 0 0 184px 212px;"
      ></v-img>
      <v-row>
        <v-col></v-col>
        <v-col class="text-right">
          <p>
            <span style="
  font-weight: bold;
  
  color: #021bf9;">Deffinition</span>; a practice or exercise to test or improve one's fitness for
            athletic competition, ability, or performance to exhaust (something,
            such as a mine) by working to devise, arrange, or achieve by
            resolving difficulties. Merriam-Webster.com Dictionary.
          </p>
          <p
            style="
  height: 25px;  
  font-family: WorkSans;
  font-size: 21px;
  font-weight: 600;
  font-stretch: normal;
  font-style: italic;
  line-height: normal;
  letter-spacing: normal;  
  color: white;"
          >-weekend team</p>
        </v-col>
        <v-col>
          <!-- <v-img class="ml-auto" src="./assets/group-4.png"
     srcset="./assets/group-4@2x.png 2x,
             ./assets/group-4@3x.png 3x"
     
      :aspect-ratio="16/9"
      :width="width"
      
  >

          </v-img>-->
        </v-col>
      </v-row>

      <carousel-3d
        :controls-visible="true"
        :controls-prev-html="'&#10092; '"
        :controls-next-html="'&#10093;'"
        :controls-width="30"
        :controls-height="60"
        :clickable="false"
      >
        <slide v-for="(slide, i) in slider" :index="i" :key="i">
          <h1
            style=" width: 151px;
  height: 38px;
  margin: 0 56px 20px 0;
  font-family: WorkSans;
  font-size: 32px;
  font-weight: 900;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: normal;
  color: #000000;"
          >{{ slide.by }}</h1>
          <p>{{ slide.testimony }}</p>
        </slide>
      </carousel-3d>
      <p class="text-center POV" sty>POV</p>
      <!-- </v-card> -->

      <v-row justify="center">
        <p class="Lorem-ipsum-dolor-si">
          .Lorem-ipsum-dolor-si { width: 619px; height: 135px; margin: 30px 25px
          67px 27px; font-family: WorkSans; font-size: 18px; font-weight:
          normal; font-stretch: normal; font-style: normal; line-height: 1.5;
          letter-spacing: -0.64px; text-align: center; color: var(--white); }
        </p>
      </v-row>
      <v-row justify="center">
        <p class="Resource">Resource</p>
      </v-row>
      <v-row justify="center">
        <p class="These-cases-are-perf">
          These cases are perfectly simple and easy to distinguish. In a free
          hour, when our power of choice is untrammelled and when nothing
          prevents our being able to do what we like best
        </p>
      </v-row>
      <v-row justify="center">
        <p class="Help-Tips">Help & Tips</p>
      </v-row>
      <v-row justify="center" align="center">
        <v-col v-for="(tips, i) in tips" :key="i" cols="auto">
          <v-card class="mx-auto" max-width="400">
            <v-img class="white--text align-end" height="200px" :src="tips.image">
              <v-card-title class="cardColor">
                <v-row>
                  <v-col cols="9">
                    <p
                      style="width: 218px;
  height: 38px;
  margin: 0 16px 0 0;
  font-family: WorkSans;
  font-size: 16px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: -0.57px;
  color: white;"
                    >{{ tips.title }}</p>
                  </v-col>
                  <v-col>
                    <v-btn fab>
                      <v-img
                        src="./assets/oval-icon.png"
                        srcset="./assets/oval-icon@2x.png 2x, ./assets/oval-icon@3x.png 3x"
                        class="Oval-Icon"
                      ></v-img>
                    </v-btn>
                  </v-col>
                </v-row>
              </v-card-title>
            </v-img>
          </v-card>
        </v-col>
      </v-row>
      <v-row justify="center">
        <p class="Youre-all-set">You’re all set.</p>
      </v-row>
      <!-- <v-img
        contain
        class="ml-auto"
        src="./assets/group-3.png"
        srcset="./assets/group-3@2x.png 2x, ./assets/group-3@3x.png 3x"
        style="width: 159px;
  height: 158px;
  margin: 0 0 184px 212px;"
      ></v-img>-->

      <v-row justify="center" align="center">
        <v-col cols="auto">
          <p
            style="width: 619px;
  height: 54px;
  margin: 30px 25px 203px 27px;
  font-family: WorkSans;
  font-size: 18px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.5;
  letter-spacing: -0.64px;
  text-align: center;
  color:white;"
          >
            The wise man therefore always holds in these matters to this
            principle of selection.
          </p>
        </v-col>
      </v-row>
      <div>
        <v-img
          contain
          src="./assets/group-3.png"
          srcset="./assets/group-3@2x.png 2x, ./assets/group-3@3x.png 3x"
          style="width: 159px;
                height: 158px;
                margin: 127px 71px 0 0;
                "
        ></v-img>
      </div>
      <v-toolbar color="#021bf9">
        <v-toolbar-title
          class="ml-15 xs bottomTool"
          style="width: 98px;
                height: 19px;
                margin: 2px 716px 3px 0;
                font-family: WorkSans;
                font-size: 16px;
                font-weight: bold;
                font-stretch: normal;
                font-style: normal;
                line-height: normal;
                letter-spacing: normal;
                color: white;"
        >wknd@2020</v-toolbar-title>
      </v-toolbar>
    </v-container>
  </v-app>
</template>

<script>
import axios from "axios";

export default {
  name: "App",

  data: () => ({
    width: 200,
    slider: [],
    tips: [],
  }),
  mounted() {
    this.getComment();
    this.getTips();
  },
  methods: {
    getTips() {
      axios
        .get(`https://wknd-take-home-challenge-api.herokuapp.com/help-tips`)
        .then((res) => {
          console.log(res);
          this.tips = res.data;
        })
        .catch((err) => console.log(err));
    },
    getComment() {
      axios
        .get(`https://wknd-take-home-challenge-api.herokuapp.com/testimonial`)
        .then((res) => {
          console.log(res);
          this.slider = res.data;
          console.log(this.slider);
        })
        .catch((err) => console.log(err));
    },
  },
};
</script>
<style scoped>
.BG_1 {
  width: 1366px;
  height: 732px;
  padding: 0 0 113px;
  object-fit: contain;
}
.full {
  width: 100%;
  height: 100%;
  background: linear-gradient(to bottom, #eebece 50%, #000000 50%);
}
.text {
  width: 750px;
  height: 51px;
  margin: 84px 322px 20px 323px;
  font-family: WorkSans;
  font-size: 62px;
  font-weight: 900;
  font-stretch: normal;
  font-style: normal;
  line-height: 0.82;
  letter-spacing: normal;
  text-align: center;
  color: var(--white);
}
.Bitmap {
  width: 184px;
  height: 305px;
  margin: 67px 590px 0 592px;
  object-fit: contain;
}
.Group-4 {
  width: 159px;
  height: 158px;
  /* margin: 0 0 184px 1080px; */
  object-fit: contain;
}
.POV {
  height: 38px;
  margin: 148px 131px 30px 132px;
  font-family: WorkSans;
  font-size: 32px;
  font-weight: 900;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: normal;

  color: #ffffff;
}
.Lorem-ipsum-dolor-si {
  width: 619px;
  height: 135px;
  margin: 30px 25px 67px 27px;
  font-family: WorkSans;
  font-size: 18px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.5;
  letter-spacing: -0.64px;
  text-align: center;
  color: #ffffff;
}
.Resource {
  width: 149px;
  height: 38px;
  margin: 67px 89.5px 30px 92.5px;
  font-family: WorkSans;
  font-size: 32px;
  font-weight: 900;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: center;
  color: #ffffff;
}
.These-cases-are-perf {
  width: 619px;
  height: 81px;
  margin: 30px 25px 100px 27px;
  font-family: WorkSans;
  font-size: 18px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.5;
  letter-spacing: -0.64px;
  text-align: center;
  color: #ffffff;
}
.Help-Tips {
  width: 180px;
  height: 38px;
  margin: 100px 75px 30px 76px;
  font-family: WorkSans;
  font-size: 32px;
  font-weight: 900;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: center;
  color: #ffffff;
}
.Youre-all-set {
  width: 218px;
  height: 38px;
  margin: 127px 55px 30px 58px;
  font-family: WorkSans;
  font-size: 32px;
  font-weight: 900;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: center;
  color: #ffffff;
}
.Bitmap2 {
  width: 33px;
  height: 33px;
  margin: 0 13px 0 0;
  object-fit: contain;
}
.Oval-Icon {
  width: 32px;
  height: 32px;
  margin: 3px 0 3px 16px;
  object-fit: contain;
}
.bottomTool {
  margin-left: 500px;
}
.trial {
  position: absolute;
  bottom: 5px;
  left: 10px;
}
.cardColor {
   background-color: rgba(0, 0, 0, 0.51);
   
 }
 .containerLets{
   margin-top: 200px;   
 }
</style>
