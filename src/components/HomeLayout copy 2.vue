<template>
<div>
    <!-- ya if chalega ya else  agr show true ho to else me jega nhi to else. -->
<h1 v-if="show">if show true then show</h1>
<h1 v-else>Conditional rendering else block</h1>
<button v-on:click="display">Toggle Element</button>

<!-- <h2>{{data}}</h2>
<p>{{msg}}</p> -->
<!-- <button v-on:click="hello('data recived')">Call Hello Function</button> -->
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
        },
        display(){
            // this.show=false;
            this.show= !this.show;
        }
    },
    data(){
        return {show:true}
    }
};
</script>