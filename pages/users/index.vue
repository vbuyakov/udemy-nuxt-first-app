<template>
    <div>
        <input type="text" v-model="userId"/>
        <button @click="onUserLoad">Load users</button> 
    </div>
</template>

<script>
export default {
    data() {
        return {
            userId: ''
        }
    },
    methods: {
        onUserLoad() {
            this.$router.push(`/users/${this.userId}`)
        }
    }
}
</script>
