<template>
  <div class="">
    <div>
      <p><input type="text" v-model="km" /> km</p>
      <p><input type="text" v-model="m" /> m</p>
      <p><input type="text" v-model="mm" /> mm</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "UnitConversion",
  data() {
    return {
      km: 0,
      m: 0,
      mm: 0
    };
  },
  watch: {
    km: function(value) {
      this.km = value;
      this.m = value * 1000;
      this.mm = value * 1000000;
    },
    m: function(value) {
      this.km = value / 1000;
      this.m = value;
      this.mm = value * 1000;
    },
    mm: function(value) {
      this.km = value / 1000000;
      this.m = value / 1000;
      this.mm = value;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
