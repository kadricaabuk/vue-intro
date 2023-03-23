<script>
    const title = 'LOGO'

    export default {
        name: "HeaderComponent",
        data: () => {
            return {
                title
            }
        },
        methods: {
            log(l){
                console.log(l)
            },
        }
    }
</script>
<template>
    <header>
        <h1>{{title}}</h1>
        <nav>
            <button @click="log($event)">Home</button>
            <button @click="log($event)">About</button>
            <button @click="log($event)">Contact</button>
        </nav>
    </header>    
</template>
<style>
    header{
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color: red;
        color: white;
        padding: 0 16px;
    }
    a {
        color: white;
        text-decoration: none;
    }
    a:not(:last-child){
        margin-right: 10px;
    }
</style>