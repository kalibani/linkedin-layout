<template>
  <b-navbar toggleable="md" type="dark" variant="dark">
    <b-container>
      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
        <b-navbar-brand href="#">
          <router-link :to="{ name: 'MainComponent' }">
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c9/Linkedin.svg/2000px-Linkedin.svg.png" alt="Responsive image" width="38" height="38">
          </router-link>
        </b-navbar-brand>

      <b-collapse is-nav id="nav_collapse">
        <b-nav-form>
          <b-input-group>
            <b-form-input @focus.native="showSearchContent" @blur.native="hideSearchContent" v-model="search"></b-form-input>
            <b-button variant="dark" slot="append">
              <i class="fas fa-search"></i>
            </b-button>
          </b-input-group>
          <div v-if="isShow" class="card custom-card">
            <div class="card-body">
              <p class="card-text">Search for</p>
              <div class="search-title">
                <i class="fas fa-user-friends"></i>
                <h5>People</h5>
              </div>
              <div class="search-title">
                <i class="fas fa-briefcase"></i>
                <h5>Jobs</h5>
              </div>
              <div class="search-title">
                <i class="far fa-id-card"></i>
                <h5>Posts</h5>
              </div>
              <hr>
              <p class="card-text">Recent</p>
              <div class="image-wrapper" v-for="user in filteredUsers" :key="user.id">
                <img src="https://media.licdn.com/dms/image/C4E03AQFlmLGSxfTBlg/profile-displayphoto-shrink_800_800/0?e=1535587200&v=beta&t=UbTW3eAZLM5QIqBoT3Fq4q_kxtYgjtGfom8W0rBYkc8" alt="Avatar image">
                <div class="suggestion-profile">
                  <h5>{{user.first_name}} {{ user.last_name }}</h5>
                </div>
              </div>
            </div>
          </div>
        </b-nav-form>
        <b-navbar-nav>
          <b-nav-item class="active">
            <div class="icon-wrapper">
              <router-link :to="{ name: 'MainComponent' }">
                <i class="fas fa-home"></i>
                <h1>Home</h1>
              </router-link>
            </div>
          </b-nav-item>
          <b-nav-item>
            <div class="icon-wrapper">
              <i class="fas fa-user-friends"></i>
              <h1>My Network</h1>
            </div>
          </b-nav-item>
          <b-nav-item>
            <div class="icon-wrapper">
              <i class="fas fa-briefcase"></i>
              <h1>Jobs</h1>
            </div>
          </b-nav-item>
          <b-nav-item>
            <div class="icon-wrapper">
              <i class="fas fa-envelope"></i>
              <h1>Messaging</h1>
            </div>
          </b-nav-item>
          <b-nav-item>
            <div class="icon-wrapper">
              <i class="fas fa-bell"><b-badge pill variant="danger">4</b-badge></i>
              <h1>Notifications</h1>
            </div>
          </b-nav-item>
          <b-nav-item>
            <div class="icon-wrapper">
              <router-link :to="{ name: 'AppProfile' }">
                <b-img src="https://media.licdn.com/dms/image/C5603AQFqH8-QoYdjDQ/profile-displayphoto-shrink_800_800/0?e=1535587200&v=beta&t=pQeXdcVKuXVHPkXBLiFr6Ha0OKcy-jcMHyWfBnEraCw" rounded="circle" width="24" height="24" blank-color="#777" alt="img" class="m-1" />
                <h2>Me</h2>
              </router-link>
            </div>
          </b-nav-item>
          <b-nav-item class="separated-border">
            <div class="icon-wrapper">
            <i class="fab fa-buromobelexperte"></i>
            <h1>Work</h1>
            </div>
          </b-nav-item>
          <b-nav-item>
            <div class="upgrade-offer">
              <h2>Free Upgrade to Premium</h2>
            </div>
          </b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-container>
  </b-navbar>
</template>

<script>
export default {
  name: 'AppNavbar',
  data () {
    return {
      isShow: false,
      /* eslint-disable */
      users : [
        { isActive: true, id: 40, first_name: 'Dickerson', last_name: 'Macdonald' },
        { isActive: false, id: 21, first_name: 'Larsen', last_name: 'Shaw' },
        { isActive: false, id: 89, first_name: 'Geneva', last_name: 'Wilson' },
        { isActive: false, id: 22, first_name: 'Martin', last_name: 'palermo' },
        { isActive: false, id: 80, first_name: 'Lionel', last_name: 'Messi' },
        { isActive: false, id: 25, first_name: 'Zlatan', last_name: 'Ibrahimovic' },
        { isActive: false, id: 84, first_name: 'Anton', last_name: 'Medan' }
      ],
      search: ''
    }
  },
  computed: {
    filteredUsers () {
      let self = this
      return this.users
        .filter(user => user.first_name
        .toLowerCase()
        .indexOf(self.search.toLowerCase()) >= 0
      )
    }
  },
  methods: {
    showSearchContent () {
      this.isShow = true
    },
    hideSearchContent () {
      this.isShow = false
    }
  }
}
</script>

<style scoped>
  .navbar{
    padding: 0px !important;
  }
  .active{
    border-bottom: 2px solid #fff;

  }

  .nav-item {
    padding-left: 10px !important;
    padding-right: 10px !important;
  }

  h1 {
    font-size: 12px;
    line-height: 16px;
    font-weight: 400;
    display: block;
    color: #fff !important;
  }
  .bg-dark{
    background: #283e4a !important;
    color: #fff !important;
  }

  .btn-dark {
    background: #e1e9ee !important;
    border-color: #e1e9ee !important;
  }
  .btn-dark i {
    color: blue !important;
  }

  .icon-wrapper{
    width: 100%;
  }

  .icon-wrapper i{
    font-size: 20px !important;
    margin-top: 10px;
    text-align: center;
    display: block;
    margin-left: auto;
    margin-right: auto;
    color: #fff !important;
  }

  .icon-wrapper img{
    margin-top: 7px;
    text-align: center;
    display: block;
    margin-left: auto;
    margin-right: auto;
    color: #fff;
  }

  .icon-wrapper h2{
    text-align: center;
    font-size: 12px;
    line-height: 11px;
    font-weight: 400;
    display: block;
    color: #fff !important;
  }

  .input-group{
    padding-right: 4rem;
  }

  .input-group .form-control {
    background-color: #fff !important;
  }

  .badge{
    padding: 3px 5px !important;
    font-size: 13px !important;
    position: relative;
    top: -11px;
    left: -9px;
  }

  .separated-border{
    margin-left: 20px;
    height: 73px;
    border-left: 1px solid  #5c6f7c;
  }

  .upgrade-offer{
    max-width: 80px;
    margin-top: 15px;
  }

  .upgrade-offer h2{
    text-align: center;
    font-size: 12px;
    line-height: 11px;
    font-weight: 600;
    display: block;
    color: #dccea4 !important;
  }

  .custom-card {
    position: absolute;
    top: 60px;
    z-index: 1;
    width: 46rem;
  }

  .custom-card p {
    color: #000;
    font-weight: bold;
  }

  .custom-card .search-title h5 {
    color: #495D6E;
    font-size: 15px;
    margin-left: 11px;
    margin-bottom: 11px;
    font-weight: bold;
    display: inline-block;
  }

  .custom-card .search-title i {
    color: #0084bf;
  }

  .image-wrapper {
    margin-bottom: 10px;
  }

  .image-wrapper img {
    vertical-align: top;
    width: 40px;
    height: 40px;
    border-radius: 50%;
  }

  .suggestion-profile {
    display: inline-block;
  }

  .suggestion-profile h5 {
    font-size: 16px;
    padding-top: 10px;
    padding-left: 5px;
    color: #000;
    font-weight: bold;
  }

  @media (min-width: 1025px) and (max-width: 1280px) {

    .input-group .form-control {
      display: flex;
      width: 182px;
    }

    .input-group{
      padding-right: 5rem;
    }

    .nav-item {
      padding-left: 3px !important;
      padding-right: 3px !important;
    }

  }

  @media (min-width: 1281px) {
    .input-group .form-control {
      display: flex;
      width: 250px;
    }
  }

  /*
    ##Device = Tablets, Ipads (landscape)
    ##Screen = B/w 768px to 1024px
  */
  @media (min-width: 768px) and (max-width: 1024px) {

    .input-group .form-control {
      display: flex;
      width: 114px;
    }

    .input-group{
      padding-right: 0rem;
    }

    .icon-wrapper i{
      font-size: 13px !important;
      margin-top: 10px;
      text-align: center;
      display: block;
      margin-left: auto;
      margin-right: auto;
      color: #fff !important;
    }

    .icon-wrapper h1 {
      font-size: 10px;
      line-height: 16px;
      font-weight: 400;
      display: block;
      color: #fff !important;
    }

    .icon-wrapper img{
      margin-top: 7px !important;
      text-align: center;
      display: flex;
      margin-left: auto !important;
      margin-right: auto !important;
      color: #fff !important;
    }

    .nav-item {
      padding-left: 0px !important;
      padding-right: 0px !important;
    }

  }

  /*
    ##Device = Mobile(landscape)
    ##Screen = B/w 320px to 480px
  */

  @media (min-width: 320px) and (max-width: 480px) {
    .icon-wrapper i{
      font-size: 20px !important;
      margin-top: 10px;
      text-align: center;
      display: flex;
      margin-left: 4px;
      margin-right: auto;
      color: #fff !important;
    }

    .separated-border {
      display: none;
    }

    .icon-wrapper h2 {
      text-align: left;
    }

    .custom-card {
      position: absolute;
      top: 91px;
      z-index: 1;
      width: 19rem;
    }

  }

</style>
