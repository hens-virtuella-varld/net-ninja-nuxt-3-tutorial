<template>
  <div>
    <Head>
      <Title>Net Ninja | {{ product.title }}</Title>
      <Meta name="description" :content="product.description" />
    </Head>
  </div>
  <div>
    <ProductDetails :product="product" />
  </div>
</template>

<script setup>
const { id } = useRoute().params;
const uri = 'https://fakestoreapi.com/products/' + id;

const { data: product } = await useFetch(uri, { key: id });

if (!product.value) {
  throw createError({
    statusCode: 404,
    statusMessage: 'Page Not Found',
    fatal: true,
  });
}

definePageMeta({
  layout: 'products',
});
</script>
