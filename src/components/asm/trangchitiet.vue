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

  <div class="container">
    <div class="row p-2">
      <article class="col-8">
        <!-- Nội dung bài viết sẽ ở đây -->
      </article>
      <aside class="col-4">
        <h3>Bình luận bài viết tại đây</h3>
        <textarea
          v-model="commentText"
          placeholder="Nhập bình luận của bạn"
          rows="4"
          cols="50"
        ></textarea>
        <button @click="submitComment" class="btn btn-primary mt-2">
          Đăng bình luận
        </button>
      </aside>
    </div>
  </div>

  <footer class="bg-dark text-white text-center py-3 mt-auto">
    <p class="mb-0">&copy;Copyright by FPT Polytechnic</p>
  </footer>
</template>

<script>
export default {
  name: "ASMBai5",
  data() {
    return {
      commentText: "", // Biến lưu trữ nội dung bình luận
    };
  },
  methods: {
    submitComment() {
      if (this.commentText.trim()) {
        alert("Bình luận của bạn: " + this.commentText);
        // Thêm code xử lý gửi bình luận vào hệ thống ở đây (ví dụ: API request)
        this.commentText = ""; // Reset lại nội dung bình luận sau khi gửi
      } else {
        alert("Vui lòng nhập bình luận.");
      }
    },
  },
};
</script>

<style scope></style>
