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
        <h1 class="text-info text-center">
          Phương pháp tập Pilates giúp phục hồi chấn thương cột sống
        </h1>
        <img src="./img/tap-pilates1.jpg" alt="" width="100%" />
        <p>
          Tập Pilates có thể vẫn còn khá xa lạ với người Việt, nhưng tại các
          nước phương Tây thì đây chính là phương pháp tập thể dục giúp duy trì
          vóc dáng, tăng cường ý chí và cải thiện sự linh hoạt, dẻo dai cho
          người tập. Đặc biệt, các bài tập Pilates còn có khả năng trị đau lưng,
          là giải pháp hữu hiệu để phục hồi chấn thương cột sống. Sau đây hãy
          cùng tìm hiểu các phương pháp tập luyện này giúp phục hồi chấn thương
          cột sống nhanh chóng nhé!
        </p>

        <h4>Pilates giúp phục hồi chấn thương cột sống nhanh chóng</h4>
        <p>
          Một trong những căn bệnh ngày càng phổ biến, đặc biệt là dân văn
          phòng, đó là đau lưng, thoát vị đĩa đệm. Tuy nhiên, nếu điều trị không
          đúng cách có thể dẫn đến nhiều biến chứng nguy hiểm, bao gồm: Ví dụ,
          điều trị bằng laser không đúng cách hoặc tập yoga không đúng cách có
          thể khiến bệnh nhân nằm liệt giường.
        </p>
        <img src="./img/tap-piltes.jpg" alt="" width="100%" />
        <h4>Phương pháp tập Pilates Cat Cow</h4>
        <p>Các bước thực hiện:</p>
        <ul>
          <li>
            Bắt đầu với tư thế 4 điểm. Vai và cổ tay của bạn phải thẳng hàng và
            vuông góc với thảm, lưng của bạn phải bằng phẳng và xương chậu của
            bạn phải cân đối. Hít vào, võng lưng, nâng cằm lên, mở rộng ngực.
            Thở ra, cong xương cụt, nâng cong lưng và đưa cằm về gần khoảng
            ngực. Lặp đi lặp lại động tác từ 5-7 lần.
          </li>
          <li>Hít vào, võng lưng, nâng cằm lên, mở rộng ngực</li>
          <li>
            Thở ra, cong xương cụt, nâng cong lưng và đưa cằm về gần khoang ngực
          </li>
          <li>Lặp đi lặp lại động tác từ 5-7 lần.</li>
        </ul>
        <h4>Lời kết</h4>
        <p>
          Trên đây là phương pháp tập Pilates giúp phục hồi chấn thương cột sống
          nhanh chóng. Để đạt được kết quả tập luyện như mong muốn, bạn cần duy
          trì chế độ tập luyện đều đặn, thực hiện đúng động tác, kết hợp cùng
          chế độ ăn uống khoa học.
        </p>
      </article>
      <aside class="col-4">
        <h3>Bình luận bài viết tại đây</h3>
        <textarea
          placeholder="Nhập bình luận của bạn"
          rows="2"
          cols="50"
        ></textarea>
        <button class="bg-success text-white rounded-2 p-2">
          Gửi bình luận
        </button>
        <h3>Danh sách các bình luận:</h3>
        <ul>
          <li><strong>Bình An: </strong>Bài viết rất hữu ích</li>
          <li><strong>Bình An: </strong>Cảm ơn những chia sẻ bổ ích</li>
        </ul>
      </aside>
    </div>
  </div>

  <footer class="bg-dark text-white text-center py-3 mt-auto">
    <p class="mb-0">&copy;Copyright by FPT Polytechnic</p>
  </footer>
</template>

<script>
export default {
  name: "Lab3Bai3",
};
</script>

<style></style>
