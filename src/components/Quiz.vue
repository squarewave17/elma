<template>
  <section class="quiz">
    <div id="realEstate">
      <header>
        <img class="logo" src="@/assets/logo_real-estate.svg" />
      </header>
      <div class="estate-list">
        <div class="estate-image">
          <img src="@/assets/properties/property_1_starter.jpg" />
        </div>
        <div class="estate-info">
          <div>
            <h6>Starter</h6>
            <img src="@/assets/avatars/pete_agent.png" />
            <p class="name">Pete Agent</p>
          </div>
          <div>
            <p class="price">$285 per week</p>
          </div>
        </div>
      </div>
      <footer class="realestate-footer">
        <button class="realestate-btn">Select Property</button>
      </footer>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
#realEstate {
  background-color: #f9eded;
  height: 100vh;
  position: absolute;
  width: 100%;
}
.logo {
  position: relative;
  top: 81px;
  left: 50%;
  transform: translateX(-50%);
}
.estate-list {
  display: flex;
  flex-direction: column;
  position: relative;
  top: 169px;
  width: 358px;
  left: 50%;
  transform: translateX(-50%);
}
.estate-info {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  background: white;
  border-radius: 20px;
  position: absolute;
  top: 90%;
  width: 100%;
  height: 103px;
}
.estate-image img {
  width: 358px;
  border-radius: 21px;
}
.estate-info h6 {
  color: #143656;
  font-size: 20px;
  line-height: 27px;
  letter-spacing: -0.3px;
  padding-left: 26px;
  padding-top: 15px;
  font-family: 'Nunito';
}
.estate-info img {
  border: 5px solid #fff;
  padding-left: 26px;
}
.estate-info .name {
  color: #143656;
  font-size: 11px;
  line-height: 13px;
  letter-spacing: -0.3px;
  position: relative;
  left: 80%;
  top: -24%;
  font-family: 'Rubik';
  font-weight: 300;
}
.estate-info .price {
  font-size: 20px;
  line-height: 24px;
  letter-spacing: -0.3px;
  color: #143656;
  padding-right: 23px;
  padding-top: 42px;
  font-family: 'Rubik';
  font-weight: 500;
}
.realestate-footer {
  position: fixed;
  bottom: 0;
  background: #fff;
  width: 100%;
  box-shadow: 0px -5px 50px rgba(15, 26, 66, 0.05);
  border-radius: 20px;
  display: flex;
  justify-content: center;
  height: 70px;
  align-items: center;
}
.realestate-btn {
  background: #be1e2d;
  border-radius: 10px;
  color: white;
  padding: 10px 33px;
  height: 40px;
  border: none;
  font-family: 'Rubik';
  cursor: pointer;
}
</style>
