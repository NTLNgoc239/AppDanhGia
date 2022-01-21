<template>
  <div class="thankyou3">
    <div class="icon">
      <img src="../assets/susscess.svg" />
    </div>
    <div class="text"></div>
    <pre>
  Chân thành cảm ơn Quý khách
  Những lời khen của Quý khách là nguồn động viên tinh 
  thần to lớn giúp Nhân viên nói riêng và
  bộ phận CSKH Vietmap nói chung phụ vụ Quý khách
  hàng ngày một tốt hơn
  Chúc Quý khách một ngày vui vẻ
    </pre>
    <p class="text-3">TRÂN TRỌNG !</p>
    <router-link to="/">
      <b-button type="submit" class="btn btn-primary changescreen">
        <i class="fas fa-arrow-left"></i>QUAY VỀ MÀN HÌNH CHÍNH</b-button
      ></router-link
    >
    <router-view />
  </div>
</template>

<style scoped>
.thankyou3 {
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
  font-weight: bold;
}
button {
  background-color: #01a3e0;
  font-size: 24px;
  font-weight: bold;
  color: #ffffff;
  border: 1px solid #01a3e0;
  border-radius: 8px;
  width: 70%;
}
@media (max-width: 576px) {
  .text {
    font-size: 16px;
  }
  button {
    font-size: 10px;
  }
}
</style>
