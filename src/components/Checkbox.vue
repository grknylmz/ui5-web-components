<template>
  <div>
    <header>
      <h1>Checkbox</h1>
    </header>
    <ui5-checkbox text="Chocolate" checked tabindex="0"></ui5-checkbox>
    <ui5-checkbox text="Strawberry" checked tabindex="0"></ui5-checkbox>
    <ui5-checkbox text="Waffles" checked tabindex="0"></ui5-checkbox>
    <ui5-checkbox text="Cake" checked tabindex="0"></ui5-checkbox>
    <ui5-checkbox text="Pie(unavailable)" disabled tabindex="0"></ui5-checkbox>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import "@ui5/webcomponents/dist/CheckBox";

@Component
export default class Checkbox extends Vue {
  onClick() {
    alert("Hey!");
  }
}
</script>

<style scoped>
</style>
