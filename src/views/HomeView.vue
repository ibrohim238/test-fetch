<template>
  <main class="container sm:mx-auto py-3">
    <IndexComponent ref="index"></IndexComponent>
    <CreateComponent/>
  </main>
</template>

<script>
import IndexComponent from "../components/comment/IndexComponent";
import CreateComponent from "@/components/comment/CreateComponent";

export default {
  name: "HomeView",
  components: {
    IndexComponent,
    CreateComponent
  }
}
</script>

<style scoped>

</style>
