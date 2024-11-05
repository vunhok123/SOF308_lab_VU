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

    <div class="container">
  <div class="row">
    <!-- Sidebar thông tin cá nhân bên trái -->
    <aside class="col-md-3 bg-light p-3 border rounded">
      <!-- Ảnh đại diện -->
      <div class="text-center mb-3">
        <img
          src="https://via.placeholder.com/100"  
          alt="Avatar"
          class="rounded-circle img-fluid"
        />
      </div>
      
      <!-- Thông tin cơ bản -->
      <h2 class="text-primary text-center">John Doe</h2>
      <p class="text-center text-muted">Nhà phát triển phần mềm</p>

      <!-- Mô tả ngắn -->
      <p class="text-center">Đam mê công nghệ và lập trình, với 5 năm kinh nghiệm trong lĩnh vực phát triển phần mềm và ứng dụng di động.</p>

      <!-- Thông tin liên hệ -->
      <h4 class="text-primary mt-4">Liên hệ</h4>
      <ul class="list-unstyled">
        <li><i class="bi bi-envelope"></i> johndoe@example.com</li>
        <li><i class="bi bi-telephone"></i> +84 123 456 789</li>
        <li><i class="bi bi-geo-alt"></i> Thành phố Hồ Chí Minh, Việt Nam</li>
      </ul>

      <!-- Liên kết mạng xã hội -->
      <h4 class="text-primary mt-4">Kết nối</h4>
      <ul class="list-inline text-center">
        <li class="list-inline-item">
          <a href="#" class="text-primary"><i class="bi bi-facebook"></i></a>
        </li>
        <li class="list-inline-item">
          <a href="#" class="text-primary"><i class="bi bi-twitter"></i></a>
        </li>
        <li class="list-inline-item">
          <a href="#" class="text-primary"><i class="bi bi-instagram"></i></a>
        </li>
        <li class="list-inline-item">
          <a href="#" class="text-primary"><i class="bi bi-linkedin"></i></a>
        </li>
      </ul>
    </aside>

    <!-- Nội dung chính bên phải -->
    <main class="col-md-9 p-3">
      <h1>Nội dung chính</h1>
      <p>Đây là khu vực chứa nội dung chính của trang web.</p>
    </main>
  </div>
</div>



    </template>
    
    <script>
    export default {
        name: "Lab1Bai3",
    
    }
    </script>
    
    <style>
    
    </style>