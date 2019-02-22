<template>
  <div class="home">
    <div class="snippet">
      <Button/>
    </div>
    <div class="snippet">
      <Checkbox/>
    </div>
    <div class="snippet">
      <DatePicker/>
    </div>
    <div class="snippet">
      <Dialog/>
    </div>
    <div class="snippet">
      <Card/>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Button from "@/components/Button.vue";
import Card from "@/components/Card.vue";
import Checkbox from "@/components/Checkbox.vue";
import DatePicker from "@/components/DatePicker.vue";
import Dialog from "@/components/Dialog.vue";

@Component({
  components: {
    Button,
    Card,
    Checkbox,
    DatePicker,
    Dialog
  }
})
export default class Home extends Vue {}
</script>


<style scoped>
.snippet {
  padding: 1rem 1.5rem;
  border: 0.0625rem solid #c1c1c1;
}
</style>