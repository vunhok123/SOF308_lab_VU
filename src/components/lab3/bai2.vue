<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-body-tertiary">
    <div class="container-fluid">
      <!-- Logo -->
      <a class="navbar-brand d-flex align-items-center" href="bai1">
        <img
          src="./img/logo-energy-pilates.png"
          alt="Logo"
          class="img-fluid"
          style="max-width: 100px; height: 40px; margin-right: 8px"
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
  </div>

  <!-- Main Content and Sidebar -->
  <section class="row">
    <!-- Sidebar -->
    <aside class="col-lg-4 col-md-12 p-3">
      <h3 class="text-info">Chuyên mục</h3>
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

      <div class="card mt-3">
        <div class="card-header text-info">
          <h3>Bài viết nổi bật</h3>
        </div>
        <div class="list-group list-group-flush">
          <div class="list-group-item">
            <div class="row">
              <div class="col-4">
                <img
                  src="./img/spinach_300x300.jpg"
                  class="img-fluid rounded-circle"
                  alt="avatar"
                />
              </div>
              <div class="col-8">
                <p class="fw-bold">Lợi ích khi ăn rau mỗi ngày</p>
                <p>
                  Tiêu thụ rau xanh hàng ngày sẽ giúp tăng cường thị lực, kiểm
                  soát cân nặng, ngăn ngừa ung thư ...
                </p>
              </div>
            </div>
          </div>
          <div class="list-group-item">
            <div class="row">
              <div class="col-4">
                <img
                  src="./img/orange_300x300.jpg"
                  class="img-fluid rounded-circle"
                  alt="avatar"
                />
              </div>
              <div class="col-8">
                <p class="fw-bold">9 tác dụng tuyệt vời của quả cam</p>
                <p>
                  Cam tự hào về khả năng chống lão hóa mạnh mẽ nhờ hàm lượng
                  chất chống oxy hóa cao ...
                </p>
              </div>
            </div>
          </div>
          <div class="list-group-item">
            <div class="row">
              <div class="col-4">
                <img
                  src="./img/sesameoil_300x300.jpg"
                  class="img-fluid rounded-circle"
                  alt="avatar"
                />
              </div>
              <div class="col-8">
                <p class="fw-bold">10 công dụng bất ngờ từ dầu dừa</p>
                <p>
                  Dầu dừa như một loại kem dưỡng ẩm tự nhiên cho cơ thể, giúp
                  việc sản xuất collagen trong các tế bào ...
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </aside>

    <!-- Main Content Area -->
    <article class="col-lg-8 col-md-12 text-info p-3">
      <h2>Tất cả bài viết</h2>

      <div class="row">
        <div class="col-md-6 mb-4">
          <div class="card">
            <div class="card-header fw-bold">
              <a href="bai3"
                >Phương pháp tập Pilates giúp phục hồi chấn thương cột sống</a
              >
              <span><i class="bi bi-chat-left-fill"> 16</i></span>
            </div>
            <img src="./img/tap-piltes.jpg" class="card-img-top" alt="..." />
            <div class="card-body">
              <p class="card-text">
                Hai người đang tập luyện trên máy Pilates reformer trong một
                phòng tập. Văn bản tiếng Việt đi kèm có thể là hướng dẫn hoặc mô
                tả về phương pháp tập Pilates giúp phục hồi chấn thương cột
                sống.
              </p>
            </div>
          </div>
        </div>
        <div class="col-md-6 mb-4">
          <div class="card">
            <div class="card-header fw-bold">
              Đây là những gì 1 giờ tập Pilates có thể làm cho cơ thể bạn
              <span><i class="bi bi-chat-left-fill"> 8</i></span>
            </div>
            <img src="./img/tap-pilates1.jpg" class="card-img-top" alt="..." />
            <div class="card-body">
              <p class="card-text">
                Được thiết kế để xây dựng cơ bắp săn chắc, khỏe mạnh hơn, bài
                tập này đã trở thành một cái tên quen thuộc nhờ có rất nhiều
                người nổi tiếng theo dõi.
              </p>
            </div>
          </div>
        </div>
      </div>

      <div class="row">
        <div class="col-md-6 mb-4">
          <div class="card">
            <div class="card-header fw-bold">
              Tập Pilates có thể cải thiện sức khoẻ tim mạch của bạn
              <span><i class="bi bi-chat-left-fill"> 5</i></span>
            </div>
            <img src="./img/tim-mach.jpg" class="card-img-top" alt="..." />
            <div class="card-body">
              <p class="card-text">
                Tập Pilates không chỉ giúp bạn có một cơ thể khỏe mạnh và linh
                hoạt mà còn có nhiều lợi ích cho sức khỏe tim mạch. Bài viết này
                sẽ tìm hiểu sâu hơn về tác động tích cực của việc tập Pilates
                đối với sức khỏe tim mạch.
              </p>
            </div>
          </div>
        </div>
        <div class="col-md-6 mb-4">
          <div class="card">
            <div class="card-header fw-bold">
              EAT CLEAN: Nên Và Không Nên Ăn Thực Phẩm Nào?
              <span><i class="bi bi-chat-left-fill"> 3</i></span>
            </div>
            <img src="./img/eat-clean.png" class="card-img-top" alt="..." />
            <div class="card-body">
              <p class="card-text">
                Chúng ta luôn chú trọng lựa chọn thực phẩm sạch và duy trì lối
                sống lành mạnh. Vậy chế độ ăn Eat clean nên và không nên ăn gì
                trong thực đơn hàng ngày để cân bằng tháp dinh dưỡng cho cơ thể?
              </p>
            </div>
          </div>
        </div>
      </div>

      <!-- Pagination -->
      <nav aria-label="Page navigation">
        <ul class="pagination justify-content-center">
          <li class="page-item">
            <a class="page-link" href="#" tabindex="-1">←</a>
          </li>
          <li class="page-item active"><a class="page-link" href="#">1</a></li>
          <li class="page-item"><a class="page-link" href="#">2</a></li>
          <li class="page-item"><a class="page-link" href="#">3</a></li>
          <li class="page-item">
            <a class="page-link" href="#">→</a>
          </li>
        </ul>
      </nav>
    </article>
  </section>
  <footer class="bg-dark text-white text-center py-3 mt-auto">
    <p class="mb-0">&copy;Copyright by FPT Polytechnic</p>
  </footer>
</template>

<script>
export default {
  name: "Lab3Bai2",
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
