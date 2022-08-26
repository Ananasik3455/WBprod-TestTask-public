<template>
  <v-container
    class="d-flex flex-wrap px-6"
    fluid
  >
    <v-row>
      <v-col
        v-for="item in items_list" :key="item.id"
        cols="12"
        xs="12"
        sm="6"
        md="4"
        lg="3"
        xl="3"
        class="d-flex"
      >
        <v-card 
          color="#232633"
          class="pa-4 mb-16 d-flex flex-column flex-grow-1 align-self-stretch"
        >
          <h4 class="mb-2 body-2 grey--text">Заказ:</h4>
          <p class="mb-4 white--text">{{ item.idx }}</p>

          <v-container
            class="d-flex px-0 mb-2"
          >
          <!-- <div :style="{ height: '46px', width: '64px', backgroundImage: `url(${item.img})` }"></div> -->
            <img 
              width="64"
              height="64"
              :src="item.img"
            >
            <v-container
              class="py-0"
            >
              <p class="my-0 body-2 white--text">{{ item.title }}</p>
              <p class="mb-0 caption deep-purple--text">Арт. {{ item.art }}</p>
            </v-container>
          </v-container>

          <v-chip
            label
            class="mb-4 align-self-start"
            color="#F7981C"
          >
            <p class="my-0 caption white--text">{{ item.location }}</p>
          </v-chip>

          <p class="d-flex mb-4 white--text">
            <img 
              class="pr-2" 
              src="../assets/Calendar.png" 
              alt=""
            >
              {{ item.date }}
            <img
              class="ms-6 pr-2"
              src="../assets/TimeSquare.png" 
              alt=""
            > 
              {{ item.time }}
          </p>

          <h4 class="mb-2 body-2 grey--text">Получатель:</h4>
          <p class="mb-4 white--text">{{ item.recipient }}</p>

          <h4 class="mb-2 body-2 grey--text">Адрес:</h4>
          <p class="mb-4 white--text">{{ item.adres }}</p>

          <Button></Button>

        </v-card>
        </v-col>
    </v-row>
  </v-container>
</template>

<script>
import Button from './Button.vue'

export default {
  data: () => ({
    items_list: [
      {
        id: 0,
        idx: '65f884gre4s556w984fe8g4g84',
        title: 'Набор садового инструмента, 3 предмета: рыхлитель, 2 совка, пластиковые ручки Набор садового инструмента, 3 предмета: рыхлитель, 2 совка, пластиковые ручки Набор садового инструмента, 3 предмета: рыхлитель, 2 совка, пластиковые ручки',
        art: '485452965',
        location: 'В пути на пункт выдачи',
        date: '12 июня 2022',
        time: '19:17',
        recipient: 'Алексей Никитин +796*****2251',
        adres: 'г. Москва, м. Пушкинская, Дегярный переулок, д. 10с2',
        img: require("../assets/IconWb.png")
      },
      {
        id: 1,
        idx: '65f884gre4s556w984fe8g4g85',
        title: 'Набор садового инструмента, 3 предмета: рыхлитель, 2 совка, пластиковые ручки',
        art: '485452965',
        location: 'В пути на пункт выдачи',
        date: '12 июня 2022',
        time: '19:17',
        recipient: 'Алексей Никитин +796*****2251',
        adres: 'г. Москва, м. Пушкинская, Дегярный переулок, д. 10с2',
        img: require("../assets/IconWb.png")
      },
      {
        id: 2,
        idx: '65f884gre4s556w984fe8g4g86',
        title: 'Набор садового инструмента, 3 предмета: рыхлитель, 2 совка, пластиковые ручки',
        art: '485452965',
        location: 'В пути на пункт выдачи',
        date: '12 июня 2022',
        time: '19:17',
        recipient: 'Алексей Никитин +796*****2251',
        adres: 'г. Москва, м. Пушкинская, Дегярный переулок, д. 10с2 г. Москва, м. Пушкинская, Дегярный переулок, д. 10с2',
        img: require("../assets/IconWb.png")
      },
      {
        id: 3,
        idx: '65f884gre4s556w984fe8g4g86',
        title: 'Набор садового инструмента, 3 предмета: рыхлитель, 2 совка, пластиковые ручки',
        art: '485452965',
        location: 'В пути на пункт выдачи',
        date: '12 июня 2022',
        time: '19:17',
        recipient: 'Алексей Никитин +796*****2251',
        adres: 'г. Москва, м. Пушкинская, Дегярный переулок, д. 10с2',
        img: require("../assets/IconWb.png")
      },
      {
        id: 4,
        idx: '65f884gre4s556w984fe8g4g86',
        title: 'Набор садового инструмента, 3 предмета: рыхлитель, 2 совка, пластиковые ручки',
        art: '485452965',
        location: 'В пути на пункт выдачи',
        date: '12 июня 2022',
        time: '19:17',
        recipient: 'Алексей Никитин +796*****2251',
        adres: 'г. Москва, м. Пушкинская, Дегярный переулок, д. 10с2',
        img: require("../assets/IconWb.png")
      }
    ]
  }),
  components: {
    Button
  },
}
</script>