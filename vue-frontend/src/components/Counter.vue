<template>
<div>
  {{count}}
  <button v-on:click="count += 1"> + 1 </button>
  <button v-on:click="count -= 1"> - 1 </button>
</div> 
</template>

<script>
import Vue from 'vue'
export default {
props: ['initialCounter'],
data: function () {
    return {
        count: this.initialCounter
    }
}
};
</script>

<style>

</style>
