<script setup lang="ts"></script>

<template>
  <v-card max-width="500" class="mx-auto" color="grey-lighten-9"
    >
    <v-layout>
      <v-app-bar
        color="teal-darken-1"
        image="https://www.industrybiznews.com/wp-content/uploads/2019/03/%E0%B8%A1.%E0%B8%9A%E0%B8%B9%E0%B8%A3%E0%B8%9E%E0%B8%B22-1130x460.jpg"
      >
        <v-app-bar-title>My Profile</v-app-bar-title>
      </v-app-bar>

      <v-main>
        <v-container fluid>
          <v-card
            border
            density="comfortable"
            title="ประวัตส่วนตัว"
            variant="text"
          >
            <v-img
              src="https://reg.buu.ac.th/registrar/getstudentimage.asp?id=64160056"
              height="250"
              width="250"
            ></v-img>

            <v-card-text>
              ชื่อ-นามสกุล : ภาสินี รักพรมราช <br />
              อายุ : 20 ปี <br />
              วัน/เดือน/ปีเกิด : 25 ตุลาคม 2545
            </v-card-text>
          </v-card>
          <v-card
            border
            class="mb-3"
            density="compact"
            title="ประวัติการศึกษา"
            variant="text"
          >
            <v-img
              src="https://www.m-culture.go.th/rayong/images/article/news1535/n20220919141423_18001.jpg"
              height="250"
              width="500"
              cover
            ></v-img>
            <v-card-text
              >มัธยมปลาย โรงเรียนชำนาญสามัคคีวิทยา สายการเรียน วิทย์-คณิต<br />
              <br />
              ปัจจุบัน กำลังศึกษาปริญญาตรี ที่มหาวิทยาลัยบูรพา<br />
              คณะวิทยาการสารสนเทศ สาขาวิทยาการคอมพิวเตอร์
            </v-card-text>
          </v-card>

          <v-card
            border
            density="comfortable"
            title="สิ่งที่เราสนใจ"
            variant="text"
          >
            <v-img
              src="https://www.chillpainai.com/src/wewakeup/scoop/images/9f9c00fb75e83461c7fad8aa9d3755e2c51b95ac.jpg"
              height="250"
              cover
            ></v-img>

            <v-card-text>
              การได้ไปท่องเที่ยวในที่ต่างๆ ของประเทศไทย
            </v-card-text>
          </v-card>
        </v-container>
      </v-main>
    </v-layout>
  </v-card>
</template>
