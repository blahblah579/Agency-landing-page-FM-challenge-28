<template>
  <v-container fluid class="pa-0">
    <v-row class="">
      <v-col class="head d-flex flex-column">
        <v-col class="d-flex pa-7 justify-space-between">
          <!-- Logo Section -->
          <div class="logo">sunnyside</div>

          <!-- BURGER MENU -->
          <v-app v-if="!isScreenLarge" class="d-md-none d-flex menu">
            <v-menu offset-y :close-on-content-click="false" :nudge-top="30">
              <template #activator="{ props }">
                <v-icon v-bind="props">mdi-menu</v-icon>
              </template>

              <v-card class="container">
                <v-list class="custom-menu text-center">
                  <v-list-item class="my-4" to="/about">
                    <v-list-item-title>About</v-list-item-title>
                  </v-list-item>
                  <v-list-item class="my-4" to="/services">
                    <v-list-item-title>Services</v-list-item-title>
                  </v-list-item>
                  <v-list-item class="my-4" to="/projects">
                    <v-list-item-title>Projects</v-list-item-title>
                  </v-list-item>
                  <v-list-item class="my-4" to="/contact">
                    <div><div class="contact2">CONTACT</div></div>
                  </v-list-item>
                </v-list>
              </v-card>
            </v-menu>
          </v-app>

          <!-- Navigation Links -->
          <div class="links d-none d-md-flex pt-4 pr-1">
            <a href="#">About</a>
            <a class="mx-11" href="#">Services</a>
            <a class="mr-10" href="#">Projects</a>
            <div><div class="contact">CONTACT</div></div>
          </div>
        </v-col>
        <v-col class="second mt-8 d-flex flex-column align-center">
          <div class="creatives d-flex flex-column justify-center align-center">
            WE ARE CREATIVES
          </div>

          <div class="img2 mt-10 mt-lg-16">
            <img src="/src/assets/icon-arrow-down.svg" alt="" />
          </div>
        </v-col>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12" class="d-flex flex-wrap pa-0">
        <v-col cols="12" class="right02 d-md-none pa-0">
          <img
            src="/src/assets/desktop/image-transform.jpg"
            alt="Transform Image"
          />
          <div class="transparent-overlay"></div>
        </v-col>
        <v-col cols="12" md="6" class="left2 d-flex flex-column justify-center">
          <div class="heading2 pr-0 pr-md-10">Transform your brand</div>
          <div class="para2 mt-7 mb-9">
            We are a full-service creative agency specializing in helping brands
            grow fast. Engage your clents through compelling visuals that do
            most of the marketing for you.
          </div>
          <div class="link2 d-flex flex-column align-center align-md-start">
            <div class="text2">LEARN MORE</div>
            <div class="line2"></div>
          </div>
        </v-col>
        <v-col cols="6" class="right2 d-md-flex d-none"> </v-col>
      </v-col>
      <v-col cols="12" class="d-flex flex-wrap pa-0">
        <v-col cols="12" class="right02 d-md-none pa-0">
          <img
            src="/src/assets/desktop/image-stand-out.jpg"
            alt="Transform Image"
          />
          <div class="transparent-overlay"></div>
        </v-col>
        <v-col cols="6" class="d-md-flex d-none right3"> </v-col>
        <v-col cols="12" md="6" class="left3 d-flex flex-column justify-center">
          <div class="heading3">Stand out to the right audience</div>
          <div class="para3 mt-9 mb-10">
            Using a collaborative formula of designers, researchers,
            photographers, videographers, and copywriters, we'll build and
            extend your brand in digital places.
          </div>
          <div class="link3 d-flex flex-column align-center align-md-start">
            <div class="text3">LEARN MORE</div>
            <div class="line3"></div>
          </div>
        </v-col>
      </v-col>
      <v-col cols="12" class="d-none d-md-flex flex-wrap pa-0">
        <v-col cols="6" class="left4 d-flex flex-column align-center">
          <div class="heading4 text-center">Graphic Design</div>
          <div class="para4 mt-5 mb-10">
            Great design makes you memorable. We deliver artwork that
            underscores your brand message and captures potential clients'
            attention.
          </div>
        </v-col>
        <v-col
          cols="6"
          class="left5 d-flex flex-column justify-center align-center"
        >
          <div class="heading5">Photography</div>
          <div class="para5 mt-5 mb-10">
            Increase your credibility by getting the most stunning, high-quality
            photos that improve your business image.
          </div>
        </v-col>
      </v-col>

      <!-- Graphic Design and Photography for SMALLER SCREENS-->
      <v-col cols="12" class="d-flex d-md-none flex-column pa-0">
        <v-col class="left4 d-flex flex-column justify-center align-center">
          <div class="heading4 text-center">Graphic Design</div>
          <div class="para4 mt-5 mb-10">
            Great design makes you memorable. We deliver artwork that
            underscores your brand message and captures potential clients'
            attention.
          </div>
        </v-col>
        <v-col class="left5 d-flex flex-column justify-center align-center">
          <div class="heading5">Photography</div>
          <div class="para5 mt-5 mb-10">
            Increase your credibility by getting the most stunning, high-quality
            photos that improve your business image.
          </div>
        </v-col>
      </v-col>

      <v-col class="pa-0">
        <ClientTest />
      </v-col>
      <v-col cols="12" class="d-flex flex-wrap pa-0">
        <v-col cols="6" md="3" class="pa-0">
          <img
            class="img20"
            src="/src/assets/desktop/image-gallery-milkbottles.jpg"
            alt=""
          />
        </v-col>
        <v-col cols="6" md="3" class="pa-0">
          <img
            class="img20"
            src="/src/assets/desktop/image-gallery-orange.jpg"
            alt=""
          />
        </v-col>
        <v-col cols="6" md="3" class="pa-0">
          <img
            class="img20"
            src="/src/assets/desktop/image-gallery-cone.jpg"
            alt=""
          />
        </v-col>
        <v-col cols="6" md="3" class="pa-0">
          <img
            class="img20"
            src="/src/assets/desktop/image-gallery-sugarcubes.jpg"
            alt=""
          />
        </v-col>
      </v-col>
      <v-col class="foot pa-0">
        <v-col class="d-flex flex-column align-center">
          <div class="heading30 mt-10">sunnyside</div>
          <div
            class="links-bottom d-flex justify-space-between align-center mt-8 mb-14"
          >
            <a class="pa-0" href="#">About</a>
            <a class="py-0 mid1" href="#">Services</a>
            <a class="pa-0" href="#">Projects</a>
          </div>
          <div class="social d-flex pt-4 mb-10 justify-space-between">
            <div class="logo1">
              <v-icon icon="mdi-facebook"></v-icon>
            </div>
            <div class="logo2 pl-6 pr-3">
              <v-icon icon="mdi-instagram"></v-icon>
            </div>
            <div class="logo3 pl-3 pr-6">
              <v-icon icon="mdi-twitter"></v-icon>
            </div>
            <div class="logo4">
              <v-icon icon="mdi-pinterest"></v-icon>
            </div>
          </div>
        </v-col>
      </v-col>
    </v-row>
  </v-container>
</template>
  
  <script setup>
document.addEventListener("DOMContentLoaded", () => {
  const text3 = document.querySelector(".text3");
  const line3 = document.querySelector(".line3");

  if (text3 && line3) {
    text3.addEventListener("mouseenter", () => {
      line3.style.backgroundColor = "hsl(6, 100%, 69%)";
    });

    text3.addEventListener("mouseleave", () => {
      line3.style.backgroundColor = "hsl(3, 88%, 90%)";
    });

    line3.addEventListener("mouseenter", () => {
      line3.style.backgroundColor = "hsl(6, 100%, 69%)";
    });

    line3.addEventListener("mouseleave", () => {
      line3.style.backgroundColor = "hsl(3, 88%, 90%)";
    });
  }
});
document.addEventListener("DOMContentLoaded", () => {
  const text2 = document.querySelector(".text2");
  const line2 = document.querySelector(".line2");

  if (text2 && line2) {
    text2.addEventListener("mouseenter", () => {
      line2.style.backgroundColor = "hsl(52, 100%, 49%)";
    });

    text2.addEventListener("mouseleave", () => {
      line2.style.backgroundColor = "hsl(53, 97%, 85%)";
    });

    line2.addEventListener("mouseenter", () => {
      line2.style.backgroundColor = "hsl(52, 100%, 49%)";
    });

    line2.addEventListener("mouseleave", () => {
      line2.style.backgroundColor = "hsl(53, 97%, 85%)";
    });
  }
});

import { ref, onMounted, onUnmounted } from "vue";
import ClientTest from "./ClientTest.vue";

const isScreenLarge = ref(window.innerWidth >= 599.5);

function updateScreenSize() {
  isScreenLarge.value = window.innerWidth >= 599.5;
}

onMounted(() => {
  window.addEventListener("resize", updateScreenSize);
});

onUnmounted(() => {
  window.removeEventListener("resize", updateScreenSize);
});
</script>
  
  <style scoped>
@font-face {
  font-family: f1;
  src: url(/src/assets/Barlow-Black.ttf);
}
@font-face {
  font-family: f2;
  src: url(/src/assets/Fraunces_144pt_SuperSoft-Regular.ttf);
}
@font-face {
  font-family: f3;
  src: url(/src/assets/Fraunces_9pt_SuperSoft-Bold.ttf);
}
@font-face {
  font-family: f4;
  src: url(/src/assets/Barlow-Regular.ttf);
}
@font-face {
  font-family: f5;
  src: url(/src/assets/Fraunces_9pt-Black.ttf);
}
@font-face {
  font-family: f6;
  src: url(/src/assets/Fraunces_72pt-Regular.ttf);
}
@font-face {
  font-family: f7;
  src: url(/src/assets/Barlow-SemiBold.ttf);
}
.head {
  background-image: url("@/assets/desktop/image-header.jpg");
  background-size: cover; /* Contain the whole image within the div */
  background-position: center; /* Center the image */
  background-repeat: no-repeat; /* Prevent repetition */
}
.second {
  margin-bottom: 260px;
}

.bar {
  padding-left: 47px;
  padding-right: 47px;
  padding-top: 40px;
}

.logo {
  font-size: 30px;
  font-weight: bold;
  color: white; /* White text for the logo */
  letter-spacing: 2px;
  font-family: f1;
}
.links a {
  text-decoration: none; /* Removes underline */
  color: white; /* White text for links */
  font-size: 16px;
  font-weight: 500;
  transition: color 0.3s ease;
  font-family: f4;
  font-weight: 500;
}
.links a:hover {
  color: #f0e68c; /* Optional: Hover effect (light yellow) */
}
.contact {
  background-color: #fff;
  color: hsl(212, 16%, 16%);
  border-radius: 50px;
  font-family: f2;
  font-size: 14px;
  font-weight: bolder;
  letter-spacing: 1px;
  position: relative;
  top: -10px;
  padding-left: 30px;
  padding-right: 30px;
  padding-top: 14px;
  padding-bottom: 14px;
}
.contact:hover {
  background-color: hsl(198, 97%, 71%);
  color: hsl(0, 0%, 100%);
}
.contact2 {
  background-color: hsl(51, 99%, 49%);
  color: hsl(212, 16%, 16%);
  border-radius: 50px;
  font-family: f2;
  font-size: 14px;
  font-weight: bolder;
  letter-spacing: 1px;
  position: relative;
  top: -10px;
  padding-left: 30px;
  padding-right: 30px;
  padding-top: 14px;
  padding-bottom: 14px;
  margin-top: 10px;
}
.contact2:hover {
  background-color: hsl(198, 97%, 71%);
  color: hsl(0, 0%, 100%);
}
.creatives {
  font-size: 50px;
  font-family: f3;
  letter-spacing: 10px;
  text-align: center;
}
.img2 {
  scale: 0.9;
}
.line2,
.line3 {
  width: 122px; /* Full width, adjust as needed */
  height: 10px; /* Thickness of the line */
  border-radius: 30px; /* Rounded edges */
  position: relative;
  top: -8px;
  z-index: 0;
  cursor: pointer;
}
.line2 {
  background-color: hsl(53, 97%, 85%);
}
.line3 {
  background-color: hsl(3, 88%, 90%);
}
.left2 {
  background-color: hsl(26, 100%, 99%);
  padding-left: 160px;
  padding-right: 70px;
}
.left02 {
  background-color: #fff;
}
.left3 {
  background-color: hsl(26, 100%, 99%);
  padding-left: 106px;
  padding-right: 126px;
}
.heading2 {
  color: hsl(205, 26%, 18%);
  font-family: f5;
  font-size: 38px;
  margin-top: 135px;
  line-height: 43px;
}
.heading3 {
  color: hsl(205, 26%, 18%);
  font-family: f5;
  font-size: 38px;
  margin-top: 143px;
  line-height: 43px;
}
.para2,
.para3 {
  color: hsl(244, 6%, 52%);
  font-weight: 500;
  font-size: 16px;
}
.text2,
.text3 {
  cursor: pointer;
  color: hsl(205, 26%, 18%);
  font-family: f5;
  font-size: 14px;
  z-index: 1;
  left: 10px;
  position: relative;
}
.link2,
.link3 {
  margin-bottom: 130px;
}
.right2 {
  background-image: url("/src/assets/desktop/image-transform.jpg");
  background-size: cover; /* Ensures the image covers the entire div */
  background-position: center; /* Centers the image */
  background-repeat: no-repeat; /* Prevents the image from repeating */
  width: 100%; /* Full width of the parent container */
  height: 100%; /* Full height of the parent container */
}
.right02 {
  width: 100vw; /* Take full viewport width */
  height: 70vh; /* Full viewport height */
  position: relative; /* Needed to properly position child elements */
  overflow: hidden; /* Prevents content overflow */
}

.right02 img {
  width: 100%; /* Stretch horizontally */
  height: 100%; /* Stretch vertically */
  object-fit: cover; /* Ensures the image covers the container without distortion */
  display: block; /* Prevents any extra spacing */
}

/* Transparent overlay ensures the <v-col> renders */
.transparent-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0); /* Fully transparent */
  pointer-events: none; /* Prevents interaction with the overlay */
}
.right3 {
  background-image: url("/src/assets/desktop/image-stand-out.jpg");
  background-size: cover; /* Ensures the image covers the entire div */
  background-position: center; /* Centers the image */
  background-repeat: no-repeat; /* Prevents the image from repeating */
  width: 100%; /* Full width of the parent container */
  height: 100%; /* Full height of the parent container */
}

.para4 {
  color: hsl(167, 36%, 33%);
  font-weight: 500;
  font-size: 15px;
  font-family: f7;
  text-align: center;
}
.left4 {
  padding-left: 160px;
  padding-right: 160px;
  background-image: url("/src/assets/desktop/image-graphic-design.jpg");
  background-size: cover; /* Ensures the image covers the entire element */
  background-position: center; /* Centers the image */
  background-repeat: no-repeat; /* Prevents the image from repeating */
  width: 100%;
  height: 100%;
}
.left5 {
  padding-left: 160px;
  padding-right: 160px;
  background-image: url("/src/assets/desktop/image-photography.jpg");
  background-size: cover; /* Ensures the image covers the entire element */
  background-position: center; /* Centers the image */
  background-repeat: no-repeat; /* Prevents the image from repeating */
  width: 100%;
  height: 100%;
}
.heading4 {
  color: hsl(168, 49%, 22%);
  font-family: f5;
  font-size: 25px;
  margin-top: 337px;
  line-height: 43px;
}
.heading5 {
  color: hsl(200, 58%, 27%);
  font-family: f5;
  font-size: 25px;
  margin-top: 337px;
  line-height: 43px;
}
.para5 {
  color: hsl(200, 58%, 27%);
  font-weight: 500;
  font-size: 15px;
  font-family: f7;
  text-align: center;
}
.img20 {
  width: 100%;
  height: 100.1%;
}
.heading30 {
  font-size: 30px;
  font-weight: bold;
  color: hsl(166, 44%, 32%); /* White text for the logo */
  letter-spacing: 2px;
  font-family: f1;
}
.foot {
  background-color: hsl(167, 44%, 70%);
}
.links-bottom {
  padding-left: 500px;
  padding-right: 500px;
}
.links-bottom a {
  text-decoration: none; /* Removes underline */
  color: hsl(167, 29%, 47%); /* White text for links */
  font-size: 16px;
  font-weight: 500;
  transition: color 0.3s ease;
  font-family: f7;
  font-weight: 500;
}
.links-bottom a:hover {
  color: #ffffff; /* Optional: Hover effect (light yellow) */
}
.logo1,
.logo2,
.logo3,
.logo4 {
  color: hsl(166, 44%, 32%);
}
.logo1:hover,
.logo2:hover,
.logo3:hover,
.logo4:hover {
  color: rgb(255, 255, 255);
  cursor: pointer;
}
.social {
  padding-left: 550px;
  padding-right: 550px;
}
.menu {
  height: 50px;
  background-color: transparent;
  position: relative;
  top: 13px;
}
.custom-menu {
  position: relative;
  background-color: hsl(26, 100%, 99%);
  padding: 8px 16px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  min-width: 200px;
  color: hsl(240, 4%, 53%);
  border-radius: 0px;
  font-family: f7;
}

/* Triangle at the top-right of the menu */
/* .custom-menu::before {
  content: "";
  position: absolute;
  top: -0px;
  right:0px;
  width: 0;
  height: 0;
  border-left: 20px solid transparent;
  border-right: 1px solid transparent;
  border-bottom: 30px solid rgb(206, 20, 20);
} */
.container {
  position: relative;
  top: 5px;
  right: 20px;
}
.mid1 {
  padding-right: 60px;
  padding-left: 60px;
}
@media (max-width: 959.5px) {
  .left2 {
    background-color: hsl(26, 100%, 99%);
    padding-left: 70px;
    padding-right: 70px;
  }
  .left3 {
    padding-left: 50px;
    padding-right: 50px;
  }
  .heading2,
  .heading3 {
    text-align: center;
    margin-top: 70px;
  }
  .para2,
  .para3 {
    text-align: center;
    padding-left: 20px;
    padding-right: 20px;
  }
  .line2,
  .line3 {
    right: -5px;
  }
  .left4,
  .left5 {
    padding-left: 25px;
    padding-right: 25px;
  }
  .creatives {
    text-align: center;
    margin-top: 0px;
    line-height: 60px;
  }
  .head {
    background-image: url("@/assets/desktop/image-header.jpg");
    background-size: cover; /* Contain the whole image within the div */
    background-position: center; /* Center the image */
    background-repeat: no-repeat; /* Prevent repetition */
    height: 120vh; /* Full height of the viewport */
    width: 100vw; /* Full width of the container */
  }
  .link2,
  .link3 {
    margin-bottom: 45px;
  }
  .mid1 {
    padding-right: 120px;
    padding-left: 120px;
  }
  .text2,
  .text3 {
    left: 5px;
  }
}
</style>
  