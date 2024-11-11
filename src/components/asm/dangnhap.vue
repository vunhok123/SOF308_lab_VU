<template>
  <section class="vh-100 login-section">
    <div class="container-fluid">
      <div class="row justify-content-center align-items-center h-100">
        <div class="col-md-6 col-lg-4 text-black login-form-column">
          <div class="text-center logo mb-4">
            <i class="fas fa-crow fa-2x me-3" style="color: #ffffff"></i>
            <span class="h1 fw-bold mb-0 text-white">Logo</span>
          </div>

          <div class="px-5">
            <form>
              <h3 class="fw-normal mb-3 pb-3 title text-center">Log in</h3>

              <div class="form-outline mb-4">
                <input
                  type="email"
                  id="emailInput"
                  class="form-control form-control-lg"
                  placeholder="Enter your email"
                  required
                />
                <label class="form-label" for="emailInput">Email address</label>
              </div>

              <div class="form-outline mb-4">
                <input
                  type="password"
                  id="passwordInput"
                  class="form-control form-control-lg"
                  placeholder="Enter your password"
                  required
                />
                <label class="form-label" for="passwordInput">Password</label>
              </div>

              <div class="pt-1 mb-4">
                <button class="btn btn-custom btn-lg btn-block" type="submit">
                  Login
                </button>
              </div>

              <p class="small mb-5 pb-lg-2 text-center">
                <a class="text-muted" href="#!">Forgot password?</a>
              </p>
              <p class="text-center">
                Don't have an account?
                <a href="#!" class="link-custom">Register here</a>
              </p>
            </form>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ASMBai2",
};
</script>

<style scoped>
/* Background without blur effect */
.login-section {
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  z-index: 1;
  background-image: url("img/austin-chan-ukzHlkoz1IE-unsplash.jpg"); /* Replace with your image URL */
  background-size: cover;
  background-position: center;
  height: 100vh;
}

/* Form column with a soft shadow and a transparent background */
.login-form-column {
  padding-top: 5%;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
  background-color: rgba(255, 255, 255, 0.9); /* Semi-transparent background */
  backdrop-filter: blur(10px); /* Apply backdrop blur effect */
  padding: 30px;
  transition: all 0.3s ease-in-out;
}

/* Hover effect on form column */
.login-form-column:hover {
  transform: scale(1.02);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
}

/* Logo styling */
.logo {
  color: #ffffff;
}

.title {
  letter-spacing: 1px;
  color: #333;
  font-size: 2.2rem;
  font-weight: bold;
  transition: color 0.3s ease;
}

.title:hover {
  color: #2575fc;
}

/* Input styling with focus effect */
.form-control {
  background-color: #f9f9f9;
  border: none;
  border-radius: 8px;
  padding: 12px;
  transition: all 0.3s ease;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.form-control:focus {
  background-color: #fff;
  box-shadow: 0px 0px 8px rgba(0, 123, 255, 0.3);
  outline: none;
  border: 1px solid #2575fc;
}

.form-control::placeholder {
  color: #aaa;
}

/* Button hover effect */
.btn-custom {
  background: linear-gradient(135deg, #6a11cb, #2575fc);
  border: none;
  border-radius: 8px;
  font-size: 1.1rem;
  transition: all 0.3s ease;
  color: white;
  padding: 12px 20px;
  width: 100%;
}

.btn-custom:hover {
  background: linear-gradient(135deg, #2575fc, #6a11cb);
  box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.2);
  transform: scale(1.05);
}

/* Link hover effect */
.link-custom {
  color: #2575fc;
  font-weight: bold;
  text-decoration: none;
}

.link-custom:hover {
  color: #6a11cb;
  text-decoration: underline;
}

/* Animation for input fields on focus */
@keyframes shake {
  0% {
    transform: translateX(0);
  }
  25% {
    transform: translateX(-5px);
  }
  50% {
    transform: translateX(5px);
  }
  75% {
    transform: translateX(-5px);
  }
  100% {
    transform: translateX(0);
  }
}

.form-control:invalid {
  border: 1px solid red;
  animation: shake 0.5s ease;
}
</style>
