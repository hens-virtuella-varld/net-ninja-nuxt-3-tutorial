<template>
  <div>
    <h2>About</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum,
      necessitatibus temporibus officiis tenetur tempora consectetur dolor eius
      reiciendis ad, illo porro veniam inventore quasi enim fugit! Unde officia
      officiis eligendi!
    </p>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum,
      necessitatibus temporibus officiis tenetur tempora consectetur dolor eius
      reiciendis ad, illo porro veniam inventore quasi enim fugit! Unde officia
      officiis eligendi!
    </p>
    <div>{{ data }}</div>
  </div>
</template>

<script setup>
const { data } = await useFetch('/api/ninja?name=mario', {
  method: 'post',
  body: { age: 30 },
});
</script>

<style scoped>
h2 {
  margin-bottom: 20px;
  font-size: 36px;
}
p {
  margin: 20px 0;
}
</style>
