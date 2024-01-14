<template>
<div>
<h1>Hello from home component</h1>
<!-- <h2>{{data}}</h2>
<p>{{msg}}</p> -->
<button v-on:click="hello('data recived')">Call Hello Function</button>
</div>


</template>


<script>
export default {
    name:'HomeLayout',
    props:{
        data:String,
        msg:String
    },
    methods:{
        hello(parameter){
            console.log('hello vishnu ji');
            alert(parameter);
        }
    }
};
</script>