<template>

  <GuestLayout title="Set new password">

    <div class="mt-10 sm:mx-auto sm:w-full sm:max-w-sm">
      <form class="space-y-6" action="#" method="POST">
        <div>
          <label for="newPassword" class="block text-sm/6 font-medium text-left text-gray-900 dark:text-gray-100">New Password:</label>
          <div class="mt-2">
            <input type="password" name="password" id="new-password" required="" class="block w-full rounded-md bg-white px-3 py-1.5 text-base text-gray-900  outline-1 -outline-offset-1 outline-gray-300 placeholder:text-gray-400  focus:outline-2 focus:-outline-offset-2 focus:outline-indigo-600 sm:text-sm/6 dark:bg-white/5 dark:text-white dark:outline-white/10 dark:placeholder:text-gray-500 dark:focus:outline-indigo-500" />
          </div>
          <label for="password-repeat" class="mt-2 block text-sm/6 font-medium text-left text-gray-900 dark:text-gray-100">Confirm Password:</label>
          <div class="mt-2">
            <input type="password" name="password_repeat" id="password-repeat" required="" class="block w-full rounded-md bg-white px-3 py-1.5 text-base text-gray-900  outline-1 -outline-offset-1 outline-gray-300 placeholder:text-gray-400  focus:outline-2 focus:-outline-offset-2 focus:outline-indigo-600 sm:text-sm/6 dark:bg-white/5 dark:text-white dark:outline-white/10 dark:placeholder:text-gray-500 dark:focus:outline-indigo-500" />
          </div>
        </div>

        <div>
            <div class="text-sm">
              <router-link :to="{name: 'login'}" class="font-semibold text-indigo-600 hover:text-indigo-500 dark:text-indigo-400 dark:hover:text-indigo-300">Go back to Login</router-link>
            </div>
        </div>

        <div>
          <button type="submit" class="flex w-full justify-center rounded-md bg-indigo-600 px-3 py-1.5 text-sm/6 font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600 dark:bg-indigo-500 dark:shadow-none dark:hover:bg-indigo-400 dark:focus-visible:outline-indigo-500">Send code</button>
        </div>
      </form>

      
    </div>
  </GuestLayout>
</template>


<script setup>
import {LockClosedIcon} from '@heroicons/vue/20/solid'
import GuestLayout from '../../components/GuestLayout.vue';
</script>

<style scoped>

</style>