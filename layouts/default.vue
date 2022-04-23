<template>
  <Nuxt />
</template>

<script>
export default {
  name: 'DefaultLayout',
}
</script>


<style >
@import url('https://fonts.googleapis.com/css2?family=Rubik:wght@400;500;600;700&display=swap');

body {
  font: 16px 'Rubik', sans-serif;
  margin: 0;
  color: var(--color-900);
  overflow-x: hidden;
  background-color: var(--color-000);
}

:root {
  --color-000: #1f1f1f;
  --color-900: rgba(255, 255, 255, 0.82);
  --main: #681a1a;
  --main-l: #7a2a2a;
}

body {
  min-height: -webkit-fill-available;
}
html {
  height: -webkit-fill-available;
}

h1,
h2,
p {
  margin: 0;
  padding: 0;
  line-height: 1;
}

a,
a:hover,
a:active,
:visited {
  list-style: none;
  text-decoration: none;
  color: inherit;
}
</style>