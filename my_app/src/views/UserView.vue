<template>
    <div>
        <h1>User</h1>
        <p>{{ messages }}</p>
        <p>{{ $route.params.id }}</p>
        <p>{{ $route.params.name }}</p>
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