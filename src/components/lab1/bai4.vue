<template>
 <nav class="navbar navbar-expand-lg bg-body-tertiary">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">
        <img src="/images/logo-energy-pilates.png" alt="" style="width: 150px;">
      </a>

      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarNavDropdown">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">
              <i class="bi bi-pencil-square"></i> Bài viết
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">
              <i class="bi bi-play-btn"></i> Video
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">
              <i class="bi bi-info-circle"></i> Giới Thiệu
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">
              <i class="bi bi-calendar-event"></i> Sự kiện
            </a>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              <i class="bi bi-person-circle"></i> Tài khoản
            </a>
            <ul class="dropdown-menu">
              <li><a class="dropdown-item" href="#"><i class="bi bi-box-arrow-in-right"></i> Đăng nhập</a></li>
              <li><a class="dropdown-item" href="#"><i class="bi bi-key"></i> Quên Mật khẩu</a></li>
              <li><a class="dropdown-item" href="#"><i class="bi bi-person-plus"></i> Đăng kí thành viên</a></li>
            </ul>
          </li>
        </ul>

        <ul class="navbar-nav d-flex">
          <li class="nav-item">
            <a class="nav-link">
              <i class="bi bi-translate"></i> Tiếng Việt
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link">
              <i class="bi bi-translate"></i> Tiếng Anh
            </a>
          </li>
        </ul>
      </div> 
    </div>
  </nav>

  <div class="container">
  <section class="row">
    <!-- Sidebar thông tin cá nhân bên trái -->
    <aside class="col-sm-4 p-3 rounded">
      <!-- <div class="col-sm-4"> -->
      <h2 class="text-info mb-4">Về tôi</h2>
      <div class="card blog">
        <img src="/images/avatar.png" class="card-img-top" aLt="..">
        <div class="card-body">
          <h5 class="card-title">Giới thiệu bản thân</h5>
          <p class="card-text">TS. Trần Hoàng, Tổ chức Tư vấn sức khe quốc tế độc lập <br>
              Châm ngôn: Ta không được chọn nơi mình sinh ra, nhưng ta được chọn cách mình sẽ sống
          </p>
        </div>
      </div>

      <h3 class="text-info mt-2">Chuyên mục</h3>
      <ul class="list-group">
        <li class="list-group-item active bg-info d-flex justify-content-between align-items-center">
          <a class="nav-link" href="#">Chế độ tập</a>
          <span cLass="badge bg-primary rounded-pill">12</span>
        </li>

        <li class="list-group-item d-flex justify-content-between align-items-center">
          <a class="nav-link" href="#">Chế độ dinh dưỡng</a>
          <span class="badge bg-primary rounded-pill">15</span>
        </li>

        <li class="list-group-item d-flex justify-content-between align-items-center">
          <a class="nav-link" href="#">Cẩm nang cuộc sống</a>
          <span class="badge bg-primary rounded-pill">99</span>
        </li>
      </ul>
    <!-- </div> -->
    </aside>

    <!-- Nội dung chính bên phải -->
    <article class="col-sm-8 p-3 rounded">
      <h2 class="text-info mb-4">Blog của tôi</h2>


  <div class="row">
    <!-- Main Post -->
    <div class="col-md-8 main-post">
      <h5>Phương pháp tập Pilates giúp phục hồi chấn thương cột sống <span class="text-muted">💬 16</span></h5>
      <img src="/images/tap-piltes.jpg" alt="" style="width: 550px">
      <p>Ngoài việc giúp duy trì vóc dáng, cải thiện sự linh hoạt, dẻo dai cho người tập, Pilates giúp cơ bắp và các khớp mọc dài hơn, kéo giãn hơn...</p>
    </div>

    <!-- Related Posts -->
    <div class="col-md-4 related-posts">
      <div class="media">
        <img src="/images/corevalue.jpg" alt="Post Image" style="width: 50px">
        <div class="media-body">
          <h6 class="mt-0">Biết ơn đời, đời sẽ thương ta</h6>
          <span class="text-muted">💬 30</span>
        </div>
      </div>
      <div class="media">
        <img src="/images/orange_300x300.jpg" alt="Post Image" style="width: 50px">
        <div class="media-body">
          <h6 class="mt-0">9 tác dụng tuyệt vời của quả cam</h6>
          <span class="text-muted">💬 28</span>
        </div>
      </div>
      <div class="media">
        <img src="/images/sesameoil_300x300.jpg" alt="Post Image" style="width: 50px">
        <div class="media-body">
          <h6 class="mt-0">10 công dụng bất ngờ từ dầu dừa</h6>
          <span class="text-muted">💬 15</span>
        </div>
      </div>
      <div class="media">
        <img src="/images/spinach_300x300.jpg" alt="Post Image" style="width: 50px">
        <div class="media-body">
          <h6 class="mt-0">Lợi ích khi ăn rau mỗi ngày</h6>
          <span class="text-muted">💬 12</span>
        </div>
      </div>
    </div>
  </div>

  <!-- View More Button -->
  <div class="text-center">
    <button class="view-more-btn">Xem thêm</button>
  </div>

</article>


  </section>
  <footer class="row bg-dark text-white p-3 text-center justify-content-center">&copy; 2024 Blog của Tôi. Tất cả quyền được bảo lưu.</footer>
</div>



    </template>
    
    <script>

    
    export default {
        name: "Lab1Bai4",
    
    }
    </script>
    
    <style>
    
    </style>