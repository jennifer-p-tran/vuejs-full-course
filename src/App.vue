<script setup>
// These 2 lines work on Workspaces
// import Welcome from '/workspaces/vuejs-full-course/src/components/pages/Welcome.vue'
// import Layout from '/workspaces/vuejs-full-course/src/components/layouts/Layout.vue'

// These 2 lines work on Local Machine
// import Welcome from 'C:/Users/tranl/OneDrive/cs-projects/vuejs-full-course/src/components/pages/Welcome.vue'
// import Layout from 'C:/Users/tranl/OneDrive/cs-projects/vuejs-full-course/src/components/layouts/Layout.vue'

// These 2 lines work on both Workspaces and Local Machine
import Welcome from './components/pages/Welcome.vue'
import Layout from './components/layouts/Layout.vue'
import Dashboard from './components/pages/Dashboard.vue'
</script>


<template>
    <!-- 50:00 Welcome is now technically a child element to the parent Layout component
        tags. You only have the corresponding closing tag when you are creating
        children elements. -->
    <Layout>
        <Welcome />
        <Dashboard />
    </Layout>
</template>


<style scoped>
</style>