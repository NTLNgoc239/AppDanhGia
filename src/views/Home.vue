<template>
  <!-- <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div> -->
  <div id="break">
    <div class="home" id="session1">
      <div class="content">
        <div class="text">
          <p class="text-1">Chào mừng Quý khách đến với</p>
          <a class="text-show">SHOWROOM VIETMAP</a>
          <pre class="text-home">
  Với mong muốn hỗ trợ khách hàng ngày một tốt hơn,
  Vietmap trân trọng kính mời Quý khách đánh giá chất lượng hỗ trợ
  của nhân viên Showroom
          </pre>
          <!-- <p class="text-2">
            
          </p>
          <p class="text-2"></p> -->
        </div>
        <div id="info">
          <info-customer></info-customer>
          <div class="text">
            <pre class="text-home">
  Với những trải nghiệm thực tế tại Showroom hôm nay,
  Quý khách vui lòng chia sẻ mức độ hài lòng về
  chất lượng hỗ trợ của nhân viên tư vấn
            </pre>
            <!-- <p class="text-2"></p>
            <p class="text-2"></p> -->
          </div>
        </div>
        <div class="rating">
          <ul>
            <button
              v-b-modal.modal-center1
              type="button"
              variant="outline-dark"
            >
              <div class="image">
                <img src="../assets/button1.svg" />
              </div>
              <div>
                <a class="text-3">Rất không hài lòng</a>
              </div>
            </button>
            <button
              v-b-modal.modal-center1
              type="button"
              variant="outline-dark"
            >
              <div class="image">
                <img src="../assets/button2.svg" />
              </div>
              <div>
                <a class="text-3">Không hài lòng</a>
              </div>
            </button>
            <button
              v-b-modal.modal-center3
              type="button"
              variant="outline-dark"
            >
              <div class="image">
                <img src="../assets/button3.svg" />
              </div>
              <div>
                <a class="text-3">Bình thường</a>
              </div>
            </button>
            <button v-b-modal.modal-center type="button" variant="outline-dark">
              <div class="image">
                <img src="../assets/button4.svg" />
              </div>
              <div>
                <a class="text-3">Hài lòng</a>
              </div>
            </button>
            <button v-b-modal.modal-center type="button" variant="outline-dark">
              <div class="image">
                <img src="../assets/button5.svg" />
              </div>
              <div>
                <a class="text-3">Rất hài lòng</a>
              </div>
            </button>
          </ul>
        </div>

        <!-- Popup1 -->
        <div>
          <b-modal id="modal-center1" hide-footer="true">
            <div class="modal-center___BV_modal_body_" style="padding: 2rem">
              <div class="image-popup">
                <img src="../assets/button6.svg" />
              </div>
              <div class="text-comment">
                <p class="text-4">
                  Vietmap xin lỗi vì nhân viên Vietmap chưa làm Quý khách hài
                  lòng
                </p>
                <!-- <p class="text-4"></p> -->
              </div>
              <div class="text-popup">
                <p>
                  Quý khách vui lòng chia sẻ những điều không hài lòng để
                  Vietmap cải thiện chất lượng hoặc để lại số điện thoại, Quản
                  lý bộ phận CSKH Vietmap sẽ liên hệ lại để hỗ trợ Quý khách tốt
                  hơn cũng như để nâng cao chất lượng phục vụ khách hàng tại
                  Showroom
                </p>
                <!-- <p class="text-2">
                  
                </p>
                <p class="text-2">
                  
                </p>
                <p class="text-2">
                  
                </p>
                <p class="text-2"></p> -->
              </div>
              <b-form>
                <b-form-group
                  label="Số điện thoại (không bắt buộc)"
                  label-for="phone-input"
                  style="
                    font-weight: bold;
                    font-size: 12px;
                    margin-bottom: 20px;
                  "
                >
                  <b-form-input
                    id="phone-input"
                    placeholder="Nhập số điện thoại của Quý khách"
                  ></b-form-input>
                </b-form-group>
                <b-form-group
                  label="Góp ý"
                  label-for="comment-input"
                  style="
                    font-weight: bold;
                    font-size: 12px;
                    margin-bottom: 20px;
                  "
                >
                  <textarea
                    id="comment-input"
                    placeholder="Ghi góp ý của Quý khách vào đây"
                  ></textarea>
                </b-form-group>
                <router-link to="/thankyou1"
                  ><button
                    id="thankyou1"
                    type="submit"
                    class="btn btn-primary sendcomment"
                    @click="redirectToThankyou1()"
                  >
                    GỬI ĐÁNH GIÁ
                  </button></router-link
                >
              </b-form>
            </div>
          </b-modal>
        </div>

        <!-- Popup3 -->
        <b-modal id="modal-center3" hide-footer="true">
          <div class="modal-center___BV_modal_body_" style="padding: 2rem">
            <div class="image-popup">
              <img src="../assets/button7.svg" />
            </div>
            <div class="text-comment">
              <p>
                Vietmap rất tiếc vì nhân viên Showroom chưa đáp ứng được mong
                đợi của Quý khách
              </p>
              <!-- <p class="text-4">Vietmap rất tiếc vì nhân viên Showroom</p>
              <p class="text-4">chưa đáp ứng được mong đợi của Quý khách</p> -->
            </div>
            <div class="text-popup">
              <p>
                Quý khách vui lòng góp ý những điểm nhân viên Vietmap cần cải
                thiện để Quý khách hài lòng hơn
              </p>
              <!-- <p class="text-2">
                Quý khách vui lòng góp ý những điểm nhân viên
              </p>
              <p class="text-2">
                Trần Phối Dung cần cải thiện để Quý khách hài lòng hơn
              </p> -->
            </div>
            <form>
              <b-form-group
                label="Số điện thoại (không bắt buộc)"
                label-for="phone-input"
                style="font-weight: bold; font-size: 12px; margin-bottom: 20px"
              >
                <b-form-input
                  id="phone-input"
                  placeholder="Nhập số điện thoại của Quý khách"
                ></b-form-input>
              </b-form-group>
              <b-form-group
                label="Góp ý"
                label-for="comment-input"
                style="font-weight: bold; font-size: 12px; margin-bottom: 20px"
              >
                <textarea
                  id="comment-input"
                  placeholder="Ghi góp ý của Quý khách vào đây"
                ></textarea>
              </b-form-group>
              <router-link to="/thankyou2">
                <b-button type="submit" class="btn btn-primary sendcomment"
                  >GỬI ĐÁNH GIÁ</b-button
                ></router-link
              >
            </form>
          </div>
        </b-modal>
        <!-- Popup45 -->
        <b-modal id="modal-center" hide-footer="true">
          <div class="modal-center___BV_modal_body_" style="padding: 2rem">
            <div class="image-popup">
              <img src="../assets/button8.svg" />
            </div>
            <div class="text-comment">
              <p>Quý khách vui lòng cho Vietmap xin số điện thoại</p>
            </div>
            <form>
              <b-form-group
                label="Số điện thoại (không bắt buộc)"
                label-for="phone-input"
                style="font-weight: bold; font-size: 12px; margin-bottom: 20px"
              >
                <b-form-input
                  id="phone-input"
                  placeholder="Nhập số điện thoại của Quý khách"
                ></b-form-input>
              </b-form-group>
              <router-link to="/thankyou3">
                <b-button type="submit" class="btn btn-primary sendcomment"
                  >GỬI ĐÁNH GIÁ</b-button
                ></router-link
              >
            </form>
          </div>
        </b-modal>
      </div>
      <router-view />
    </div>
    <div class="home" id="session2">
      <b-row>
        <div class="text">
          <p class="text-1">Chào mừng Quý khách đến với</p>
          <div class="text-show">
            <a>SHOWROOM VIETMAP</a>
          </div>
          <p class="text-2">
            Với mong muốn hỗ trợ khách hàng ngày một tốt hơn,
          </p>
          <p class="text-2">
            Vietmap trân trọng kính mời Quý khách đánh giá chất lượng hỗ trợ
          </p>
          <p class="text-2">của nhân viên Showroom</p>
        </div>
        <b-col sm="6">
          <info-customer></info-customer>
          <div id="info">
            <div class="text">
              <p class="text-2">
                Với những trải nghiệm thực tế tại Showroom hôm nay,
              </p>
              <p class="text-2">
                Quý khách vui lòng chia sẻ mức độ hài lòng về
              </p>
              <p class="text-2">chất lượng hỗ trợ của nhân viên tư vấn</p>
            </div>
          </div>
        </b-col>
        <b-col sm="6">
          <div class="rating">
            <ul>
              <button
                v-b-modal.modal-center4
                type="button"
                variant="outline-dark"
              >
                <div class="image">
                  <img src="../assets/button1.svg" />
                </div>
                <div>
                  <a class="text-3">Rất không hài lòng</a>
                </div>
              </button>
              <button
                v-b-modal.modal-center4
                type="button"
                variant="outline-dark"
              >
                <div class="image">
                  <img src="../assets/button2.svg" />
                </div>
                <div>
                  <a class="text-3">Không hài lòng</a>
                </div>
              </button>
              <button
                v-b-modal.modal-center5
                type="button"
                variant="outline-dark"
              >
                <div class="image">
                  <img src="../assets/button3.svg" />
                </div>
                <div>
                  <a class="text-3">Bình thường</a>
                </div>
              </button>
              <button
                v-b-modal.modal-center6
                type="button"
                variant="outline-dark"
              >
                <div class="image">
                  <img src="../assets/button4.svg" />
                </div>
                <div>
                  <a class="text-3">Hài lòng</a>
                </div>
              </button>
              <button
                v-b-modal.modal-center6
                type="button"
                variant="outline-dark"
              >
                <div class="image">
                  <img src="../assets/button5.svg" />
                </div>
                <div>
                  <a class="text-3">Rất hài lòng</a>
                </div>
              </button>
            </ul>
          </div>
          <!-- Popup1 -->
          <div>
            <b-modal id="modal-center4" hide-footer="true">
              <div class="modal-center___BV_modal_body_">
                <div class="image-popup">
                  <img src="../assets/button6.svg" />
                </div>
                <div class="text-comment">
                  <p>
                    Vietmap xin lỗi vì nhân viên Vietmap chưa làm Quý khách hài
                    lòng
                  </p>
                  <!-- <p></p> -->
                </div>
                <b-row>
                  <b-col sm="6">
                    <div class="text-popup">
                      <p>
                        Quý khách vui lòng chia sẻ những điều không hài lòng để
                        Vietmap cải thiện chất lượng hoặc để lại số điện thoại,
                        Quản lý bộ phận CSKH Vietmap sẽ liên hệ lại để hỗ trợ
                        Quý khách tốt hơn cũng như để nâng cao chất lượng phục
                        vụ khách hàng tại Showroom
                      </p>
                      <!-- <p>
                        Quý khách vui lòng chia sẻ những điều không hài lòng
                      </p>
                      <p>
                        Vietmap cải thiện chất lượng hoặc để lại số điện thoại,
                      </p>
                      <p>
                        Quản lý bộ phận CSKH Vietmap sẽ liên hệ lại để hỗ trợ
                        Quý
                      </p>
                      <p>
                        khách tốt hơn cũng như để nâng cao chất lượng phục vụ
                      </p>
                      <p>khách hàng tại Showroom</p> -->
                    </div>
                  </b-col>

                  <b-col sm="6">
                    <b-form>
                      <b-form-group
                        label="Số điện thoại (không bắt buộc)"
                        label-for="phone-input"
                        style="
                          font-weight: bold;
                          font-size: 12px;
                          margin-bottom: 20px;
                        "
                      >
                        <b-form-input
                          id="phone-input"
                          placeholder="Nhập số điện thoại của Quý khách"
                        ></b-form-input>
                      </b-form-group>
                      <b-form-group
                        label="Góp ý"
                        label-for="comment-input"
                        style="
                          font-weight: bold;
                          font-size: 12px;
                          margin-bottom: 20px;
                        "
                      >
                        <textarea
                          id="comment-input"
                          placeholder="Ghi góp ý của Quý khách vào đây"
                        ></textarea>
                      </b-form-group>
                    </b-form>
                  </b-col>
                  <router-link to="/thankyou1"
                    ><button
                      id="thankyou1"
                      type="submit"
                      class="btn btn-primary sendcomment"
                      @click="redirectToThankyou1()"
                    >
                      GỬI ĐÁNH GIÁ
                    </button></router-link
                  >
                </b-row>
              </div>
            </b-modal>
          </div>

          <!-- Popup3 -->
          <b-modal id="modal-center5" hide-footer="true">
            <div class="modal-center___BV_modal_body_">
              <div class="image-popup">
                <img src="../assets/button7.svg" />
              </div>
              <div class="text-comment">
                <p>
                  Vietmap rất tiếc vì nhân viên Showroom chưa đáp ứng được mong
                  đợi của Quý khách
                </p>
                <!-- <p>chưa đáp ứng được mong đợi của Quý khách</p> -->
              </div>
              <b-row>
                <b-col sm="6">
                  <div class="text-popup">
                    <p>
                      Quý khách vui lòng góp ý những điểm nhân viên Vietmap cần
                      cải thiện để Quý khách hài lòng hơn
                    </p>
                  </div>
                </b-col>
                <b-col sm="6">
                  <form>
                    <b-form-group
                      label="Số điện thoại (không bắt buộc)"
                      label-for="phone-input"
                      style="
                        font-weight: bold;
                        font-size: 12px;
                        margin-bottom: 20px;
                      "
                    >
                      <b-form-input
                        id="phone-input"
                        placeholder="Nhập số điện thoại của Quý khách"
                      ></b-form-input>
                    </b-form-group>
                    <b-form-group
                      label="Góp ý"
                      label-for="comment-input"
                      style="
                        font-weight: bold;
                        font-size: 12px;
                        margin-bottom: 20px;
                      "
                    >
                      <textarea
                        id="comment-input"
                        placeholder="Ghi góp ý của Quý khách vào đây"
                      ></textarea>
                    </b-form-group>
                  </form>
                </b-col>
                <router-link to="/thankyou2">
                  <b-button type="submit" class="btn btn-primary sendcomment"
                    >GỬI ĐÁNH GIÁ</b-button
                  ></router-link
                >
              </b-row>
            </div>
          </b-modal>
          <!-- Popup45 -->
          <b-modal id="modal-center6" hide-footer="true">
            <div class="modal-center___BV_modal_body_">
              <div class="image-popup">
                <img src="../assets/button8.svg" />
              </div>
              <div class="text-comment">
                <p>Quý khách vui lòng cho</p>
                <p>Vietmap xin số điện thoại</p>
              </div>
              <form>
                <b-form-group
                  label="Số điện thoại (không bắt buộc)"
                  label-for="phone-input"
                  style="
                    font-weight: bold;
                    font-size: 12px;
                    margin-bottom: 20px;
                  "
                >
                  <b-form-input
                    id="phone-input"
                    placeholder="Nhập số điện thoại của Quý khách"
                  ></b-form-input>
                </b-form-group>
                <router-link to="/thankyou3">
                  <b-button type="submit" class="btn btn-primary sendcomment"
                    >GỬI ĐÁNH GIÁ</b-button
                  ></router-link
                >
              </form>
            </div>
          </b-modal>
          <router-view />
        </b-col>
      </b-row>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import InfoCustomer from "@/components/InfoCustomer.vue";
// import InfoCustomer from '../components/InfoCustomer.vue';

export default {
  name: "Home",
  components: {
    InfoCustomer,
  },
};
</script>

<style scoped>
.home {
  width: 100vw;
  height: 100vh;
  text-align: center;
  flex-direction: row;
  margin-bottom: 10px;
}
.content {
  margin-top: 30px;
}
.text {
  line-height: 20px;
}
.text-1 {
  color: #292c2e;
  font-size: 28px;
  margin-bottom: 30px;
}
.text-show {
  font-size: 48px;
  line-height: 50px;
  color: #00aeef;
  font-weight: bold;
  margin-top: 20px;
  margin-bottom: 20px;
}
.text-2 {
  font-size: 16px;
  color: #292c2e;
  text-align: center;
}
.rating {
  margin-top: 48px;
}
ul {
  padding: 8px;
}
button {
  /* border: 1px solid #6c757d59;
  border-radius: 8px; */
  width: 140px;
  height: 140px;
  border: 0;
  /* padding: 10px; */
  margin: 10px;
  background-color: rgb(255 255 255 / 4%);
}
.btn {
  width: 100px;
  height: 50px;
  display: inline-block;
  margin-top: 0px;
  padding: 2;
  font-weight: 400;
  line-height: 1.5;
  color: #212529;
  text-align: center;
  text-decoration: none;
  vertical-align: middle;
  cursor: pointer;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  border: 1px solid;
  padding: 0.375rem 0.75rem;
  font-size: 1rem;
  border-radius: 0.25rem;
  transition: none;
}
a {
  text-decoration: none;
}
.text-3 {
  font-size: 14px;
  line-height: 16px;
  color: #292c2e;
  font-weight: bold;
}

.image-popup {
  width: 96px;
  height: 96px;
  line-height: 96px;
  margin-bottom: 40px;
}
.text-comment {
  font-size: 20px;
  color: #00aeef;
  vertical-align: middle;
  font-weight: bold;
  margin-bottom: 24px;
  text-align: center;
}
.text-popup {
  font-size: 18px;
  color: #464a4d;
  justify-content: center;
  align-items: center;
  display: flex;
  margin-bottom: 40px px;
}
.label {
  font-weight: bold;
  font-size: 12px;
  margin-bottom: 10px;
}
.form-control {
  margin-bottom: 10px;
  font-size: 12px;
}
form-input {
  border: 1px solid;
  border-radius: 10px;
}
textarea {
  width: 100%;
  height: 75px;
  border: 1px solid #ced4da;
  border-radius: 0.5rem;
}
.sendcomment {
  background-color: #05bbff;
  font-size: 16px;
  color: #fff;
  width: 100%;
  margin-top: 20px;
  margin-left: 0;
}
.modal-body {
  align-items: center;
  width: 50%;
  padding: 3rem !important;
}
button.close {
  border: 1px solid #fff;
}
.image-popup {
  align-items: center;

  margin-left: auto;
  margin-right: auto;
}
form {
  margin-top: 30px;
}
p {
  padding: 0;
  margin-bottom: 0;
}
.image {
  width: 100%;
}
pre {
  overflow: hidden;
}
@media (min-width: 992px) {
  .home {
    margin-top: 30px;
  }
  button {
    width: 180px;
    height: 180px;
    border: none;
  }
  .text-3 {
    font-size: 15px;
  }
  .rating {
    margin-top: 0px;
  }
  .text-2 {
    font-size: 20px;
  }
  .modal-body {
    align-items: center;
    padding: 2.5rem;
  }
  col .text-2 {
    font-size: 16px;
    text-align: center;
  }
  .text-popup {
    text-align: center;
  }
  .sendcomment {
    width: 100%;
    align-items: center;
  }
  .text-comment {
    font-size: 18px;
  }
  .modal-body {
    padding: 2rem;
  }
}
/* Small devices (landscape phones, 576px and up) */
@media (max-width: 576px) {
  #session1 {
    visibility: visible;
  }
  #session2 {
    display: none;
  }
  .text-1 {
    font-size: 14px;
    margin-bottom: 0;
  }
  .text-show {
    font-size: 30px;
    margin: 15px;
  }
  .text-2 {
    font-size: 10px;
  }
  .rating {
    margin-top: 0;
  }
  ul {
    margin-top: 0;
  }
  .text-3 {
    display: none;
  }
  button {
    width: 50px;
    margin: 5px;
    height: 50px;
  }
  .modal-body {
    padding: 4rem;
  }
  .text-comment {
    font-size: 18px;
  }
  .text-popup {
    font-size: 13px !important;
    text-align: center;
  }
  .text-home {
    font-size: 12px;
  }
}

/* Tablet */
@media (min-width: 768px) {
  .home {
    margin-top: 30px;
  }
  #session1 {
    visibility: visible;
  }
  #session2 {
    display: none;
  }
  button {
    margin: 0;
  }
  .text-popup {
    font-size: 16px;
    text-align: center;
  }
  .text-4 {
    font-size: 20px;
  }
  .text-2 {
    margin-top: 20px;
  }
  .text-home {
    font-size: 25px;
    line-height: 40px;
  }
  pre {
    overflow: hidden;
  }
}
/*Extra large devices (large desktops, 1200px and up) */
@media (min-width: 992px) {
  .home {
    margin-top: 30px;
  }
  #session1 {
    display: none;
  }
  #session2 {
    display: block;
  }
  button {
    width: 180px;
    height: 180px;
    border: none;
    background-color: rgb(255 255 255 / 4%);
    margin: 20px;
  }
  .text-3 {
    font-size: 15px;
  }
  .rating {
    margin-top: 0px;
  }
  .text-2 {
    font-size: 20px;
  }
  .text-popup {
    font-size: 13px;
  }
  form {
    margin-top: 0;
  }
  .modal-content {
    width: 500px;
  }
  .modal-body {
    position: relative;
    padding: 3rem;
  }
  .text-comment {
    margin-bottom: 20px;
  }
}
</style>
