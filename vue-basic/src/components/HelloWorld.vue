<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <alert mode="danger">First</alert>
    <alert mode="primary">Second</alert>
    <alert mode="success">Third</alert>

  </div>
</template>

<script>
import Alert from './Alert.vue';
export default {
  components: { Alert },
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
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
