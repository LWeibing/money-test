<template>
  <button class="button" @click="$emit('click',$event)">
    <slot></slot>
  </button>
</template>

<script lang="ts">
  import Vue from 'vue';
  import {Component} from 'vue-property-decorator';

  @Component
  export default class Button extends Vue {

  }
</script>

<style lang="scss" scoped>
  .button {
    background: rgb(255,153,0);
    color: white;
    border-radius: 4px;
    border: none;
    height: 40px;
    padding: 0 16px;
  }
</style>