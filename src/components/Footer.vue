<template>
  <footer>
    <!-- font alata -->
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Alata&display=swap"
      rel="stylesheet"
    />
    <!-- font josefin sans -->
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Josefin+Sans:wght@300&display=swap"
      rel="stylesheet"
    />
    <div class="top">
      <div class="left">
        <img src="../assets/logo.svg" alt="" />
      </div>
      <div class="right">
        <div class="social-media">
          <img src="../assets/icon-facebook.svg" alt="" />
        </div>
        <div class="social-media">
          <img src="../assets/icon-twitter.svg" alt="" />
        </div>
        <div class="social-media">
          <img src="../assets/icon-pinterest.svg" alt="" />
        </div>
        <div class="social-media">
          <img src="../assets/icon-instagram.svg" alt="" />
        </div>
      </div>
    </div>
    <div class="bottom">
      <div class="left">
        <div class="item">About</div>
        <div class="item">Careers</div>
        <div class="item">Events</div>
        <div class="item">Products</div>
        <div class="item">Supports</div>
      </div>
      <div class="right">© 2021 Loopstudio. All right reserved</div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
footer {
  background-color: black;
  color: white;
  margin-top: 100px;
  height: 150px;
}
.top {
  display: flex;
}
.top .right {
  display: flex;
  margin-left: 53%;
  gap: 20px;
  margin-top: 30px;
  cursor: pointer;
}
.top .right img:hover {
  opacity: 0.5;
}
.top .left {
  display: flex;
  margin-top: 30px;
  margin-left: 10%;
  cursor: pointer;
}

.bottom {
  display: flex;
  margin-top: 30px;
}
.bottom .left {
  display: flex;
  margin-left: 10%;
  gap: 30px;
  font-family: "Alata", sans-serif;
}
.bottom .left .item:hover {
  text-decoration: underline;
  color: white;
  cursor: pointer;
}
.bottom .right {
  display: flex;
  margin-left: 31%;
  font-family: "Josefin Sans", sans-serif;
  color: hsl(0, 0%, 55%);
}
@media only screen and (min-width: 320px) and (max-width: 480px) {
  footer {
    height: 100%;
    position: relative;
  }
  .top .left {
    width: 100%;
    margin-top: 20%;
    margin-left: 0%;
    justify-content: center;
  }
  .top .right {
    width: 100%;
    margin-left: 0%;
    margin-top: 120%;
    position: absolute;
    justify-content: center;
  }
  .bottom .left {
    margin-left: 0%;
    flex-direction: column;
    width: 100%;
    align-items: center;
  }

  .bottom .right {
    margin-left: 0%;
    margin-top: 95%;
    width: 100%;
    justify-content: center;
    position: absolute;
  }
}

@media only screen and (min-width: 481px) and (max-width: 768px) {
  footer {
    height: 130%;
    position: relative;
  }
  .top .left {
    width: 100%;
    margin-top: 10%;
    margin-left: 0%;
    justify-content: center;
  }
  .top .right {
    width: 100%;
    margin-left: 0%;
    margin-top: 80%;
    position: absolute;
    justify-content: center;
  }
  .bottom .left {
    margin-left: 0%;
    flex-direction: column;
    width: 100%;
    align-items: center;
  }

  .bottom .right {
    margin-left: 0%;
    margin-top: 70%;
    width: 100%;
    justify-content: center;
    position: absolute;
  }
}

@media only screen and (min-width: 769px) and (max-width: 1024px) {
  .top .right {
    margin-left: 35%;
  }
  .bottom .right {
    margin-left: 12%;
  }
}
</style>