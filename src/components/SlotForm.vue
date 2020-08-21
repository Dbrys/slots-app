<template >
  <div>
    <slot name="header"></slot>
    <form>
      <slot name="userName"></slot>
    </form>
  </div>
</template>


<script>
export default {
  name: "SlotForm",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
