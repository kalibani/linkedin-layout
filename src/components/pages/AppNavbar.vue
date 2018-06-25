<template>
  <b-navbar toggleable="md" type="dark" variant="dark">
    <b-container>
      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
        <b-navbar-brand href="#">
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c9/Linkedin.svg/2000px-Linkedin.svg.png" alt="Responsive image" width="38" height="38">
        </b-navbar-brand>

      <b-collapse is-nav id="nav_collapse">
        <b-nav-form>
          <b-input-group>
            <b-form-input></b-form-input>
            <b-button variant="dark" slot="append">
              <i class="fas fa-search"></i>
            </b-button>
          </b-input-group>
        </b-nav-form>
        <b-navbar-nav>
          <b-nav-item class="active">
            <div class="icon-wrapper">
              <i class="fas fa-home"></i>
              <h1>Home</h1>
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
              <b-img src="https://www.konsula.com/myassets/img/photo/chris.jpg" rounded="circle" width="24" height="24" blank-color="#777" alt="img" class="m-1" />
              <h2>Me</h2>
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
      isShow: false
    }
  },
  methods: {
    showIcon () {
      this.isShow = true
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
    margin-top: 7px !important;
    text-align: center;
    display: block;
    margin-left: auto !important;
    margin-right: auto !important;
    color: #fff !important;
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
    padding-right: 5rem;
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

    .nav-item {
      padding-left: 0px !important;
      padding-right: 0px !important;
    }

  }
</style>
