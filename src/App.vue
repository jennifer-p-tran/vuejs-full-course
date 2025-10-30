<script setup>
import Welcome from '/workspaces/vuejs-full-course/src/components/pages/Welcome.vue'
import Layout from '/workspaces/vuejs-full-course/src/components/layouts/Layout.vue'
</script>


<template>
    <!-- Welcome is now technically a child element to the parent Layout component
        tags. You only have the corresponding closing tag when you are creating
        children elements. -->
    <Layout>
        <Welcome />
    </Layout>
</template>


<style scoped>
</style>