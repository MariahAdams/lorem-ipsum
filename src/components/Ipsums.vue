<template>
  <section>
    Behold your choices:
    <Ipsum :ipsum="selected"/>
    <IpsumsList 
      :ipsums="ipsums"
      :onSelect="handleSelect"
    />
  </section>
</template>

<script>
import IpsumsList from './IpsumsList';
import Ipsum from './Ipsum';
import ipsumsApi from '../services/ipsumsApi';

export default {
  data() {
    return {
      ipsums: ipsumsApi.getAll(),
      selected: null
    };
  },
  components: {
    IpsumsList,
    Ipsum
  },
  methods: {
    handleSelect(ipsum) {
      this.selected = ipsum;
      console.log('You have selected ', ipsum.title);
    }
  }
};
</script>

<style>
section {
  margin: 20px;
}
</style>
