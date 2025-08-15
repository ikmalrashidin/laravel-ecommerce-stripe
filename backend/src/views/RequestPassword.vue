<template>

  <GuestLayout title="Request Password">

    <div class="mt-10 sm:mx-auto sm:w-full sm:max-w-sm">
      <form class="space-y-6" action="#" method="POST">
        <div>
          <label for="email" class="sr-only">Email address</label>
          <div class="mt-2">
            <input type="email" name="email" id="email" autocomplete="email" required placeholder="Email address" class="block w-full rounded-md bg-white px-3 py-1.5 text-base text-gray-900 outline-1 -outline-offset-1 outline-gray-300 placeholder:text-gray-400  focus:outline-2 focus:-outline-offset-2 focus:outline-indigo-600 sm:text-sm/6 dark:bg-white/5 dark:text-white dark:outline-white/10 dark:placeholder:text-gray-500 dark:focus:outline-indigo-500" />
          </div>
        </div>

        <div>
            <div class="text-sm">
              <router-link :to="{name: 'login'}" class="font-semibold text-indigo-600 hover:text-indigo-500 dark:text-indigo-400 dark:hover:text-indigo-300">Remember your password?</router-link>
            </div>
        </div>

        <div>
          <button type="submit" class="flex w-full justify-center gap-2 rounded-md bg-indigo-600 px-3 py-1.5 text-sm/6 font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600 dark:bg-indigo-500 dark:shadow-none dark:hover:bg-indigo-400 dark:focus-visible:outline-indigo-500">
            <LockClosedIcon class="h-5 w-5 text-indigo-500 " aria-hidden="true" />
              Send code</button>
        </div>
      </form>

      
    </div>
  </GuestLayout>
</template>


<script setup>
  import { LockClosedIcon } from '@heroicons/vue/20/solid';
  import GuestLayout from '../../components/GuestLayout.vue';
  
</script>
<style scoped>

</style>