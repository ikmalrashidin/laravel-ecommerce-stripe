<template>

    <div class="flex min-h-screen flex-1 flex-col justify-center px-6 py-12 lg:px-8">

        
        <div class="sm:mx-auto sm:w-full sm:max-w-sm">
                <h2 class="mt-10 text-center text-3xl font-bold tracking-tight text-gray-900 dark:text-white">
                    {{ title }}
                </h2>
                    <form class="space-y-6" @submit.prevent="emit('submit')" method="POST">
                <slot></slot>
                    </form>
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


</script>


<style scoped>

    

</style>