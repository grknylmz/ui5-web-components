<template>
  <div>
    <header>
      <h1>Dialog</h1>
    </header>
    <div class="snippet">
      <ui5-button v-on:click="onClickOpen" id="openDialogButton" type="Emphasized">Open Dialog</ui5-button>

      <ui5-dialog ref="dialog" header-text="Register Form">
        <section class="login-form" slot="content-1">
          <div>
            <ui5-label for="username" required>Username:</ui5-label>
            <ui5-input id="username"></ui5-input>
          </div>

          <div>
            <ui5-label for="password" required>Password:</ui5-label>
            <ui5-input id="password" type="Password" value-state="Error"></ui5-input>
          </div>

          <div>
            <ui5-label for="email" type="Email" required>Email:</ui5-label>
            <ui5-input id="email"></ui5-input>
          </div>

          <div>
            <ui5-label for="address">Address:</ui5-label>
            <ui5-input id="address"></ui5-input>
          </div>
        </section>

        <div
          data-ui5-slot="footer"
          style="display: flex; align-items: center;padding: .5rem"
          slot="footer"
        >
          <div style="flex: 1;"></div>
          <ui5-button id="closeDialogButton" type="Emphasized">Register</ui5-button>
        </div>
      </ui5-dialog>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import "@ui5/webcomponents/dist/Dialog";

interface IDialog {
  open(): any;
}

@Component
export default class Dialog extends Vue {
  onClickOpen() {
    let dialog = this.$refs.dialog;
    dialog.open();
  }
}
</script>

<style scoped>
</style>
