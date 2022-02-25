<template>
  <VHeader/>
  <router-view/>
  <VFooter/>
</template>

<script>
import VHeader from "@/components/layout-parts/VHeader";
import VFooter from "@/components/layout-parts/VFooter";

export default {
  name: 'App',
  components: {
    VHeader,
    VFooter
  },
}
</script>

<style>
</style>
