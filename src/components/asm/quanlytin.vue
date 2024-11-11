<template>
  <div id="app" class="container py-5">
    <h1 class="mb-4 text-center">Đăng Bài Viết</h1>

    <!-- Form Đăng Bài -->
    <form @submit.prevent="addOrUpdatePost" class="animated-form">
      <div class="mb-4">
        <label for="title" class="form-label">Tiêu đề bài viết:</label>
        <input
          type="text"
          id="title"
          v-model="newTitle"
          class="form-control form-control-lg shadow-sm"
          placeholder="Nhập tiêu đề bài viết"
          required
        />
      </div>

      <div class="mb-4">
        <label for="content" class="form-label">Nội dung bài viết:</label>
        <textarea
          id="content"
          v-model="newContent"
          class="form-control form-control-lg shadow-sm"
          placeholder="Nhập nội dung bài viết"
          rows="5"
          required
        ></textarea>
      </div>

      <div class="mb-4">
        <label for="image" class="form-label">Chọn hình ảnh minh họa:</label>
        <input
          type="file"
          id="image"
          class="form-control form-control-lg shadow-sm"
          @change="handleImageUpload"
          accept="image/*"
        />
        <div v-if="imagePreview" class="mt-3">
          <h5>Ảnh minh họa:</h5>
          <img
            :src="imagePreview"
            alt="Preview Image"
            class="img-fluid rounded shadow-lg"
            style="max-height: 300px"
          />
        </div>
      </div>

      <button type="submit" class="btn custom-btn shadow-sm">
        {{ isEdit ? "Cập nhật bài viết" : "Đăng bài viết" }}
      </button>
    </form>

    <hr class="my-5" />

    <!-- Danh sách bài viết đã đăng -->
    <h2 class="mb-4 text-center">Danh sách bài viết của bạn:</h2>
    <div class="row">
      <div v-for="(post, index) in posts" :key="post.id" class="col-md-4 mb-5">
        <div class="card custom-card shadow-lg">
          <img
            v-if="post.image"
            :src="post.image"
            alt="Post Image"
            class="card-img-top custom-card-img rounded-top"
          />
          <div class="card-body custom-card-body">
            <h5 class="card-title">{{ post.title }}</h5>
            <p class="card-text">{{ post.content }}</p>
            <div class="btn-group w-100">
              <button @click="editPost(index)" class="btn custom-edit-btn">
                Sửa
              </button>
              <button @click="deletePost(index)" class="btn custom-delete-btn">
                Xóa
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// Import Toast từ Vue Toastification

export default {
  name: "ASMBai4",
  data() {
    return {
      newTitle: "",
      newContent: "",
      imagePreview: "",
      posts: [
        {
          id: 1,
          title: "Bài viết mẫu 1",
          content:
            "Đây là nội dung bài viết mẫu 1. Bạn có thể chỉnh sửa bài viết này.",
          image: "https://via.placeholder.com/300x200",
        },
        {
          id: 2,
          title: "Bài viết mẫu 2",
          content:
            "Đây là nội dung bài viết mẫu 2. Nội dung có thể được thay đổi theo yêu cầu.",
          image: "https://via.placeholder.com/300x200",
        },
      ],
      isEdit: false,
      editIndex: null,
    };
  },
  methods: {
    addOrUpdatePost() {
      if (this.isEdit) {
        this.posts[this.editIndex] = {
          title: this.newTitle,
          content: this.newContent,
          image: this.imagePreview,
        };
        this.isEdit = false;
        this.toast.success("Bài viết đã được cập nhật thành công!");
      } else {
        this.posts.push({
          id: this.posts.length + 1,
          title: this.newTitle,
          content: this.newContent,
          image: this.imagePreview,
        });
        this.toast.success("Bài viết đã được đăng thành công!");
      }
      this.resetForm();
    },
    handleImageUpload(event) {
      const file = event.target.files[0];
      if (file) {
        const reader = new FileReader();
        reader.onload = (e) => {
          this.imagePreview = e.target.result;
        };
        reader.readAsDataURL(file);
      }
    },
    editPost(index) {
      const post = this.posts[index];
      this.newTitle = post.title;
      this.newContent = post.content;
      this.imagePreview = post.image;
      this.isEdit = true;
      this.editIndex = index;
    },
    deletePost(index) {
      this.posts.splice(index, 1);
      this.toast.info("Bài viết đã được xóa.");
    },
    resetForm() {
      this.newTitle = "";
      this.newContent = "";
      this.imagePreview = "";
    },
  },
};
</script>

<style scoped>
/* Custom styles for buttons and inputs */
.custom-btn {
  background-color: #28a745;
  color: white;
  border: none;
  padding: 12px 24px;
  font-size: 18px;
  border-radius: 8px;
  transition: background-color 0.3s, transform 0.2s ease-in-out;
}

.custom-btn:hover {
  background-color: #218838;
  transform: translateY(-2px); /* Đẩy nút lên khi hover */
}

.custom-edit-btn {
  background-color: #ffc107;
  color: white;
  border: none;
  padding: 10px 20px;
  font-size: 16px;
  border-radius: 8px;
  transition: background-color 0.3s, transform 0.2s ease-in-out;
}

.custom-edit-btn:hover {
  background-color: #e0a800;
  transform: translateY(-2px);
}

.custom-delete-btn {
  background-color: #dc3545;
  color: white;
  border: none;
  padding: 10px 20px;
  font-size: 16px;
  border-radius: 8px;
  transition: background-color 0.3s, transform 0.2s ease-in-out;
}

.custom-delete-btn:hover {
  background-color: #c82333;
  transform: translateY(-2px);
}

.form-control:focus {
  border-color: #80bdff;
  box-shadow: 0 0 8px rgba(0, 123, 255, 0.5);
}

.custom-card-img:hover {
  transform: scale(1.05);
}

.custom-card {
  border-radius: 10px;
  transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
}

.custom-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
}
</style>
