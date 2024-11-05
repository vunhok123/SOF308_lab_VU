<template>
  <div class="container mt-5">
    <h3 class="text-center">Bảng Thành phần dinh dưỡng</h3>
    <table class="table table-bordered">
      <thead class="table-light">
        <tr>
          <th
            rowspan="2"
            class="text-center align-middle"
            style="background-color: yellow"
          >
            Thành phần
          </th>
          <th colspan="2" class="text-center" style="background-color: yellow">
            Giá trị
          </th>
        </tr>
        <tr>
          <th class="text-center" style="background-color: yellow">
            Khối lượng
          </th>
          <th class="text-center" style="background-color: yellow">% DV*</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Calories</td>
          <td class="text-center">200 kcal</td>
          <td class="text-center">20%</td>
        </tr>
        <tr>
          <td>Chất béo</td>
          <td class="text-center">9g</td>
          <td class="text-center">14%</td>
        </tr>
        <tr>
          <td>Chất béo bão hoã</td>
          <td class="text-center">4 g</td>
          <td class="text-center">20%</td>
        </tr>
        <tr>
          <td>Chất đạm</td>
          <td class="text-center">8 mg</td>
          <td class="text-center">16%</td>
        </tr>
        <tr>
          <td>Chất xơ</td>
          <td class="text-center">5 mg</td>
          <td class="text-center">20%</td>
        </tr>
        <tr>
          <td>Đường</td>
          <td class="text-center">12 g</td>
          <td class="text-center">-</td>
        </tr>
        <tr>
          <td rowspan="2">Vitamin</td>
          <td class="text-center">vitamin C</td>
          <td class="text-center">25%</td>
        </tr>
        <tr>
          <td class="text-center">vitamin D</td>
          <td class="text-center">10%</td>
        </tr>
      </tbody>
    </table>
    <p class="text-muted">
      * DV: Daily Value (Giá trị hàng ngày được khuyến nghị)
    </p>
  </div>
</template>

<script>
export default {
  name: "Lab2Bai1",
};
</script>

<style scoped>
.table {
  width: 100%;
  margin-top: 20px;
}

.text-center {
  text-align: center;
}

.text-muted {
  font-size: 0.875rem;
  margin-top: 10px;
}
</style>
