<template>
  <nav class="navbar navbar-expand-lg bg-body-tertiary">
    <div class="container-fluid">
      <!-- Thêm logo vào thanh điều hướng -->
      <a class="navbar-brand d-flex align-items-center" href="bai1">
        <img
          src="./img/logo-energy-pilates.png"
          alt="Logo"
          style="width: 100px; height: 40px; margin-right: 8px"
        />
      </a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNavDropdown"
        aria-controls="navbarNavDropdown"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavDropdown">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="bai2"
              >Bài viết</a
            >
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
            <a
              class="nav-link dropdown-toggle"
              href="#"
              role="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
            >
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
      <span class="navbar-text"> Tiếng Việt | Tiếng Anh </span>
    </div>
  </nav>

  <!-- Main Content Section -->
  <div class="container mt-4">
    <div
      id="carouselExampleIndicators"
      class="carousel slide"
      data-bs-ride="carousel"
    >
      <div class="carousel-indicators">
        <button
          type="button"
          data-bs-target="#carouselExampleIndicators"
          data-bs-slide-to="0"
          class="active"
          aria-current="true"
          aria-label="Slide 1"
        ></button>
        <button
          type="button"
          data-bs-target="#carouselExampleIndicators"
          data-bs-slide-to="1"
          aria-label="Slide 2"
        ></button>
        <button
          type="button"
          data-bs-target="#carouselExampleIndicators"
          data-bs-slide-to="2"
          aria-label="Slide 3"
        ></button>
      </div>
      <div class="carousel-inner">
        <div class="carousel-item active">
          <img src="./img/banner1.jpg" class="d-block w-100" alt="..." />
        </div>
        <div class="carousel-item">
          <img src="./img/banner2.jpg" class="d-block w-100" alt="..." />
        </div>
        <div class="carousel-item">
          <img src="./img/banner3.jpg" class="d-block w-100" alt="..." />
        </div>
      </div>
      <button
        class="carousel-control-prev"
        type="button"
        data-bs-target="#carouselExampleIndicators"
        data-bs-slide="prev"
      >
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button
        class="carousel-control-next"
        type="button"
        data-bs-target="#carouselExampleIndicators"
        data-bs-slide="next"
      >
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
    </div>

    <section class="row">
      <!-- Sidebar on the Left -->
      <aside class="col-lg-4 col-md-6 p-3 rounded">
        <h2 class="text-info mb-4">Về tôi</h2>
        <div class="card blog">
          <img src="./img/avatar.png" class="card-img-top" alt="Avatar" />
          <div class="card-body">
            <h5 class="card-title">Giới thiệu bản thân</h5>
            <p class="card-text">
              TS. Trần Hoàng, Tổ chức Tư vấn sức khỏe quốc tế độc lập <br />
              Châm ngôn: Ta không được chọn nơi mình sinh ra, nhưng ta được chọn
              cách mình sẽ sống
            </p>
          </div>
        </div>

        <h3 class="text-info mt-2">Chuyên mục</h3>
        <ul class="list-group">
          <li
            class="list-group-item active bg-info d-flex justify-content-between align-items-center"
          >
            <a class="nav-link" href="#">Chế độ tập</a>
            <span class="badge bg-primary rounded-pill">12</span>
          </li>
          <li
            class="list-group-item d-flex justify-content-between align-items-center"
          >
            <a class="nav-link" href="#">Chế độ dinh dưỡng</a>
            <span class="badge bg-primary rounded-pill">15</span>
          </li>
          <li
            class="list-group-item d-flex justify-content-between align-items-center"
          >
            <a class="nav-link" href="#">Cẩm nang cuộc sống</a>
            <span class="badge bg-primary rounded-pill">99</span>
          </li>
        </ul>
      </aside>

      <!-- Main Blog Content on the Right -->
      <article class="col-lg-8 col-md-6 p-3 rounded">
        <h2 class="text-info mb-4">Blog của tôi</h2>

        <div class="row">
          <!-- Main Post -->
          <div class="col-md-8 main-post">
            <h5>
              Phương pháp tập Pilates giúp phục hồi chấn thương cột sống
              <span class="text-muted">💬 16</span>
            </h5>
            <img src="./img/tap-piltes.jpg" alt="Pilates" class="img-fluid" />
            <p>
              Ngoài việc giúp duy trì vóc dáng, cải thiện sự linh hoạt, dẻo dai
              cho người tập, Pilates giúp cơ bắp và các khớp mọc dài hơn, kéo
              giãn hơn...
            </p>
          </div>

          <!-- Related Posts -->
          <div class="col-md-4 related-posts">
            <div class="media">
              <img src="./img/corevalue.jpg" alt="Post" class="img-thumbnail" />
              <div class="media-body">
                <h6 class="mt-0">Biết ơn đời, đời sẽ thương ta</h6>
                <span class="text-muted">💬 30</span>
              </div>
            </div>
            <div class="media mt-3">
              <img
                src="./img/orange_300x300.jpg"
                alt="Post"
                class="img-thumbnail"
              />
              <div class="media-body">
                <h6 class="mt-0">9 tác dụng tuyệt vời của quả cam</h6>
                <span class="text-muted">💬 28</span>
              </div>
            </div>
            <div class="media mt-3">
              <img
                src="./img/sesameoil_300x300.jpg"
                alt="Post"
                class="img-thumbnail"
              />
              <div class="media-body">
                <h6 class="mt-0">10 công dụng bất ngờ từ dầu dừa</h6>
                <span class="text-muted">💬 15</span>
              </div>
            </div>
            <div class="media mt-3">
              <img
                src="./img/spinach_300x300.jpg"
                alt="Post"
                class="img-thumbnail"
              />
              <div class="media-body">
                <h6 class="mt-0">Lợi ích khi ăn rau mỗi ngày</h6>
                <span class="text-muted">💬 12</span>
              </div>
            </div>
          </div>
        </div>

        <!-- View More Button -->
        <div class="text-center">
          <button class="btn btn-primary">Xem thêm</button>
        </div>
      </article>
    </section>
  </div>

  <!-- Sidebar: Most Read Section -->
  <div class="container mt-4">
    <section class="row">
      <!-- Sidebar on the Left -->
      <aside class="col-sm-4 p-3 rounded">
        <h3 class="text-info mb-4">Đọc nhiều</h3>
        <div class="col-md-4 related-posts">
          <div class="media">
            <img src="./img/corevalue.jpg" alt="Post" class="img-thumbnail" />
            <div class="media-body">
              <h6 class="mt-0">Biết ơn đời, đời sẽ thương ta</h6>
              <span class="text-muted">💬 30</span>
            </div>
          </div>
          <div class="media mt-3">
            <img
              src="./img/orange_300x300.jpg"
              alt="Post"
              class="img-thumbnail"
            />
            <div class="media-body">
              <h6 class="mt-0">9 tác dụng tuyệt vời của quả cam</h6>
              <span class="text-muted">💬 28</span>
            </div>
          </div>
        </div>
      </aside>

      <!-- Video Section -->
      <article class="col-sm-8 p-3 rounded">
        <h2 class="text-center">VIDEO - ĐỪNG BỎ LỠ</h2>
        <div class="bg-light p-3">
          <div class="row g-3 mb-4">
            <div class="col-md-6">
              <div class="card">
                <img
                  src="./img/video1.jpg"
                  class="card-img-top"
                  alt="Video 1"
                />
                <div class="card-body">
                  <h5 class="card-title">Đi xa hơn để trưởng thành hơn</h5>
                  <p class="card-text">
                    Tuổi trẻ chỉ nghĩ đến những chuyến đi, đời mong một ngày
                    được bay nhảy trên những phương trời mới lạ. Để rồi những cô
                    đơn mê mải, tuổi trẻ ấy mới muốn một nơi để trở về.
                  </p>
                </div>
              </div>
            </div>

            <div class="col-md-6">
              <div class="card">
                <img
                  src="./img/video2.jpg"
                  class="card-img-top"
                  alt="Video 2"
                />
                <div class="card-body">
                  <h5 class="card-title">Chút tâm tư những ngày cuối năm</h5>
                  <p class="card-text">
                    Guồng quay cuộc sống dù có vội vàng, dù có tấp nập đến đâu
                    thì cũng chẳng nằm ngoài quy luật tự nhiên và bất biến xuân,
                    hạ, thu, đông. Và rồi một năm cũ sắp trôi qua.
                  </p>
                </div>
              </div>
            </div>
          </div>

          <div class="row g-3 mb-4">
            <div class="col-md-6">
              <div class="card">
                <img
                  src="./img/video3.jpg"
                  class="card-img-top"
                  alt="Video 3"
                />
                <div class="card-body">
                  <h5 class="card-title">Ước gì được trở về tuổi thơ</h5>
                  <p class="card-text">
                    Tuổi trẻ chỉ nghĩ đến những chuyến đi, đời mong một ngày
                    được bay nhảy trên những phương trời mới lạ. Để rồi những cô
                    đơn mê mải, tuổi trẻ ấy mới muốn một nơi để trở về.
                  </p>
                </div>
              </div>
            </div>

            <div class="col-md-6">
              <div class="card">
                <img
                  src="./img/video4.jpg"
                  class="card-img-top"
                  alt="Video 4"
                />
                <div class="card-body">
                  <h5 class="card-title">Ba người thầy vĩ đại</h5>
                  <p class="card-text">
                    Ta xem vạn vật là thầy. Tinh thần học hỏi của ta luôn rộng
                    mở hơn tất cả các người. Ta học hỏi từ tất cả mọi vật, từ
                    cành cây ngọn cỏ đến đám mây trên trời kia.
                  </p>
                </div>
              </div>
            </div>
          </div>
          <div class="text-center">
            <button class="btn btn-primary">Xem thêm</button>
          </div>
        </div>
      </article>
    </section>
  </div>
  <footer class="bg-dark text-white text-center py-3 mt-auto">
    <p class="mb-0">&copy;Copyright by FPT Polytechnic</p>
  </footer>
</template>

<script>
export default {
  name: "Lab3Bai1",
};
</script>

<style scoped>
/* Optional custom styles */
.navbar {
  background-color: #f8f9fa;
}

.container-fluid img.img-fluid {
  max-height: 500px;
  object-fit: cover;
}

.btn-primary {
  background-color: #007bff;
  color: white;
  padding: 0.5rem 1.5rem;
  border-radius: 5px;
}

.main-post img {
  width: 100%;
  height: auto;
  border-radius: 8px;
}

.media img {
  width: 50px;
  height: 50px;
  border-radius: 50%;
}
</style>
