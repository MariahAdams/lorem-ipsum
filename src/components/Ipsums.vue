<template>
  <section>
    Behold your choices:
    <Ipsum />
    <IpsumsList :ipsums="ipsums"/>
  </section>
</template>

<script>
import IpsumsList from './IpsumsList';
import Ipsum from './Ipsum';
import ipsumsApi from '../services/ipsumsApi';

export default {
  data() {
    return {
      ipsums: ipsumsApi.getAll()
    };
  },
  components: {
    IpsumsList,
    Ipsum
  }
};
</script>

<style>

</style>
