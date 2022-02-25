<template>
    <div>
      <CardComponent v-for="comment in comments" :key="comment.id" :comment="comment"></CardComponent>
    </div>
</template>

<script>
import CardComponent from "./CardComponent";
import axios from "axios";

export default {
    name: "IndexComponent",
    components: {
        CardComponent
    },
    data() {
        return {
            comments: null
        }
    },
    mounted() {
        this.getComments()
    },
    methods: {
        getComments() {
            axios.get('http://localhost:8035/api/comments')
                .then(responce => {
                    this.comments = responce.data.data
                })
        },
    }
}
</script>

<style scoped>

</style>
