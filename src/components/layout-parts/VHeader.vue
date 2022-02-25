<template>
    <header class="bg-white border-dotted border-b-2">
        <div class="sm:container mx-auto flex justify-between items-center">
            <nav class="text-zinc-800">
                <p>Телефон: (499) 340-94-71</p>
                <p>Email: info@future-group.ru</p>
                <h1 class="text-2xl pt-5">Комментарии</h1>
            </nav>
            <div>
              <router-link :to="{ name: 'home' }">
                <img class="w-32" alt="image" :src="image_src">
              </router-link>
            </div>
        </div>
    </header>
</template>

<script>
import image from '../../assets/logo.png'

export default {
    name: "VHeader",
    data() {
        return {
            image_src: image
        }
    }
}
</script>

<style scoped>

</style>

