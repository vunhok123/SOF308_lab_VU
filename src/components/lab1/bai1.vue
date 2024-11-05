<template>
    <div class="container">
<header class="row bg-warning p-2">Header</header>
<nav class="row bg-primary p-2">Nav</nav>
<section class="row">
<aside class="col-sm-4 bg-success p-5">Side bar</aside>
<article class="col-sm-8 bg-info p-5">Main content</article>
</section>
<footer class="row bg-danger p-3">Footer</footer>
</div>

</template>

<script>
export default {
    name: "Lab1Bai1",

}
</script>

<style>
/* Toàn bộ trang */
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}

/* Header */
.header {
  background-color: yellow;
  color: black;
  padding: 15px;
  text-align: center;
  font-size: 24px;
}

/* Navigation */
.nav {
  background-color: #0072bb; /* Màu xanh nước */
  color: white;
  padding: 10px;
  text-align: center;
  font-size: 18px;
}

/* Layout của trang chính */
.layout {
  display: flex;
}

/* Sidebar */
.sidebar {
  background-color: #4CAF50; /* Màu xanh lá cây */
  color: white;
  width: 25%; /* Chiếm 25% chiều rộng */
  padding: 15px;
  box-sizing: border-box;
}

/* Main Content */
.main-content {
  background-color: #b3d9ff; /* Màu xanh nước nhạt */
  color: black;
  width: 75%; /* Chiếm 75% chiều rộng */
  padding: 15px;
  box-sizing: border-box;
}

/* Footer */
.footer {
  background-color: red;
  color: white;
  padding: 10px;
  text-align: center;
  font-size: 16px;
}

</style>