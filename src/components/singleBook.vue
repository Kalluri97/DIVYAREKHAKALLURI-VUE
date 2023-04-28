<template>
    <!--div v-if="book.published == false"-->

    <div  :class="book.published ? 'green': 'red' ">
<div>
    <h2 >RANK:{{book.Rank}}</h2><br>
    <h2> NAME:{{book.Name}}</h2>
    <h2> YEAR:{{book.Year}}</h2>
    <h2>REVENUE:{{book.Revenue}}</h2>
</div>
<div>

    <h4>DISH:{{book.Famous_dish}}</h4>
    <h4> SERVED:{{book.Customers_served}}</h4>
    <h4> RATINGS:{{book.Ratings}}</h4>
   
</div>
    
    </div>
</template>

<script>

export default{
    name: 'SingleBook',
    props:{
        book: Array
    }
}
</script>

<style scoped>



h4{
    margin: 2px;
   word-spacing: 50px;
 

}

 h2{
word-spacing: 50px;
} 



div{
    background-color:rgba(247, 173, 173, 0.442);
    padding: 1em;
    text-align: center;
    width: 80%;
    margin: auto;

}

.red{
background-color: rgba(180, 210, 247, 0.412) !important;

}


</style>