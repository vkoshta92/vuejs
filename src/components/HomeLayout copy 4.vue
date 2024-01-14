<template>
<div>
    <!-- <h1>Template in vue js</h1> -->
   <div v-html="rowHtml"></div>
    <h3>{{name}}</h3>
    <!-- once ke use se ak bar hi change hoga. -->
    <h3 v-once>{{name}}</h3>

    <h3>{{10+19}}</h3>
    <h4>{{a*b}}</h4>
    <h5>{{ok?"yes":"No"}}</h5>
    <!--  butoon work nhikrega angar niche se false krenge jab km krega -->
    <button v-bind:disabled="disableBtn" v-on:click="updateText()">Click Me</button>
</div>
</template>

<script>
export default {
    name:"HomeLayout",
    data(){
        return {
            name:"vishnu",
            a:10,
            b:20,
            ok:false,
            rowHtml:"<h1>Template in vue js</h1>", // html bhi direct print kra skte hai
            disableBtn:true  // true me button  km nhikrega hlka dikhega par kyoki disabled h uper
        }
    },
    methods:{
        updateText(){
            console.log("this",this);
            // this.name="peter";
            this.ok =!this.ok; // toggle
        }
    }
}
</script>