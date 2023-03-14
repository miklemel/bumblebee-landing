<template>
  <div>
  <div class="navbar1">
    <b-input-group size="lg">
      <b-input-group-prepend is-text>
        <b-icon icon="envelope"></b-icon>
      </b-input-group-prepend>
      <b-form-input type="email" placeholder="me@example.com"></b-form-input>
    </b-input-group>
    <b-container >

      <b-row class="justify-content-md-center align-items-center">
        <b-col sm="6" md="4">
          <b-img center class="main-logo" src="/img/main-logo.jpg" fluid></b-img>
        </b-col>
        <b-col sm="6" md="4" >
          <h1>BumBleBee</h1>
        </b-col>
<!--        <b-col sm="6" md="4">-->

<!--        </b-col>-->
      </b-row>
    </b-container>

    <b-container>
      <b-row class="justify-content-md-center">
        <b-col sm="6" md="2"
               v-for="item in routes"
               :key="item.title"
        >
          <router-link
            link
            :to="item.to"
            class="router-link"
          >
            {{ item.title }}
          </router-link>
        </b-col>

      </b-row>
    </b-container>

  </div>
    <div class="main"><router-view/>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332532323</h1>
      <h1>22332323</h1>
      <h1>2233332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22455332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>2235632323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>25352332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>223322323</h1>
      <h1>22332323</h1>
      <h1>223321323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1>
      <h1>22332323</h1></div>

</div>
</template>

<script>
import Vue from 'vue';
export default Vue.extend({
  name: 'RouterWrapper',
  components: {
  },
  data: () => ({

    routes: [
      { title: 'Главная', icon: 'map', to: '/main' },
      { title: 'О нас', icon: 'linked_camera', to: '/kdd-list' },
      { title: 'Посчитать стоимость', icon: 'backup_table', to: '/statistics' },
      { title: 'Фичи', icon: 'emoji_people', to: '/users' },
      // { title: 'Контакты', icon: 'emoji_people', to: '/users' },
    ]
  }),
  methods: {

  }
});
</script>
<style lang="scss">
.navbar1 {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
}
.main {
  margin-top: 250px;
}
.main-logo {
  width: 140px;
  height: 110px;
}
.router-link {
  //padding: 30px;
}
</style>
