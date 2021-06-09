<template>
  <Layout>

    <h1>Image compression test</h1>

    <h2>Regular img tag</h2>
    <figure>
      <img src="images/01.jpg" alt="">
      <figcaption>To display this image, I use regular img tag.<br>No compression, everything looks good</figcaption>
    </figure>

    <h2>g-image component</h2>
    <figure>
      <g-image src="~/assets/images/01.jpg" quality="100"  alt="" />
      <figcaption>To display this image, I use g-image.<br>There is a lot of compression, even though I set the quality attribut to 100.</figcaption>
    </figure>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Hello, world!'
  }
}
</script>

<style>

img {
  max-width: 100%;
}
</style>
