<template>
  <div class="container mt-3">
    <h3>Bài tập ứng dụng Modal cho Tài khoản</h3>
    <button
      type="button"
      class="btn btn-primary"
      data-bs-toggle="modal"
      data-bs-target="#myModal"
    >
      Tài khoản
    </button>
  </div>

  <div class="modal" id="myModal">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h4 class="modal-title">ĐĂNG NHẬP / ĐĂNG KÝ</h4>
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="modal"
          ></button>
        </div>
        <div class="modal-body">
          <div class="container mt-3">
            <!-- Tabs Điều Hướng -->
            <ul class="nav nav-tabs" role="tablist">
              <li class="nav-item">
                <a class="nav-link active" data-bs-toggle="tab" href="#register"
                  >Đăng ký</a
                >
              </li>
              <li class="nav-item">
                <a class="nav-link" data-bs-toggle="tab" href="#login"
                  >Đăng nhập</a
                >
              </li>
            </ul>

            <!-- Nội dung Tab -->
            <div class="tab-content mt-3">
              <!-- Tab Đăng ký -->
              <div id="register" class="container tab-pane active">
                <h3>Form Đăng ký</h3>
                <form>
                  <!-- Họ và tên -->
                  <div class="mb-3">
                    <label for="fullName" class="form-label">Họ và Tên</label>
                    <input
                      type="text"
                      class="form-control"
                      id="fullName"
                      placeholder="Nhập họ và tên"
                      required
                    />
                  </div>
                  <!-- Email -->
                  <div class="mb-3">
                    <label for="email" class="form-label">Email</label>
                    <input
                      type="email"
                      class="form-control"
                      id="email"
                      placeholder="Nhập email"
                      required
                    />
                  </div>
                  <!-- Số điện thoại -->
                  <div class="mb-3">
                    <label for="phone" class="form-label">Số điện thoại</label>
                    <input
                      type="tel"
                      class="form-control"
                      id="phone"
                      placeholder="Nhập số điện thoại"
                      required
                    />
                  </div>
                  <!-- Mật khẩu -->
                  <div class="mb-3">
                    <label for="password" class="form-label">Mật khẩu</label>
                    <input
                      type="password"
                      class="form-control"
                      id="password"
                      placeholder="Nhập mật khẩu"
                      required
                    />
                  </div>
                  <!-- Xác nhận mật khẩu -->
                  <div class="mb-3">
                    <label for="confirmPassword" class="form-label"
                      >Xác nhận mật khẩu</label
                    >
                    <input
                      type="password"
                      class="form-control"
                      id="confirmPassword"
                      placeholder="Nhập lại mật khẩu"
                      required
                    />
                  </div>
                  <!-- Giới tính -->
                  <div class="mb-3">
                    <label class="form-label">Giới tính</label>
                    <div>
                      <input
                        type="radio"
                        id="male"
                        name="gender"
                        value="male"
                        required
                      />
                      <label for="male">Nam</label>
                    </div>
                    <div>
                      <input
                        type="radio"
                        id="female"
                        name="gender"
                        value="female"
                        required
                      />
                      <label for="female">Nữ</label>
                    </div>
                  </div>
                  <!-- Ngôn ngữ -->
                  <div class="mb-3">
                    <label for="language" class="form-label">Ngôn ngữ</label>
                    <select class="form-select" id="language" required>
                      <option value="" selected disabled>Chọn ngôn ngữ</option>
                      <option value="vietnamese">Tiếng Việt</option>
                      <option value="english">Tiếng Anh</option>
                      <option value="japanese">Tiếng Nhật</option>
                    </select>
                  </div>
                  <!-- Đồng ý điều khoản -->
                  <div class="mb-3 form-check">
                    <input
                      type="checkbox"
                      class="form-check-input"
                      id="terms"
                      required
                    />
                    <label class="form-check-label" for="terms"
                      >Tôi đồng ý với các điều khoản và điều kiện trên</label
                    >
                  </div>
                  <!-- Nút đăng ký -->
                  <button type="submit" class="btn btn-primary">Đăng ký</button>
                </form>
              </div>

              <!-- Tab Đăng nhập -->
              <div id="login" class="container tab-pane fade">
                <h3>Form Đăng nhập</h3>
                <form>
                  <!-- Email -->
                  <div class="mb-3">
                    <label for="loginEmail" class="form-label">Email</label>
                    <input
                      type="email"
                      class="form-control"
                      id="loginEmail"
                      placeholder="Nhập email"
                      required
                    />
                  </div>
                  <!-- Mật khẩu -->
                  <div class="mb-3">
                    <label for="loginPassword" class="form-label"
                      >Mật khẩu</label
                    >
                    <input
                      type="password"
                      class="form-control"
                      id="loginPassword"
                      placeholder="Nhập mật khẩu"
                      required
                    />
                  </div>
                  <!-- Nút đăng nhập -->
                  <button type="submit" class="btn btn-primary w-100">
                    Đăng nhập
                  </button>
                </form>
              </div>
            </div>
          </div>

          <!-- Đoạn mà tạo Tab ở bài 3 dần ở đây -->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Lab2Bai4",
};
</script>

<style></style>
