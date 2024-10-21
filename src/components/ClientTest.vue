<template>
  <v-container fluid class="main">
    <v-row>
      <v-col>
        <v-col cols="12" class="text-center">
          <div class="heading">CLIENT TESTIMONIALS</div>
        </v-col>
        <v-col
          cols="12"
          class="d-flex mt-8 body flex-wrap flex-column flex-sm-row justify-center align-center"
        >
          <v-col
            cols="12"
            sm="6"
            md="4"
            class="px-8 d-flex flex-column align-center"
          >
            <div class="profile">
              <v-avatar size="60">
                <v-img alt="John" src="/src/assets/image-emily.jpg"></v-img>
              </v-avatar>
            </div>
            <div class="para10 mt-9 mb-8 mt-md-14 mb-md-15">
              We put our trust in Sunnyside and they delivered, making sure our
              needs were met and deadlines were always hit.
            </div>
            <div class="details text-center">
              <div class="name1">Emily R.</div>
              <div class="position1">Marketing Director</div>
            </div>
          </v-col>
          <v-col
            cols="12"
            sm="6"
            md="4"
            class="px-8 d-flex flex-column align-center"
          >
            <div class="profile">
              <v-avatar size="60">
                <v-img alt="John" src="/src/assets/image-thomas.jpg"></v-img>
              </v-avatar>
            </div>
            <div class="para10 mt-9 mb-8 mt-md-14 mb-md-15">
              Sunnyside's enthusiasm coupled with their keen interest in our
              brand's success made it a satisfying and enjoyable experience.
            </div>
            <div class="details text-center">
              <div class="name1">Thomas S.</div>
              <div class="position1">Chief Operating Officer</div>
            </div>
          </v-col>
          <v-col
            cols="12"
            sm="6"
            md="4"
            class="px-8 d-flex flex-column align-center"
          >
            <div class="profile">
              <v-avatar size="60">
                <v-img alt="John" src="/src/assets/image-jennie.jpg"></v-img>
              </v-avatar>
            </div>
            <div class="para10 mt-9 mb-8 mt-md-14 mb-md-15">
              Incredible end result! Our sales increased over 400% when we
              worked with Sunnyside. Highly recommended!
            </div>
            <div class="details text-center">
              <div class="name1">Jennie F.</div>
              <div class="position1">Business Owner</div>
            </div>
          </v-col>
        </v-col>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
.main {
  background-color: hsl(26, 100%, 99%);
}
.heading {
  margin-top: 112px;
  color: hsl(240, 1%, 65%);
  font-family: f3;
  letter-spacing: 4px;
}
.para10 {
  color: hsl(228, 3%, 39%);
  font-weight: 500;
  text-align: center;
}
.name1 {
  color: hsl(210, 24%, 13%);
  font-family: f3;
}
.position1 {
  color: hsl(40, 2%, 69%);
  font-family: f4;
  font-size: 12px;
  font-weight: 600;
}
.details {
  margin-bottom: 104px;
}
.body {
  padding-left: 105px;
  padding-right: 105px;
}

@media (min-width: 599.5px) and (max-width: 960px) {
  .heading {
    margin-top: 50px;
  }
  .body {
    padding-left: 50px;
    padding-right: 50px;
  }
  .details {
    margin-bottom: 80px;
  }
}

@media (max-width: 599.5px) {
  .details {
    margin-bottom: 40px;
  }
  .heading {
    margin-top: 40px;
  }
}
</style>