<template>
    <div class="row">
     
        <div class="col-sm-6 col-md-4 col-xl-3 mb-4" v-for="book in books" :key="book.id">
            <div class="card border-0 shadow position-relative">
          <BookItem :book="book"/>
            </div>
        </div>

    </div>
</template>

<script>
import BookItem from "@/components/BookItem.vue"
export default {
    name: "BookList",
    components:{
        BookItem
    },
    props:{
        books:{
            type:Array,
            defualt:()=>([])
        }
    }
}
</script>

<style lang="scss" scoped></style>