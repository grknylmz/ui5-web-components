<template>
  <div>
    <header>
      <h1>Button</h1>
    </header>
    <ui5-button v-on:click="onClick" class="samples-margin" type="Default">Enabled</ui5-button>
    <ui5-button v-on:click="onClick" class="samples-margin" disabled>Disabled</ui5-button>
    <ui5-button v-on:click="onClick" class="samples-margin" type="Transparent">Cancel</ui5-button>
    <ui5-button v-on:click="onClick" class="samples-margin" type="Positive" icon-end>Approve</ui5-button>
    <ui5-button v-on:click="onClick" class="samples-margin" type="Negative">Decline</ui5-button>
    <ui5-button v-on:click="onClick" class="samples-margin" type="Emphasized">Subscribe</ui5-button>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import "@ui5/webcomponents/dist/Button";

@Component
export default class Button extends Vue {
  onClick() {
    alert("Hey!");
  }
}
</script>

<style scoped>
.samples-margin {
  margin: 0 8px 8px 0;
}
.status-error {
  color: #b00;
}
.status-warning {
  color: #e9730c;
}
.status-success {
  color: #107e3e;
}
</style>
