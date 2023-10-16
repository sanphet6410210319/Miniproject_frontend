<template>
    <div>
      <v-row >
        <!-- Title with Frame and Shadow -->
        <v-col>
          <div class="title-frame">
            <h1>พัฒนาการของทารก เดือนที่ 7 (สัปดาห์ที่ 27-30)</h1>
          </div >
        </v-col>

        <!-- Card 1 -->
        <v-col >
            <v-card class="mx-auto" max-width="344" style="box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.8);">            <v-img
              src="../assets/apd/27-28-Week-794x1024.webp"
              height="400px"
            ></v-img>
            <v-card-title>
              สัปดาห์ ที่ 27-28
            </v-card-title>
            <v-card-subtitle>
              ดูรายละเอียด
            </v-card-subtitle>
            <v-card-actions>
              <v-btn icon @click="show1 = !show1">
                <v-icon>{{ show1 ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
              </v-btn>
            </v-card-actions>
            <v-expand-transition>
              <div v-show="show1">
                <v-divider></v-divider>
                <v-card-text>
                  ทารกเริ่มตัวใหญ่ขึ้นแล้วนะ ดวงตาก็เจริญเติบโตมากจนพร้อมจะลืมตาและมองเห็นได้ในอีกไม่ช้า ขนตาก็ขึ้นแล้ว สมองก็โตเต็มคับกะโหลกศีรษะ มีรอยหยักและจุดเชื่อมต่อเก็บข้อมูลต่าง ๆ ในสมองมากขึ้นแล้วด้วย                   </v-card-text>
              </div>
            </v-expand-transition>
          </v-card>
        </v-col>
  
        <!-- Card 2 -->
        <v-col>
            <v-card class="mx-auto" max-width="344" style="box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.8);">            <v-img
              src="../assets/apd/29-30-Week-794x1024.webp"
              height="400px"
            ></v-img>
            <v-card-title>
              สัปดาห์ ที่ 29-30
            </v-card-title>
            <v-card-subtitle>
              ดูรายละเอียด
            </v-card-subtitle>
            <v-card-actions>
              <v-btn icon @click="show2 = !show2">
                <v-icon>{{ show2 ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
              </v-btn>
            </v-card-actions>
            <v-expand-transition>
              <div v-show="show2">
                <v-divider></v-divider>
                <v-card-text>
                  ผมและเล็บทารกเริ่มสวย และศีรษะของทารกก็มีขนาดใหญ่ขึ้น ทั้งนี้ก็เพื่อรองรับสมองที่พัฒนาอย่างต่อเนื่อง นอกจากนี้ทารกเริ่มสามารถควบคุมอุณหภูมิร่างกายของตัวเองได้แล้วและไขกระดูกที่มีหน้าที่ผลิตเซลล์เม็ดเลือดแดงก็พัฒนาสมบูรณ์แล้ว
                </v-card-text>
              </div>
            </v-expand-transition>
          </v-card>
        </v-col>

      </v-row>
    </div>
  </template>
  
  <script>
  export default {
    data: () => ({
      show1: false,
      show2: false,
    
      
    }),
  };
  </script>
  <style>
.title-frame {
  border: 2px solid #007BFF; /* Border style and color */
  box-shadow: 0px 0px 10px #007BFF; /* Box shadow style and color */
  text-align: center;
  padding: 10px;
  border-radius: 10px; /* Rounded corners */
}

.title-frame h1 {
  font-size: 24px; /* Adjust the font size as needed */
  margin: 0;
}
.v-card {
  margin-top: 100px; /* Add margin to center the cards vertically */
}
</style>