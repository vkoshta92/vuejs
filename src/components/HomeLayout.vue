<template>
<div>
    <!-- ya if chalega ya else  agr show true ho to else me jega nhi to else. -->
<!-- <h1 v-if="show">if show true then show</h1>
<h1 v-else>Conditional rendering else block</h1>
<button v-on:click="display">Toggle Element</button> -->

<h1>for loop in vue js</h1>
<table border="1px">
    <tr>
        <td>Id</td>
        <td>Name</td>
        <td>Email</td>


    </tr>
    <tr v-for="user in users" :key="user.id">
        <td>{{user.name}}</td>
        <td>{{user.name}}</td>
        <td>{{user.email}}</td>


    </tr>
</table>


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
        // hello(parameter){
        //     console.log('hello vishnu ji');
        //     alert(parameter);
        // },
        // display(){
        //     // this.show=false;
        //     this.show= !this.show;
        // }
    },
    data(){
        // return {show:true}
       return {
 
            users:[
                {id:1,name:"peter",email:"peter@gmail.com"},
                {id:2,name:"meter",email:"meter@gmail.com"},
                {id:3,name:"ceter",email:"ceter@gmail.com"},
                {id:4,name:"heter",email:"heter@gmail.com"}

            ]
       }
       
        
       

        
    }
};
</script>