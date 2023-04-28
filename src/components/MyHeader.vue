<template>
    <div>
        <h1> {{bookName}} </h1>
        <h4>{{yourname}}</h4>
    </div>
    </template>
    
    <script>
    
    export default{ // Exporting Default Object
        name: 'MyHeader',
        props:{ 
    
            bookName:String,
            yourname:String
        }
    }
    
    </script>
    
    <style scoped>
    div

    
    {
        text-align: center;
    }
    h1{
        background-color: rgb(230, 212, 247);
    }
    

    </style>