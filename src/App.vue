<template>
  <v-app>
    <Sidedrawer
      v-model="draweropen"
    />
    <TopBar @drawerclick="draweropen = !draweropen" />
    <v-content>
      <HelloWorld/>
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';
import Sidedrawer from './components/Sidedrawer';
import TopBar from './components/TopBar';

export default {
  name: 'App',
  components: {
    HelloWorld,
    Sidedrawer,
    TopBar
  },
  data: () => ({
    draweropen: true
  }),
};
</script>
