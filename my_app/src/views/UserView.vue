<template>
    <div>
        <h1>User</h1>
        <p>{{ messages }}</p>
        <ul>
            <li v-for="item in list" :key="item.id">
                {{ item.name }}
            </li>
        </ul>
    </div>
</template>

<script lang="ts">
import * as Vue from 'vue'
import axios from 'axios';
import VueAxios from 'vue-axios';

Vue.use(VueAxios, axios);
    export default {
        name: 'UserView',
        data() {
            return {
                messages: 'Hello from UserView',
                list:undefined
            }
        },
        created(){
            vue.axios.get('https://jsonplaceholder.typicode.com/users')
            .then(response => {
                this.list = response.data;
            })
            .catch(error => {
                console.log(error);
            })
        }
    }

</script>

<style></style>