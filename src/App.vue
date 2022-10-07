<template>
  <div class="container" id="app">

    <AppHeader class="AppHeader" @buttonCliked="headerShow"></AppHeader>

    <AppSidebar class="AppSidebar" v-if="showHeader"></AppSidebar>

    <AppMainContent class="AppMainContent" @buttonCliked="header"></AppMainContent>

  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';

import AppSidebar from './components/AppSidebar.vue';

import AppMainContent from './components/AppMainConent.vue';


export default {
  name: 'App',
  components: {
    AppHeader, AppSidebar, AppMainContent
  },
  data(){
    return{
      showHeader: true
    }
  },
  methods: {
    headerShow(){
      this.showHeader = !this.showHeader
    }
  }
}
</script>


<style scoped>

.container 
{  
  display: grid;
  grid-template-columns: auto 1.6fr;
  grid-template-rows: 0.2fr 1.1fr;
  grid-auto-columns: 1fr;
  gap: 0px 0px;
  grid-auto-flow: row;
  grid-template-areas:
    "AppHeader AppHeader"
    "AppSidebar AppMainContent";
  height: 100vh;

}

.AppHeader { grid-area: AppHeader; }

.AppSidebar { grid-area: AppSidebar; }

.AppMainContent { grid-area: AppMainContent; }

</style>
