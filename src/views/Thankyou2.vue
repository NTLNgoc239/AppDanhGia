<template>
  <div class="thankyou2">
    <div class="icon">
      <img src="../assets/susscess.svg" />
    </div>
    <div class="text">
      <p>
        Chân thành cảm ơn những ý kiến góp ý của Quý khách Vietmap xin ghi nhận
        để cải thiện chất lượng dịch vụ, phục vụ khách hàng tốt hơn trong thời
        gian tới
      </p>
      <!-- <p class="text-2">
        Vietmap xin ghi nhận để cải thiện chất lượng dịch vụ,
      </p>
      <p class="text-2"></p> -->
      <p>Chúc Quý khách một ngày vui vẻ</p>
      <p class="text-3">TRÂN TRỌNG !</p>
    </div>
    <router-link to="/">
      <b-button type="submit" class="btn btn-primary changescreen">
        <i class="fas fa-arrow-left"></i>QUAY VỀ MÀN HÌNH CHÍNH</b-button
      ></router-link
    >
    <router-view />
  </div>
</template>

<style scoped>
.thankyou2 {
  background: url("../assets/thankyoubackgrounf.svg");
  text-align: center;
  margin-top: 150px;
}
img {
  width: 160px;
  height: 160px;
  margin-bottom: 32px;
}
.text {
  font-size: 20px;
  color: #292c2e;
  line-height: 30px;
}
.text-3 {
  font-size: 24px;
  line-height: 48px;
  color: #00aeef;
  margin-bottom: 80px;
}
button {
  background-color: #01a3e0;
  font-size: 24px;
  font-weight: bold;
  color: #ffffff;
  border: 1px solid #01a3e0;
  border-radius: 8px;
  width: 50%;
}

@media (max-width: 576px) {
  .text {
    font-size: 16px;
  }
}
</style>
