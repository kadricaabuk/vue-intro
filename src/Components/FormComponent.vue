<script>
    export default{
        name: "FormComponent",
        data(){
            return {
                formData: []
            }
        },
        methods: {
            handleSumbit(e){
                e.preventDefault();
                console.log(e)
            }
        },
        computed: {
            
        },
    }
</script>
<template>
    <form @submit.prevent="handleSumbit">
        <input type="text">
        <input type="text">
        <button type="submit">Submit</button>
    </form>
</template>