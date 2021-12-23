<template>
  <header>
    <nav>
      <ul>
        <li><h1>Blog</h1></li>
      </ul>
      <ul>
        <li v-for="(nav,i) in navs" :key="i">
          <nuxt-link :to="nav.path">{{nav.name}}</nuxt-link>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script lang="ts" setup>
export interface NavType {
  name: string
  path: string
}
const navs = ref<NavType[]>([
  {
    name: "About",
    path: "/about"
  },
  {
    name: "Hoge",
    path: "/hoge"
  },
  {
    name: "Foo",
    path: "/foo"
  }
])
</script>
