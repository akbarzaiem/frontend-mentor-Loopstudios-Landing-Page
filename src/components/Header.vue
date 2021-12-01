<template>
  <header>
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
    <div class="one">
      <div class="logo-image">
        <img src="../assets/logo.svg" alt="" />
      </div>
      <div class="navbar">
        <div class="index">
          <div class="item">About</div>
          <div class="item">Carrers</div>
          <div class="item">Events</div>
          <div class="item">Products</div>
          <div class="item">Supports</div>
        </div>
        <div class="hamburger" @click="mobileMenu">
          <span class="bar"></span>
          <span class="bar"></span>
          <span class="bar"></span>
        </div>
      </div>
    </div>
    <div class="two">
      <div class="hero-text">
        <p>IMMERSIVE EXPERIENCES THAT DELIVER</p>
      </div>
    </div>
  </header>
</template>

<style scoped>
header {
  position: relative;
  background-image: url("../assets/desktop/image-hero.jpg");
  background-repeat: no-repeat;
  width: 100%;
  height: 100%;
}
.one {
  display: flex;
}
.one .logo-image {
  width: 50%;
  margin-left: 10%;
}
.one .logo-image img {
  margin-top: 9%;
}
.one .navbar {
  width: 100%;
}
.index {
  display: flex;
  justify-content: flex-end;
  gap: 20px;
  margin-right: 17%;
  margin-top: 5%;
  color: white;
  cursor: pointer;
  font-family: "Alata", sans-serif;
}
.navbar .item:hover {
  text-decoration: underline;
  color: white;
}

.hero-text {
  margin-top: 10%;
  margin-left: 10%;
  box-sizing: border-box;
  width: 50%;
  height: 30%;
  color: white;
  font-size: 60px;
  border-style: solid;
  border-color: white;
}
.hero-text p {
  margin-top: 9%;
  margin-left: 6%;
  font-family: "Josefin Sans", sans-serif;
}

.hamburger .bar {
  display: block;
  width: 25px;
  height: 3px;
  margin: 5px auto;
  -webkit-transition: all 0.3s ease-in-out;
  transition: all 0.3s ease-in-out;
  background-color: white;
}

.hamburger {
  display: none;
}

@media only screen and (min-width: 320px) and (max-width: 480px) {
  .one .logo-image {
    margin-left: 5%;
    margin-top: 5%;
  }
  .one .logo-image img.active {
    position: absolute;
    z-index: 1;
    margin-left: 5%;
    margin-top: 5%;
  }
  .hero-text {
    margin-left: 5%;
    margin-right: 5%;
    margin-top: 30%;
    width: 90%;
    font-size: 2.5em;
  }
  .hero-text p {
    margin-top: 9%;
    margin-left: 3%;
  }

  .index {
    position: fixed;
    left: -100%;
    height: 104%;
    top: -4%;
    display: flex;
    flex-direction: column;
    background-color: black;
    color: white;
    width: 100%;
    border-radius: 10px;
    text-align: center;
    transition: 0.3s;
    box-shadow: 0 10px 27px rgba(0, 0, 0, 0.05);
    font-family: "Josefin Sans", sans-serif;
    text-transform: uppercase;
  }
  .index.active {
    left: 0%;
  }

  .item {
    margin: 2.5rem 0;
  }

  /* .index .item:hover.active {
    text-decoration: underline;
    color: black;
  } */
  .navbar {
    align-self: flex-end;
    margin-bottom: 1%;
  }
  .hamburger {
    display: block;
    cursor: pointer;
  }

  .hamburger.active .bar:nth-child(2) {
    opacity: 0;
  }

  .hamburger.active .bar:nth-child(1) {
    transform: translateY(8px) rotate(45deg);
    margin-top: 20%;
  }

  .hamburger.active .bar:nth-child(3) {
    transform: translateY(-8px) rotate(-45deg);
    margin-top: 1.5%;
  }
}

@media only screen and (min-width: 481px) and (max-width: 768px) {
  header {
    height: 500px;
    margin-bottom: 0%;
    width: 100%;
    overflow-y: hidden;
  }
  .hero-text {
    width: 70%;
    font-size: 2.8em;
  }
  .one .logo-image img {
    margin-top: 9%;
    height: 40%;
  }
  .one .navbar {
    width: 100%;
  }
  .index {
    display: flex;
    justify-content: flex-end;
    gap: 15px;
    font-size: 80%;
    margin-right: 17%;
    margin-top: 5%;
    color: white;
    cursor: pointer;
    font-family: "Alata", sans-serif;
  }
}

@media only screen and (min-width: 769px) and (max-width: 1024px) {
  .hero-text {
    width: 50%;
    font-size: 2.6em;
  }
}
</style> */


<script>
export default {
  name: "Header",
  methods: {
    mobileMenu() {
      document.querySelector(".hamburger").classList.toggle("active");
      document.querySelector(".index").classList.toggle("active");
      document.querySelector(".one .logo-image img").classList.toggle("active");
    },
  },
};
</script>