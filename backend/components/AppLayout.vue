<template>

    <div class="min-h-screen flex">

        <!-- Sidebar -->
            <Sidebar />
        <!-- Sidebar -->


        <div class="flex-1">
        <!-- Header -->
            <TopHeader />
        <!-- Header -->


        <!-- Content -->
        <main>
            <router-view></router-view>
        </main>
        <!-- Content -->

        </div>
    </div>
</template>


<script setup>  // add lang="ts" if using code below
// const props = defineProps<{ title: string }>()

const {title} = defineProps ({
    title: String
})

// use props.title if needed in script; in template we reference {{ title }}

const emit = defineEmits(['submit'])

import Sidebar from './Sidebar.vue'
import TopHeader from './TopHeader.vue'

</script>


<style scoped>

    

</style>