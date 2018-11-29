<template>
  <section>
    Behold your choices:
    <IpsumsList :ipsums="ipsums"/>
  </section>
</template>

<script>
import IpsumsList from './IpsumsList';
import ipsumsApi from '../services/ipsumsApi';

export default {
  data() {
    return {
      ipsums: ipsumsApi.getAll()
    };
  },
  components: {
    IpsumsList
  }
};
</script>

<style>

</style>
