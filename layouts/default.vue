<template>
  <div class="container m-auto p-10">
    <p class="mb-3 font-semibold italic">Kent Joemar L. Escoto - BSCS</p>
    <hr class="mb-3">
    <header>
      <nav class="container mx-auto">
        <ul class="flex gap-8 font-medium">
          <li>
            <NuxtLink to="/">Home</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/products">Products</NuxtLink>
          </li>
        </ul>
      </nav>
    </header>

    <div>
      <slot />
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>
.router-link-exact-active {
  color: #008b8b;
  font-weight: bold;
}
</style>