<script lang="ts">
import { defineComponent } from 'vue';
import TransactionsTable from 'components/TransactionsTable.vue';

export default defineComponent({
  name: 'Block',
  data() {
    return {
      block: this.$route.params.block
    };
  },
  components: {
    TransactionsTable
  }
});
</script>

<template lang="pug">
div.row.col-12
    div.row.col-12.gradient-box
    TransactionsTable(:account='block')
</template>
