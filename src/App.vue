<template>
  <div id="app">
    <v-app> 
      <p> {{ message }} </p> 
      <v-tabs fixed-tabs class="elevation-1" id="tabs" > 
        <v-tab class="tab-names"> Brewing Ratio </v-tab>
        <v-tab class="tab-names"> Espresso Drinks </v-tab>
        <v-tab-item> 
          <v-card flat> 
            <v-card-text> 
              <BrewingMethods/>
            </v-card-text>
          </v-card>
        </v-tab-item>
        <v-tab-item> 
          <v-card flat> 
            <v-card-text> 
            </v-card-text>
          </v-card>
        </v-tab-item>
      </v-tabs>
    </v-app>
  </div>
</template>

<script>
import BrewingMethods from "./components/BrewingMethods"; 

export default {
  name: 'app',
  components: {
    BrewingMethods
  },
  data: function() { 
    return {
      message: "JavaS Koffee"
    }
  }
}
</script>

<style scoped>
/* #app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
p { 
  font-size: 2em; 
  text-align: center; 
  margin-top: 20px; 
  margin-bottom: 20px; 
}
div { 
  font-family: "Avenir", Arial, Helvetica, sans-serif; 
}

.tabs {
  margin-top: 30px; 
}

.tab-names { 
}
</style>
