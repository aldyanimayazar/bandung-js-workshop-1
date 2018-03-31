<template>
  <div class="hello">
    <h1>Halo Nama saya {{ firstname }} {{ lastname }}</h1>
    <p>I live in {{ address.city }}, {{ address.province }}</p>
    <a :href="fbUrl">My Facebook Page</a>
    <button class="btn btn-default">Testing</button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      firstname: "Aldyan",
      lastname: "Imayazar",
      address: {
        city: "Bandung",
        province: "West Java"
      },
      fbUrl: "http://facebook.com",
      btnState: true
    };
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
