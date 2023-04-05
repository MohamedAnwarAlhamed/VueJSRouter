<template>
    <div>
        <h1>User</h1>
        <p>{{ messages }}</p>
        <router-view></router-view>
    </div>
</template>

<script lang="ts">
    export default {
        name: 'UserView',
        data() {
            return {
                messages: 'Hello from UserView'
            }
        }
    }

</script>

<style></style>