<template>
  <v-app>
    

    <v-content>
      <HelloWorld v-on:x="setX" v-if="x===false"/>
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',
  components: {
    HelloWorld,
  },
  data: () => ({
    x:false,
  }),
  methods:{
    setX(){
      this.x=true;
    }
  }
};
</script>
