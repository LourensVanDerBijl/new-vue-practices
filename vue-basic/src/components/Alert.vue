<template>
  <div>
      <div class="alert" :class="mode" role="alert">
          <slot></slot>
      </div>
  </div>
</template>

<script>
export default {
  name: "Alert",
  props: [
      'mode'
  ]
 
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.primary {
    color: #fff;
    background-color: #cce5ff;
    border-color: #b8daff;
}
.success {
    color: #fff;
    background-color: #07b61060;
    border-color: #02610f;
}
.danger {
    color: #fff;
    background-color: #fa01018f;
    border-color: #aa0202;
}
.alert {
    position: relative;
    padding: .75rem 1.25rem;
    margin-bottom: 1rem;
    border: 1px solid transparent;
    border-radius: .25rem;
}
</style>
