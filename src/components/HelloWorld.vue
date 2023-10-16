<template >
  <v-container>
    <div class="title-frame" >
      <h1 class="mothertext">Welcome to <span class="heart-box">Mother's heart box</span></h1>    </div>
    <div class="image-container">
      <div class="image-wrapper" @click="goToHistory">
        <v-img
          contain
          src="@/assets/1.1.png"
          class="image"
        ></v-img>
      </div>
      <div class="image-wrapper" @click="goToMemory">
        <v-img
          contain
          src="@/assets/1.2.png"
          class ="image"
        ></v-img>
      </div>
      <div class="image-wrapper" @click="goToAgeDp">
        <v-img
          contain
          src="@/assets/1.3.png"
          class="image"
        ></v-img>
      </div>
      <div class="image-wrapper" @click="goToConduct">
        <v-img
          contain
          src="@/assets/1.4.png"
          class="image"
        ></v-img>
      </div>
      <div class="image-wrapper" @click="goToInfant">
        <v-img
          contain
          src="@/assets/1.5.png"
          class="image"
        ></v-img>
      </div>
    </div>
    <br>
    <div class="video-container">
      <!-- Embed YouTube Video -->
      <div class="video-wrapper">
        <iframe
          width="500"
          height="315"
          src="https://www.youtube.com/embed/VcYgeNLkT-A"
          frameborder="0"
          allowfullscreen
        ></iframe>
      </div>
    </div>
  </v-container>
</template>

<style scoped>
.title-frame h1 {
  font-size: px; /* Adjust the font size as needed */
  margin: 0;
}
.title-frame {
  border: 2px solid #007BFF; /* Border style and color */
  box-shadow: 0px 0px 10px #007BFF; /* Box shadow style and color */
  text-align: center;
  padding: 2px;
  border-radius: 10px; /* Rounded corners */
}
.mothertext {
  text-align: center;
  margin-top: 50px;
  margin-bottom: 50px;
  font-size: 28px;
}

.heart-box {
    color: #ff69b4;
    font-weight: bold;
  }

  .heartbeat {
    animation: heartbeat 2s infinite;
  }

  @keyframes heartbeat {
    0% {
      transform: scale(1);
    }
    25% {
      transform: scale(1.1);
    }
    50% {
      transform: scale(0.9);
    }
    75% {
      transform: scale(1.1);
    }
    100% {
      transform: scale(1);
    }
  }
.mothertext {
  animation: textAnimation 1s ease-in-out; /* เพิ่ม animation ให้กับข้อความ */
}

.image-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center; /* จัดให้อยู่ตรงกลางแนวนอน */
  margin-top: 30px; /* ระยะห่างของรูปภาพด้านบน */
}

.image-wrapper {
  margin: 20px; /* ระยะห่างระหว่างรูปภาพ */
  max-width: 200px;
  max-height: 200px;
  cursor: pointer;
  transition: transform 0.2s; /* เพิ่มอนิเมชันการเปลี่ยนรูปภาพเมื่อเม้าส์ไปชี้ */
}

.image-wrapper:hover {
  transform: scale(1.1); /* เพิ่มขนาดของรูปภาพเมื่อเม้าส์ไปชี้ */
}

.video-container {
  display: flex;
  justify-content: center;
  margin-top: 30px;
}

.video-wrapper {
  max-width: 580px; /* ขนาดสูงสุดของรูปภาพวิดีโอ */
  margin: 0 auto; /* จัดให้วิดีโออยู่ตรงกลาง */
  border: 5px solid #333; /* เพิ่มเส้นขอบสีเข้มเป็นกรอบ */
  box-shadow: 5px 10px 15px rgba(0, 0, 0, 0.8); /* เพิ่มเอฟเฟกต์เงา */
}
.title-frame h1 {
  font-size: px; /* Adjust the font size as needed */
  margin: 0;
}

.top-left-image {
    position: absolute;
    top: 0;
    left: 0;
    width: 20%; /* Adjust the width as needed */
  }

  .top-right-image {
    position: absolute;
    top: 0;
    right: 0;
    width: 20%; /* Adjust the width as needed */
  }

  .title-frame {
    border: 2px solid #ddd;
    padding: 20px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    text-align: center;
    margin-top: 50px;
    margin-bottom: 50px;
    transition: transform 0.5s ease-in-out;
  }

  .title-frame:hover {
    transform: scale(1.05);
  }

  .mothertext {
    font-size: 28px;
    color: #333;
    font-family: 'Fredoka One', cursive;
    animation: textAnimation 1s ease-in-out;
  }

  .heart-box {
    color: #ff69b4;
    font-weight: bold;
    animation: heartbeat 2s infinite;
  }
</style>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {};
  },
  methods: {
    goToAgeDp() {
      this.$router.push({ path: '/agedp' }).catch(() => {});
    },
    goToMemory() {
      this.$router.push({ path: '/memory' }).catch(() => {});
    },
    goToConduct() {
      this.$router.push({ path: '/conduct' }).catch(() => {});
    },
    goToInfant() {
      this.$router.push({ path: '/infant' }).catch(() => {});
    },
    goToHistory() {
      this.$router.push({ path: '/history' }).catch(() => {});
    },
  },
};
</script>
