<template>
  <Html>
  <Head>
    <Title>blog</Title>
    <Link rel="stylesheet" href="https://unpkg.com/@picocss/pico@latest/css/pico.min.css"/>
  </Head>
  </Html>
  <Body>
    <div>
      <Header class="container"/>
      <main class="container">
        <NuxtPage/>
      </main>
      <Footer class="container"/>
    </div>
  </Body>
</template>

<style scoped>
:root {
  --primary: #d81b60;
}
</style>
