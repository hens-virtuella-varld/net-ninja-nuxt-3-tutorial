<template>
  <div>
    <header>
      <nav>
        <NuxtLink to="/">Net Ninja Nuxt 3 Tutorial</NuxtLink>
        <ul>
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/products">Products</NuxtLink></li>
        </ul>
         <a href="/about">normal link -- about page</a>
      </nav>
    </header>
    <h2>Home</h2>
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
  </div>
</template>

<script setup></script>

<style scoped>
h2 {
  margin-bottom: 20px;
  font-size: 36px;
}
p {
  margin: 20px 0;
}
</style>
