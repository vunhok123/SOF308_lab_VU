<template>
<nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavDropdown">
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Bài viết</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Video</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Giới Thiệu</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Sự kiện</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Tài khoản
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#">Đăng nhập</a></li>
            <li><a class="dropdown-item" href="#">Quên Mật khẩu</a></li>
            <li><a class="dropdown-item" href="#">Đăng kí thành viên</a></li>
          </ul>
        </li>
      </ul>
      
    </div>
    <span class="navbar-text">
       Tiếng Việt    Tiếng Anh
      </span>
  </div>
</nav>
</template>

<script>
export default {
    name: "Lab1Bai2",

}
</script>

<style>

</style>