<template>
   
    <div v-for="book of books" :key="book.id">

       
        <SingleBook :book="book" />

    </div>
    
</template>

<script>
import SingleBook from "./singleBook.vue"

export default {
    name: 'BookBox',
    props:{
        books: Array
    },
    components: {
        SingleBook
    }
    
}
</script>

<style scoped>
.bookbox{

    background-color: rgb(86, 74, 143);
    padding: 1em;
    color: rgb(240, 41, 41);
    margin: auto;
}
</style>