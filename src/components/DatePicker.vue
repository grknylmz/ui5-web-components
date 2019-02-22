<template>
  <div>
    <header>
      <h1>DatePicker</h1>
    </header>
    <div class="datepicker-width">
      <ui5-datepicker id="myDatepicker1"></ui5-datepicker>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import "@ui5/webcomponents/dist/DatePicker";

@Component
export default class DatePicker extends Vue {}
</script>

<style scoped>
.datepicker-width {
  width: 320px;
  max-width: 100%;
}
</style>
