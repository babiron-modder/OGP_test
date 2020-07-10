<template>
  <div class="container">
    <div>
      <Logo />
      <h1 class="title">
        ogp_test
      </h1>
      <p>v0.0.1</p>
    </div>
  </div>
</template>

<script>
export default {
  head() {
    return {
      meta: [
        { hid: 'og:description', property: 'og:description', content: '説明のテスト' },
        { hid: 'og:url', property: 'og:url', content: 'https://ogp-test.vercel.app/' },
        { hid: 'og:image', property: 'og:image', content: 'https://ogp-test.vercel.app/ogp_image.png' },
        { name: "twitter:card", content: 'summary_large_image' },
        { name: "twitter:title", content: 'Twitter上でのタイトル' },
        { name: "twitter:description", content: 'Twitter上で説明' },
        { name: "twitter:image", content: 'https://ogp-test.vercel.app/ogp_image.png' },
      ]
    }
  }}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
