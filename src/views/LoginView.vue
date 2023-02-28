<template>
  <div id="Register">
    <div class="w-full p-6 flex justify-center items-center">

      <div class="w-full max-w-xs">
        <div class="bg-black p-8 shadow rounded mb-6">

          <h1 class="mb-6 text-lg text-gray-100 font-thin">
            Тербел!
          </h1>

          <div class="mb-4">
            <TextInput
                label="Электрондық пошта"
                :label-color="false"
                placeholder="john@gmail.com"
                v-model:input="email"
                input-type="text"
                error="Тестовая ошибка"
            />
          </div>

          <div class="mb-4">
            <TextInput
                label="Құпия сөз"
                :label-color="false"
                placeholder="password123"
                v-model:input="password"
                input-type="text"
                error="Тестовая ошибка"
            />
          </div>

          <button
              class="
            block
            w-full
            bg-green-500
            text-white
            rounded-sm
            py-3
            text-sm
            tracking-wide
            mt-2" type="submit">
            Кіру
          </button>
        </div>

        <p class="text-center text-md text-gray-900">
          Тіркелмегенсізбе?

          <router-link to="register" class="text-blue-500 no-underline hover:underline">
            Тіркелу
          </router-link>

        </p>
      </div>
    </div>
  </div>
</template>

<script setup>
import TextInput from "@/components/global/TextInput";
import {ref} from 'vue'

let email = ref(null)
let password = ref(null)

</script>