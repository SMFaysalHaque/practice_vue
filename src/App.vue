<template>
  <header>
    <div class="">
      <Header name="Practice Pops and Emits" />
      <Information :informations="informations"/>
    </div>
    <!-- <RouterView /> -->
  </header>
</template>

<script>
import Header from '../src/components/Header.vue'
import Information from '../src/components/Information.vue'
import AddNewPerson from '../src/components/AddNewPerson.vue';

export default{
  name: 'App',
  components: {
    Header, Information, AddNewPerson,
  },
  data() {
    return {
      informations: []
    }
  },
  created () {
    this.informations = [
      {
        serial: 1,
        name: 'Gabbar Singh',
        mobile: 92547896
      },
      {
        serial: 2,
        name: 'Amitabh Reza',
        mobile: 81445678
      },
      {
        serial: 3,
        name: 'Humaun Ahmed',
        mobile: 2547865486
      }
    ];
  },
}
</script>
