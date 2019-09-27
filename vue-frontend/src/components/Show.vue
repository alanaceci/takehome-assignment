<template>
  <!-- PART 4: Add your code here -->
  <div>
  <div>{{name}}</div>
  <Counter v-bind:initialCounter=episodes_seen />
  </div>
</template>

<script>
// PART 4: Add your code here
import Counter from "./Counter.vue";
export default {
  components: {
  Counter
  },
  props: {
    id: Number,
    name: String,
    episodes_seen: Number
  },
  data() {
    return {
        id: this.props.id,
        name: this.props.name,
        episodes_seen: this.props.episodes_seen
    };
  }
};
</script>

<style>
font: bold
</style>
