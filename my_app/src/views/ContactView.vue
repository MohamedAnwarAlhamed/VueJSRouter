<template>
    <div>
        <h1>Contact</h1>
        <p>{{ message }}</p>
        <button @click="goToUser()">Go to User</button>
    </div>
</template>



<script lang="ts">
import router from '../router';
    export default {
        name: 'ContactView',
        data() {
            return {
                message: 'Hello from ContactView'
            }
        },
        methods:{
            goToUser(){
                router.push({name: 'User', params: {id: 1, name: 'John'}});
            },
        }
    }
</script>

<style></style>