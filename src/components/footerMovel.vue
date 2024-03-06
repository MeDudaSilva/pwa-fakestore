<script>
import SvgIcon from '@jamescoyle/vue-icon';
import { mdiAccount } from '@mdi/js';
import Account from 'vue-material-design-icons/Account.vue';

export default {
  name: "my-cool-component",
  components: {
    SvgIcon
  },
  data() {
    return {
       path: mdiAccount,
    }
  }
}
</script>
<template>
<div>
    <Account />
    <svg-icon type="mdi" :path="path"><SvgIcon/></svg-icon>
</div>
</template>
<style>

</style>