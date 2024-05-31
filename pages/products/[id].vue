<template>
  <div>
    <p>Product details for {{ id }}</p>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Earum temporibus
      nesciunt aspernatur inventore corrupti, possimus numquam mollitia eveniet.
      Pariatur tempora numquam explicabo atque soluta quae facilis harum
      expedita tempore deserunt.
    </p>
  </div>
</template>

<script setup>
const { id } = useRoute().params;
</script>
