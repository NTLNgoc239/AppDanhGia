<template>
  <div class="info-customer">
    <div class="image">
      <img src="../assets/istockphoto-922962354-612x612.jpg" />
    </div>
    <div class="name">
      <p>Trần Phối Dung</p>
    </div>
  </div>
</template>

<style scoped>
.info-customer {
  margin-top: 20px;
  margin-bottom: 20px;
  text-align: center;
}
img {
  border: 1px solid #2787f4;
  border-radius: 0;
  width: 100px;
  height: 150px;
}
.name {
  font-size: 28px;
  font-weight: bold;
  color: #292c2e;
  margin-top: 20px;
}
p {
  font-size: 25px;
}
@media (min-width: 992px) {
  img {
    border-radius: 0;
    width: 200px;
    height: 250px;
  }
  p {
    font-size: 20px;
    margin-top: 30px;
  }
}
/* Small devices (landscape phones, 576px and up) */
@media (min-width: 768px) {
  img {
    border-radius: 50%;
    width: 200px;
    height: 250px;
  }
  p {
    font-size: 40px;
    margin-top: 30px;
  }
  .name {
    margin-top: 20px;
  }
}

@media (min-width: 1200px) {
  img {
    border-radius: 0;
    width: 200px;
    height: 250px;
  }
  p {
    font-size: 40px;
    margin-top: 30px;
  }
  .name {
    margin-top: 20px;
  }
}
</style>

<script>
export default {
  name: "InfoCustomer",
  props: {
    name: String,
  },
};
</script>
