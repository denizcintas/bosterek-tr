<template>
    <NavBar />
    <RouterView />

</template>

<script>
import NavBar from "@/components/NavBar.vue";
export default {
    name: "App",
    components: {
        NavBar
    },
    data() {
        return {
            message: "merhaba",
            count: 0,
            isVisable: true
        }
    }
}
</script>


<style>
@import url('https://fonts.googleapis.com/css2?family=Mulish:wght@300;400;600;700&display=swap');

body {
    font-family: 'Mulish', sans-serif;
}
</style>