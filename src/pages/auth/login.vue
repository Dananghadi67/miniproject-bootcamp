<script setup lang="ts">
import { Button, Input, FormItem } from '@/components/m'
import Img from '@/assets/images/auth.png'
</script>

<template>
  <main class="flex justify-center bg-foreground-primary text-white min-h-screen">
    <section class="w-1/3 py-20 px-5 h-full">
      <div class="space-y-3 mb-8">
        <div class="text-3xl font-semibold">Welcome Back 👋</div>
        <div class="text-white">We are happy to have you back</div>
      </div>
      <form class="space-y-3">
        <FormItem id="email" label="email" class="w-full">
          <Input
            id="email"
            type="email"
            color="default"
            placeholder="Enter your Email"
            class="w-full"
          />
        </FormItem>
        <FormItem id="password" label="password" class="w-full">
          <Input
            id="password"
            type="password"
            color="default"
            placeholder="Enter your password"
            class="w-full"
          />
        </FormItem>
        <div>
          <Button class="block w-full mt-5" color="primary">Login</Button>
        </div>
      </form>
    </section>
    <section class="flex-1 h-full p-3">
      <div class="rounded-lg overflow-hidden h-full">
        <img :src="Img" class="w-full object-cover" alt="img" />
      </div>
    </section>
  </main>
</template>

<style scoped></style>
