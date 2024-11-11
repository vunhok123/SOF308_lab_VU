<template>
  <!-- Navbar: Navigation Bar -->
  <nav class="navbar navbar-expand-lg bg-body-tertiary">
    <div class="container-fluid">
      <!-- Logo -->
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

  <!-- Section: Design Block -->
  <section class="background-image-section overflow-hidden">
    <div class="container px-4 py-5 px-md-5 text-center text-lg-start my-5">
      <div class="row gx-lg-5 align-items-center mb-5">
        <!-- Left side: Form (Now on the left side) -->
        <div class="col-lg-6 mb-5 mb-lg-0 position-relative">
          <div
            id="radius-shape-1"
            class="position-absolute rounded-circle shadow-5-strong"
          ></div>
          <div
            id="radius-shape-2"
            class="position-absolute shadow-5-strong"
          ></div>

          <div class="card bg-solid">
            <div class="card-body px-4 py-5 px-md-5">
              <!-- Title: "Đăng ký" with improved contrast -->
              <h2 class="text-center mb-4 title">Đăng ký</h2>

              <form>
                <!-- Name fields -->
                <div class="row">
                  <div class="col-md-6 mb-4">
                    <div data-mdb-input-init class="form-outline">
                      <input
                        type="text"
                        id="form3Example1"
                        class="form-control"
                      />
                      <label class="form-label" for="form3Example1"
                        >First name</label
                      >
                    </div>
                  </div>
                  <div class="col-md-6 mb-4">
                    <div data-mdb-input-init class="form-outline">
                      <input
                        type="text"
                        id="form3Example2"
                        class="form-control"
                      />
                      <label class="form-label" for="form3Example2"
                        >Last name</label
                      >
                    </div>
                  </div>
                </div>

                <!-- Email input -->
                <div data-mdb-input-init class="form-outline mb-4">
                  <input type="email" id="form3Example3" class="form-control" />
                  <label class="form-label" for="form3Example3"
                    >Email address</label
                  >
                </div>

                <!-- Password input -->
                <div data-mdb-input-init class="form-outline mb-4">
                  <input
                    type="password"
                    id="form3Example4"
                    class="form-control"
                  />
                  <label class="form-label" for="form3Example4">Password</label>
                </div>

                <!-- Checkbox for subscription -->
                <div class="form-check d-flex justify-content-center mb-4">
                  <input
                    class="form-check-input me-2"
                    type="checkbox"
                    value=""
                    id="form2Example33"
                    checked
                  />
                  <label class="form-check-label" for="form2Example33"
                    >Subscribe to our newsletter</label
                  >
                </div>

                <!-- Submit button -->
                <div class="d-flex justify-content-center">
                  <button
                    type="submit"
                    data-mdb-button-init
                    data-mdb-ripple-init
                    class="btn btn-primary btn-block mb-4"
                  >
                    Sign up
                  </button>
                </div>

                <!-- Social login options -->
                <div class="text-center">
                  <p class="text-dark">or sign up with:</p>
                  <div class="d-flex justify-content-center">
                    <button
                      type="button"
                      data-mdb-button-init
                      data-mdb-ripple-init
                      class="btn btn-link btn-floating mx-1"
                    >
                      <i class="fab fa-facebook-f"></i>
                    </button>

                    <button
                      type="button"
                      data-mdb-button-init
                      data-mdb-ripple-init
                      class="btn btn-link btn-floating mx-1"
                    >
                      <i class="fab fa-google"></i>
                    </button>

                    <button
                      type="button"
                      data-mdb-button-init
                      data-mdb-ripple-init
                      class="btn btn-link btn-floating mx-1"
                    >
                      <i class="fab fa-twitter"></i>
                    </button>

                    <button
                      type="button"
                      data-mdb-button-init
                      data-mdb-ripple-init
                      class="btn btn-link btn-floating mx-1"
                    >
                      <i class="fab fa-github"></i>
                    </button>
                  </div>
                </div>
              </form>
            </div>
          </div>
        </div>

        <!-- Right side content (Now on the right side) -->
        <div class="col-lg-6 mb-5 mb-lg-0" style="z-index: 10">
          <h1 class="my-5 display-5 fw-bold ls-tight title-left">
            A blog is a journal that is publicly shared, but its power lies in
            the ability to create connections. <br />
            <span style="color: rgba(255, 255, 255, 0.7)"
              >for your business</span
            >
          </h1>
          <p class="mb-4 opacity-70 text-white">
            Một blog là một cuốn nhật ký được chia sẻ công khai, nhưng sức mạnh
            của nó nằm ở khả năng tạo ra những kết nối.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ASMBai3",
};
</script>

<style scoped>
/* Navbar Styling */
.navbar {
  z-index: 100;
}

/* Section background with image */
.background-image-section {
  background-image: url("img/austin-chan-ukzHlkoz1IE-unsplash.jpg");
  background-size: cover;
  background-position: center center;
  background-attachment: fixed;
  padding: 100px 0;
  color: white; /* Ensures text is white */
  position: relative;
  overflow: hidden;
}

/* Add a dark overlay and blur effect on the background image */
.background-image-section::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: inherit;
  filter: blur(8px); /* Apply blur effect */
  background: rgba(0, 0, 0, 0.5); /* Dark overlay with 50% opacity */
  z-index: -1; /* Make sure the overlay and blur effect are behind the content */
}

/* Solid card background */
.bg-solid {
  background-color: rgba(
    255,
    255,
    255,
    0.9
  ); /* Solid white background with opacity */
  border-radius: 10px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease;
}

/* Hover effect on card */
.bg-solid:hover {
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.2);
  transform: scale(1.02);
}

/* Button custom styles */
.btn-primary {
  background-color: #2575fc;
  border-color: #2575fc;
}

.btn-primary:hover {
  background-color: #6a11cb;
  border-color: #6a11cb;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

/* Input fields */
.form-outline input {
  border-radius: 8px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

.form-outline label {
  color: #333; /* Dark color for labels */
}

/* Icon button styles */
.btn-link {
  color: #2575fc;
}

.btn-link:hover {
  color: #6a11cb;
}

.form-check-label {
  font-size: 0.9rem;
  color: #333; /* Ensure checkbox label is readable */
}

/* Title styling: Đăng ký */
.title {
  color: #333; /* Dark color for the title */
  font-weight: bold;
}

/* Title on the right side */
.title-left {
  color: #fff; /* White color for right-side text */
}

/* Paragraph text on the right side */
.text-white {
  color: #fff; /* White color for text */
}

/* Responsiveness */
@media (max-width: 767px) {
  .container {
    padding: 10px;
  }
  .row {
    flex-direction: column;
  }
}
</style>
