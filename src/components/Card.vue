<template>
  <div>
    <header>
      <h1>Card</h1>
    </header>
    <ui5-card heading="New Purchase Orders" subtitle="Today" status="1 of 15" class="medium">
      <ui5-table class="demo-table content-padding">
        <ui5-table-column data-ui5-slot="columns">
          <div data-ui5-slot="header">
            <ui5-label>Sales Order</ui5-label>
          </div>
        </ui5-table-column>

        <ui5-table-column data-ui5-slot="columns">
          <div data-ui5-slot="header">
            <ui5-label>Customer</ui5-label>
          </div>
        </ui5-table-column>

        <ui5-table-column data-ui5-slot="columns">
          <div data-ui5-slot="header">
            <ui5-label>Net Amount</ui5-label>
          </div>
        </ui5-table-column>

        <ui5-table-column data-ui5-slot="columns" min-width="450" popin-text="Status" demand-popin>
          <div data-ui5-slot="header">
            <ui5-label>Status</ui5-label>
          </div>
        </ui5-table-column>

        <ui5-table-row data-ui5-slot="rows" slot="rows-1">
          <ui5-table-cell slot="cells-1">
            <div class="double-line-content" slot="content-1">
              <span>
                <b>Notebook Basic 15</b>
              </span>
              <span style="margin-top: 0.5rem">HT-1000</span>
            </div>
          </ui5-table-cell>
          <ui5-table-cell slot="cells-2">
            <span class="middle" slot="content-1">Very Best Screens</span>
          </ui5-table-cell>
          <ui5-table-cell slot="cells-3">
            <span class="middle" slot="content-1">30 x 18 x 3cm</span>
          </ui5-table-cell>
          <ui5-table-cell slot="cells-4">
            <span style="color: #2b7c2b" class="middle" slot="content-1">
              <b>4.2</b>KG
            </span>
          </ui5-table-cell>
          <ui5-table-cell slot="cells-5">
            <span class="middle" slot="content-1">
              <b>956</b>EUR
            </span>
          </ui5-table-cell>
        </ui5-table-row>
      </ui5-table>
    </ui5-card>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import "@ui5/webcomponents/dist/Card";
import "@ui5/webcomponents/dist/Table";


@Component
export default class Card extends Vue {}
</script>

<style scoped>
.status-error {
  color: #b00;
}
.status-warning {
  color: #e9730c;
}
.status-success {
  color: #107e3e;
}
.content-padding {
  padding: 0.5rem 1rem 0 1rem;
}
</style>
