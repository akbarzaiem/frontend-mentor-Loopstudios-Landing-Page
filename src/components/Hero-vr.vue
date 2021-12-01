<template>
  <div class="middle">
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
    <div class="left">
      <img src="../assets/desktop/image-interactive.jpg" alt="" />
    </div>
    <div class="right">
      <div class="box">
        <p class="tittle">THE LEADER IN INTERACTIVE VR</p>
        <p class="desc">
          Founded in 2011, Loopstudios has been producing world-class virtual
          reality projects for some of the best companies around the globe. Our
          award-winning creations have transformed businesses through digital
          experiences that bind to their brand.
        </p>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: "Hero-vr",
};
</script>

<style scoped>
.middle {
  display: flex;
  margin-top: 50px;
  justify-content: center;
}
.left {
  position: relative;
  height: 100%;
  right: 13%;
}
.right {
  position: absolute;
  margin-top: 190px;
  margin-left: 600px;
}
.box {
  box-sizing: border-box;
  background-color: white;
  width: 600px;
  height: 370px;
  padding: 50px;
}
.box .tittle {
  font-size: 45px;
  word-spacing: 2px;
  text-align: start;
  font-family: "Josefin Sans", sans-serif;
}
.box .desc {
  text-align: justify;
  width: 400px;
  font-family: "Alata", sans-serif;
  color: hsl(0, 0%, 55%);
  font-size: 15px;
}
@media only screen and (min-width: 320px) and (max-width: 480px) {
  .middle {
    flex-direction: column;
    width: 90%;
  }
  .middle .left {
    left: 5%;
    right: 5%;
  }
  .middle .left img {
    width: 100%;
  }
  .right {
    margin-top: 200%;
    margin-left: 0%;
    margin-bottom: 30%;
  }
  .box {
    box-sizing: border-box;
    background-color: white;
    width: 100%;
    height: 70%;
    padding: 0%;
    left: 0%;
  }
  .box .tittle {
    margin-left: 5%;
    margin-right: 5%;
    margin-bottom: 20%;
    width: 90%;
    font-size: 45px;
    word-spacing: 2px;
    text-align: center;
    font-family: "Josefin Sans", sans-serif;
  }
  .box .desc {
    margin-left: 5%;
    margin-right: 5%;
    text-align: justify;
    margin-top: -10%;
    width: 90%;
    font-family: "Alata", sans-serif;
    color: hsl(0, 0%, 55%);
    font-size: 15px;
  }
}

@media only screen and (min-width: 481px) and (max-width: 768px) {
  .middle {
    width: 90%;
    display: flex;
    flex-direction: column;
  }
  .middle .left {
    left: 5%;
    right: 5%;
  }
  .middle .left img {
    width: 100%;
  }
  .middle .right {
    margin-top: 220%;
    margin-left: 5%;
    margin-right: 5%;
    margin-bottom: 50%;
    width: 90%;
  }
  .box {
    width: 100%;
    height: max-content;
    margin-left: 0%;
  }
  .box .tittle {
    margin-left: 5%;
    margin-right: 5%;
    margin-bottom: 20%;
    width: 90%;
    font-size: 45px;
    word-spacing: 2px;
    text-align: center;
    font-family: "Josefin Sans", sans-serif;
  }
  .box .desc {
    margin-left: 5%;
    margin-right: 5%;
    text-align: justify;
    margin-top: -10%;
    width: 90%;
    font-family: "Alata", sans-serif;
    color: hsl(0, 0%, 55%);
    font-size: 15px;
  }
}

@media only screen and (min-width: 769px) and (max-width: 1024px) {
  .middle {
    width: 90%;
    display: flex;
    flex-direction: column;
  }
  .left {
    height: 100%;
    right: 5%;
    left: 5%;
  }
  .middle .left img {
    width: 100%;
  }
  .right {
    margin-top: 10%;
    margin-left: 5%;
    margin-right: 5%;
    width: 100%;
    position: relative;
  }
  .box {
    width: 100%;
    height: max-content;
  }
  .box .tittle {
    margin-left: 5%;
    margin-right: 5%;
    margin-bottom: 20%;
    width: 90%;
    font-size: 45px;
    word-spacing: 2px;
    text-align: center;
    font-family: "Josefin Sans", sans-serif;
  }
  .box .desc {
    margin-left: 5%;
    margin-right: 5%;
    text-align: justify;
    margin-top: -10%;
    width: 90%;
    font-family: "Alata", sans-serif;
    color: hsl(0, 0%, 55%);
    font-size: 15px;
  }
}
</style>