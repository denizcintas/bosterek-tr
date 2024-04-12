<template>

    <section>
        <div class="container">
            <SectionHeader title='Books'
                text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur minus magnam hic dolorem asperiores ducimus. Text" />
            <BookList :books="books"/>
        </div>

    </section>

</template>

<script>
import SectionHeader from "@/components/SectionHeader.vue";
import BookList from "@/components/BookList.vue"
import books from '@/db.js'
export default {
    name: "BooksView",
    components: {
        SectionHeader,
        BookList
    },
    data() {
        return {
            books: books
        }
    }
}
</script>

<style scoped>
.auth-box {
    margin-top: -30px
}
</style>