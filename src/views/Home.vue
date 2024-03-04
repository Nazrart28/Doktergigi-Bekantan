<template>
  <Navbar />
<v-main>
  <v-container fluid>
    <v-row>
      <v-col cols="12">
        <v-row>
          <v-col cols="12" sm="6">
            <h1 class="title1">
              It's A Big World<br />
              Out There, Go <br />Explore
            </h1>
            <p class="par1">
              Conveniently customiz proactiv web service for<br />
                  leveraged without continualliery aggregate fricctionle
                  <br />ou wellies richard.and very customize continually.
            </p>
            <v-btn class="text-noe mt-8 bt1" color="indigo-lighten-1" size="x-large" variant="flat" rounded="0">
              Get Exploration
            </v-btn>
            <v-btn class="text-none ml-2 text-indigo-lighten-1 mt-8" size="x-large" variant="flat" rounded="0">
              Read More
            </v-btn>
          </v-col>
          <v-col cols="12" sm="6">
            <v-img src="/13.png" class="img1"></v-img>
          </v-col>
        </v-row>
      </v-col>
      <v-col cols="12" sm="12">
        <v-card flat>
          <v-tabs v-model="tab" color="indigo-lighten-1" align-tabs="center">
          <v-tab :value="1">
          <v-icon class="mr-2">mdi mdi-bed</v-icon>consultation
          </v-tab>
          <v-tab :value="2">
          <v-icon class="mr-2">mdi mdi-bed</v-icon>Check Dental Health
          </v-tab>
          <v-tab :value="3">
          <v-icon class="mr-2">mdi mdi-bed</v-icon>Emergency measures
          </v-tab>
          <v-tab :value="4">
          <v-icon class="mr-2">mdi mdi-bed</v-icon>Install braces
          </v-tab>
        </v-tabs>
        <v-window v-model="tab">
        <v-window-item v-for="n in 4" :key="n" :value="n">
          <v-container fluid>
            <v-row justify="center" align="center">
              <v-col cols="12" sm="2">
                <div class="text-subtile-1 text-medium-emphasis">Select Hospital</div>
                <v-select density="compact" placeholder="Destination"  :items="[
                            'Fortis Memorial Research Institute',
                            'Mega Medipol University Hospital',
                            'Pusat Medis Teknon - Grup Quironsalud',
                            'Gleneagles Medini Hospital',
                            'Dar Al Fouad Hospital',
                            'HELIOS Hospital Berlin-Buch',
                          ]"
                          variant="outlined"></v-select>
              </v-col>
              <v-col cols="12" sm="2">
                <div class="text-subtile-1 text-medium-emphasis">Select a date</div>
                <v-text-field density="compact" placeholder="Date" type="date" variant="outlined"></v-text-field>
              </v-col>
              <!-- <v-col cols="12" sm="2">
                <div class="text-subtile-1 text-medium-emphasis">Check out</div>
                <v-text-field density="compact" placeholder="Date" type="date" variant="outlined"></v-text-field>
              </v-col> -->
              <v-col cols="12" sm="2">
                <div class="text-subtile-1 text-medium-emphasis">Specialist</div>
                <v-select density="compact" placeholder="Specialist"  :items="[
                            'Periodonsia specialist',
                            'Orthodontist specialist',
                            'Oral disease specialist',
                            'Dental conservation specialist',
                            'Paediatric dentistry specialist',
                            'Oral surgery specialist',
                          ]"
                          variant="outlined"></v-select>
              </v-col>
              <v-col cols="12" sm="2">
                <div class="text-subtile-1 text-medium-emphasis">Types of treatment</div>
                <v-select density="compact" placeholder="Types of treatment"  :items="[
                            'Scaling',
                            'Sealant',
                            'Tooth fillings',
                            'Root canal treatment',
                            'Tooth extraction',
                            'Fitting of dentures',
                          ]"
                          variant="outlined"></v-select>
              </v-col>
              <v-col cols="12" sm="2">
                <v-btn class="text-none mt-5" color="indigo-lighten-1" size="x-large" variant="flat" rounded="0" elevation="12">
                  Schedule Now
                </v-btn>
              </v-col>
            </v-row>
          </v-container>
        </v-window-item>
      </v-window>
        </v-card>
      </v-col>
      <v-col cols="12" sm="12">
        <h1 class="text-center">Best Doctor Arround The World</h1>
        <v-row justify="center">
          <v-col cols="12" sm="10">
            <v-row>
              <v-col cols="12" sm="4">
                <v-hover v-slot="{ isHovering, props}">
                  <v-card :elevation="isHovering ? 12: 2" :class="{ 'on-hover':isHovering }" v-bind="props" class="card1">
                  <v-img src="/1.jpg" cover height="100%">
                    <div class="d-flex flex-row-reverse">
                      <v-btn class="text-none mr-2 mt-2" color="indigo-lighten-1" size="x-large" variant="flat" rounded="0" elevation="12">
                        Already
                      </v-btn>
                    </div>
                    <div class="text-black top">
                      <h1 class="mt-4">Dr.Angela Petrenko</h1>
                      <div>
                        <p class="ma-0 text-body-1 font-weight-bold">Starting From $1200</p>
                      </div>
                    </div>
                    <div class="d-flex justify-center">
                      <v-btn v-for="(icon, index) in icons" :key="index" variant="text" :class="{ 'show-btns' : isHovering}" :color="transparent" :icon="icon"></v-btn>
                    </div>
                  </v-img>
                  </v-card>
                </v-hover>
              </v-col>
              <v-col cols="4" class="d-flex flex-column">
                <v-row>
                  <v-col cols="12" sm="12">
                    <v-hover v-slot="{ isHovering, props}">
                  <v-card :elevation="isHovering ? 12: 2" :class="{ 'on-hover':isHovering }" v-bind="props" class="card1">
                  <v-img src="/13.jpg" cover height="100%">
                    <div class="d-flex flex-row-reverse">
                      <v-btn class="text-none mr-2 mt-2" color="indigo-lighten-1" size="x-large" variant="flat" rounded="0" elevation="12">
                        Already
                      </v-btn>
                    </div>
                    <div class="text-black top ">
                      <h1 class="mt-10 ml-4">Dr.Olga Tkachenko</h1>
                      <div>
                        <p class="ma-0 text-body-1 font-weight-bold ml-4">Starting From $1900</p>
                      </div>
                    </div>
                    <div class="d-flex justify-center">
                      <v-btn v-for="(icon, index) in icons" :key="index" variant="text" :class="{ 'show-btns' : isHovering}" :color="transparent" :icon="icon"></v-btn>
                    </div>
                  </v-img>
                  </v-card>
                </v-hover>
                  </v-col>
                  <v-col cols="12" sm="12">
                    <v-hover v-slot="{ isHovering, props}">
                  <v-card :elevation="isHovering ? 12: 2" :class="{ 'on-hover':isHovering }" v-bind="props" class="card1">
                  <v-img src="/14.jpg" cover height="100%">
                    <div class="d-flex flex-row-reverse">
                      <v-btn class="text-none mr-2 mt-2" color="indigo-lighten-1" size="x-large" variant="flat" rounded="0" elevation="12">
                        Already
                      </v-btn>
                    </div>
                    <div class="text-black top ">
                      <h1 class="mt-10 ml-4">Dr Stephanie Grossman</h1>
                      <div>
                        <p class="ma-0 text-body-1 font-weight-bold ml-4">Starting From $1500</p>
                      </div>
                    </div>
                    <div class="d-flex justify-center">
                      <v-btn v-for="(icon, index) in icons" :key="index" variant="text" :class="{ 'show-btns' : isHovering}" :color="transparent" :icon="icon"></v-btn>
                    </div>
                  </v-img>
                  </v-card>
                </v-hover>
                  </v-col>
                </v-row>
              </v-col>
              <v-col cols="12" sm="4">
                <v-hover v-slot="{ isHovering, props}">
                  <v-card :elevation="isHovering ? 12: 2" :class="{ 'on-hover':isHovering }" v-bind="props" class="card1">
                  <v-img src="/2.jpg" cover height="100%">
                    <div class="d-flex flex-row-reverse">
                      <v-btn class="text-none mr-2 mt-2" color="indigo-lighten-1" size="x-large" variant="flat" rounded="0" elevation="12">
                        Already
                      </v-btn>
                    </div>
                    <div class="text-black top">
                      <h1 class="mt-4">Dr. Irina Zabalotina</h1>
                      <div>
                        <p class="ma-0 text-body-1 font-weight-bold">Starting From $1600</p>
                      </div>
                    </div>
                    <div class="d-flex justify-center">
                      <v-btn v-for="(icon, index) in icons" :key="index" variant="text" :class="{ 'show-btns' : isHovering}" :color="transparent" :icon="icon"></v-btn>
                    </div>
                  </v-img>
                  </v-card>
                </v-hover>
              </v-col>

            </v-row>
          </v-col>
        </v-row>
      </v-col>
      <v-col cols="12" sm="12">
        <h1 class="text-center">Our Hospital</h1>
        <v-row justify="center">
          <v-col cols="12" sm="10">
            <v-row>
              <v-col cols="12" sm="3" v-for="(popular,i) in populars" :key="i">
                <v-hover v-slot="{isHovering, props}">
                <v-card class="mx-auto" color="grey-lighten-4" max-width="600" v-bind="props">
                <v-img :aspect-ratio="16 /9" cover :src="popular.image">
                <v-expand-transition>
                  <div v-if="isHovering" class="d-flex transition-fast-in-fast-out bg-red-lighten-1 v-card--reveal" style="height: 100%">
                  <v-row>
                    <v-col cols="12" sm="12">
                      <h1 class="ml-4">{{ popular.subtitle1 }}</h1>
                    </v-col>
                    <v-col cols="12" sm="12">
                      <h6 class="ml-4 mt-n4 mb-3">
                        {{ popular.subtitle2 }}
                      </h6>
                    </v-col>
                  </v-row>
                  </div>
                </v-expand-transition>
              </v-img>
              <v-card-text class="pt-6">
                <div class="font-weight-light text-grey text-h6 mb-2">
                  {{ popular.title }}
                </div>
              </v-card-text>
              <v-card-actions>
                <span class="text-grey-darken-2 text-caption me-2">
                  ({{ rating }})
                </span>
                <v-rating v-model="rating" color="white" active-color="yellow-accent-4" half-increments hover size="18"></v-rating>
                <v-spacer></v-spacer>
                <v-btn class="text-none" color="indigo-lighten-1" size="large" variant="flat" rounded="0" elevation="6">$1200</v-btn>
              </v-card-actions>
                </v-card>
                </v-hover>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </v-col>
      <v-col cols="12" sm="12">
        <h1 class="text-center">Choose your service</h1>
        <v-row justify="center">
          <v-col cols="12" sm="10">
            <v-row>
              <v-col cols="12" sm="2" v-for="(offer, i) in offers" :key="i">
                <v-card class="mx-auto px-2 pt-6" height="200px" flat>
                  <div align="center" justify="center">
                    <v-img :src="offer.image" height="100px" width="100px" cover></v-img>

                  </div>
                  <v-card-title class="text-center">
                    <h6>{{ offer.title }}</h6>
                  </v-card-title>
                </v-card>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </v-col>
      <v-col cols="12" sm="12">
        <v-row justify="center">
          <v-col cols="12" sm="10">
            <v-row>
              <v-col cols="12" sm="3" v-for="(hotel, i) in hotels" :key="i">
              <v-hover v-slot="{isHovering,props}">
                <v-card class="mx-auto" color="grey-lighten-4" max-width="600" v-bind="props">
                <v-img :aspect-ratio="16 /9" cover :src="hospital.image">
                  <v-expand-transition>
                    <div v-if="isHovering" class="d-flex transition-fast-in-fast-out bg-teal-lighten-1 v-card--reveal" style="height: 100%;">
                    <v-row>
                      <v-col cols="12" sm="12">
                        <h1 class="ml-4">{{ hospital.subtitle1 }}</h1>
                      </v-col>
                      <v-col cols="12" sm="12">
                        <h6 class="ml-4 mt-n4 mb-3">
                          {{ hospital.subtitle2 }}
                        </h6>
                      </v-col>
                    </v-row>
                    </div>
                  </v-expand-transition>
                </v-img>
                <v-card-text class="pt-6">
                  <div class="font-weight-light text-grey text-h6 mb-2">
                    {{ hospital.title }}
                  </div>
                  <div class="font-weight-light text-caption">
                    <v-icon color="indigo-lighten-1">
mdi mdi-map-marker
                    </v-icon> Bali, Indonesha
                  </div>
                </v-card-text>
                <v-card-actions>
                  <span class="text-grey-darken-2 text-caption me-2">({{ rating }})</span>
                  <v-rating v-model="rating" color="white" active-color="yellow-accent-4" half-increments hover size="18">
                  </v-rating>
                  <v-spacer></v-spacer>
                  <v-btn class="text-none" color="indigo-lighten-1" size="large" variant="flat" rounded="0" elevation="6">$1200</v-btn>
                </v-card-actions>
                </v-card>
              </v-hover>
            </v-col>
            </v-row>
          </v-col>
        </v-row>
      </v-col>
      <!-- <v-col cols=12 sm="12">
          <h1 class="text-center">Best Service Share a Smile</h1>
          <v-sheet class="mx-auto" elevation="8" max-width="1200">
            <v-slide-group v-model="model" class="pa-4" center-active show-arrows>
              <v-slide-group-item v-for="travel in travels" :key="travel" v-slot="{isSelected, toggle}">
                <v-card :color="isSelected ? 'primary' : 'grey-lighten-1'" class="ma-4" height="200" width="130" @click="toggle" flat>
                  <div class="d-flex fill-height align-center justify-center">
                    <v-img :src="travel.image" cover height="100%" width="100%"></v-img>
                  </div>
                </v-card>
              </v-slide-group-item>
            </v-slide-group>
          </v-sheet>
      </v-col> -->
      <v-col cols="12" sm="12">
        <v-card>
          <v-img src="/p.jpg" cover height="100%">
            <div class="d-flex justify-center ligne1">
              <h1>Sign up for our newsletter</h1>
            </div>
            <div class="d-flex justify-center ligne2">
              <v-text-field density="compact" placeholder="Enter your e-main here" variant="solo-inverted" color="#393E50" rounded="0"></v-text-field>
              <v-btn class="text-none tp" color="indigo-lighten-1" size="large" variant="flat" rounded="0" elevation="12">
                Subscribe Now
              </v-btn>
            </div>
          </v-img>
        </v-card>
      </v-col>
 </v-row>
  </v-container>
</v-main>
<Footer />
</template>

<script setup>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
</script>
<script>
export default {
  data: () => ({
    tab: null,
    model: null,
    icons: ["mdi-rewind", "mdi-play", "mdi-fast-forward"],
    transparent: "rgba(255, 255, 255, 0)",
    rating: 4.5,
    populars: [
      {
        image: "UZA Antwerp Hospital.jpg",
        title: " UZA Antwerp Hospital",
        subtitle1: "Belgia",
        money: "$1200",
      },
      {
        image: "European-Medical-Center-EMC.jpg",
        title: " European-Medical-Center-EMC",
        subtitle1: "Russia",
        money: "$1300",
      },
      {
        image: "HELIOS Hospital Schwerin.jpg",
        title: " HELIOS Hospital Schwerin",
        subtitle1: "West Mecklenburg",
        money: "$900",
      },
      {
        image: "Memorial Hospital.jpg",
        title: " Memorial Hospital",
        subtitle1: "Taiwan",
        money: "$1700",
      },
    ],
    offers: [
      {
        image: "i11.png",
        title: "Dental crown",
      },
      {
        image: "i12.png",
        title: "Veneer",
      },
      {
        image: "i13.png",
        title: "Dental bridge",
      },
      {
        image: "i14.png",
        title: "Teeth whitening",
      },
      {
        image: "i15.png",
        title: "Braces",
      },
      {
        image: "i16.png",
        title: "Dental implants",
      },
    ],
    hospital: [
      {
        image: "UZA Antwerp Hospital.jpg",
        title: " UZA Antwerp Hospital",
        subtitle1: "Belgia",
        subtitle2: "4 Day's 3 Night",
        money: "$2000",
      },
      {
        image: "European-Medical-Center-EMC.jpg",
        title: " European-Medical-Center-EMC",
        subtitle1: "Russia",
        subtitle2: "5 Day's 4 Night",
        money: "$2000",
      },
      {
        image: "HELIOS Hospital Schwerin.jpg",
        title: " HELIOS Hospital Schwerin",
        subtitle1: "West Mecklenburg",
        subtitle2: "3 Day's 2 Night",
        money: "$2000",
      },
      {
        image: "Memorial Hospital.jpg",
        title: " Memorial Hospital",
        subtitle1: "Taiwan",
        subtitle2: "4 Day's 3 Night",
        money: "$2000",
      },
    ],
    travels: [
      {
        image: "f1.jpg",
      },
      {
        image: "f2.jpg",
      },
      {
        image: "f3.jpg",
      },
      {
        image: "f4.jpg",
      },
      {
        image: "f5.jpg",
      },
      {
        image: "f6.jpg",
      },
      {
        image: "5.jpg",
      },
      {
        image: "8.jpg",
      },
    ],
  }),
};
</script>
<style scoped>
.title1 {
  color: #1f3347;
  font-size: 50px;
  font-style: bold;
  margin-left: 100px;
  margin-top: 70px;
}
.par1 {
  color: "#AAA1B4";
  margin-left: 100px;
}
.bt1 {
  margin-left: 100px;
}
.img1 {
  width: 1000px !important;
  height: 1000px !important;
  z-index: 1;
  margin-top: -200px;
}
.v-card.card1 {
  transition: opacity 0.4s ease-in-out;
}

.v-card.card1:not(.on-hover) {
  opacity: 0.6;
}

.show-btns {
  color: rgba(255, 255, 255, 1) !important;
}
.top {
  margin-top: 100%;
  margin-left: 20px;
}
.v-card--reveal {
  align-items: end;
  bottom: 0;
  justify-content: start;
  opacity: 0.9;
  position: absolute;
  width: 100%;
}
.ligne1 {
  margin-top: 150px;
}
.ligne2 {
  margin-top: 10px;
  padding: 0 250px 0 250px;
}
.tp {
  margin-top: -2px;
}
</style>
