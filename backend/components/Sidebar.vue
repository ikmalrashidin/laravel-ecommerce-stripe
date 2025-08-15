<template>

    <div class="w-[200px] bg-indigo-700 rounded-l-xl py-4 px-2">
        <!-- Dashboard -->
        <router-link :to="{name: 'app.dashboard'}" class="flex items-center text-gray-100 transition-colors duration-300 hover:bg-black/30 rounded-md py-1 px-2 my-2 hover:text-gray-300">
            <span class="mr-2 ">
                <HomeIcon class="w-5"/>
            </span>
            <span class="text-xs">
                Dashboard
            </span>
        </router-link>
        <!-- Dashboard -->

        <!-- Products -->
        <router-link :to="{name: 'app.dashboard'}" class="flex items-center text-gray-100 transition-colors duration-300 hover:bg-black/30 rounded-md py-1 px-2 my-2 hover:text-gray-300">
            <span class="mr-2 ">
                <ViewListIcon class="w-5" aria-hidden="true"/>
            </span>
            <span class="text-xs">
                Products
            </span>
        </router-link>
        <!-- Products -->
        

        <!-- Users -->
        <router-link :to="{name: 'app.dashboard'}" class="flex items-center text-gray-100 transition-colors duration-300 hover:bg-black/30 rounded-md py-1 px-2 my-2 hover:text-gray-300">
            <span class="mr-2 ">
                <HomeIcon class="w-5"/>
            </span>
            <span class="text-xs">
                Users
            </span>
        </router-link>
        <!-- Users -->


        <!-- Reports -->
        <router-link :to="{name: 'app.dashboard'}" class="flex items-center text-gray-100 transition-colors duration-300 hover:bg-black/30 rounded-md py-1 px-2 my-2 hover:text-gray-300">
            <span class="mr-2 ">
                <HomeIcon class="w-5"/>
            </span>
            <span class="text-xs">
                Reports
            </span>
        </router-link>
        <!-- Reports -->


    </div>

</template>


<script setup> 
    import { HomeIcon, ViewListIcon, UsersIcon, ChartBarIcon } from '@heroicons/vue/24/outline'
</script>


<style scoped>

    

</style>