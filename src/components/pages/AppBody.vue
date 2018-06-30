<template>
<div class="container">
  <div class="row">
    <div class="col-md-4 col-lg-3 col-sm-12 col-xs-12">
      <div class="card hovercard">
          <div class="cardheader"></div>
          <div class="avatar">
              <img alt="" src="https://www.konsula.com/myassets/img/photo/chris.jpg">
          </div>
          <div class="info">
            <div class="title">
                <a target="_blank" href="">Christian Hanggra</a>
            </div>
            <div class="desc">Tech Enthusiast</div>
          </div>
          <hr>
          <div class="info">
            <div class="viewed">
                80
            </div>
            <div class="desc">Who's viewed your profile</div>
            <hr>
          </div>
          <div class="info">
            <div class="viewed">
                1,133
            </div>
            <div class="desc">Conections</div>
            <div class="desc-2">Manage Your work</div>
          </div>
          <div class="info-bottom">
            <div class="desc">
              Access exclusive tools & insights
            </div>
            <div class="desc-2">
              <i class="fas fa-square fas-box"></i>
              Free Upgrade to Premium
            </div>
            <div class="desc-2">
              <i class="fas fa-square fas-box"></i>
              Free Upgrade to Premium
            </div>
          </div>
      </div>
    </div>
    <div class="col-md-8 col-lg-6 col-sm-12 col-xs-12">
      <div class="post-area">
        <div class="card">
          <div class="card-body">
            <div class="status-area">
              Share an article, photo or idea
            </div>
            <hr>
            <div class="button-left">
              <button type="button" class="btn btn-primary btn-custom">
                <i class="far fa-edit"></i>
                Tulis artikel
              </button>
              <button type="button" class="btn btn-secondary btn-custom">
                <i class="fas fa-camera"></i>
              </button>
              <button type="button" class="btn btn-success btn-custom">
                <i class="fas fa-video"></i>
                Video
              </button>
            </div>
            <div class="button-right">
              <button type="button" class="btn btn-primary btn-custom-primary">Posting</button>
            </div>
          </div>
        </div>
      </div>
      <h2 class="status-area-border">
        <span>Sort by : <strong>Top <i class="fas fa-caret-down caret-down"></i></strong></span>
      </h2>
    <div class="post-area">
      <div class="card">
        <div class="card-body">
          <div class="post-area-profile">
            <img src="https://cdn-images-1.medium.com/max/960/1*rchGC6ySU1CEezcLEMJkzg.jpeg" class="img-avatar" alt="Avatar image">
            <div class="profile">
              <h5>Wirjadi Lorens</h5>
              <h6>Founder at OKTAGON</h6>
              <h6>1d</h6>
            </div>
          </div>
          <div class="post-area-wrapper">
            <img src="https://cdn-images-1.medium.com/max/960/1*rchGC6ySU1CEezcLEMJkzg.jpeg" class="img-fluid img-custom" alt="Responsive image">
            <div class="post-area-title">
              Artificial Intelligence ( AI ), Dari Teknologi Abstrak Hingga Jadi 'Otak' Bisnis
              <h6>daily.oktagon.co.id</h6>
            </div>
          </div>
          <hr>
          <div class="status-area">
          </div>
          <hr>
          <div class="button-left">
            <button type="button" class="btn btn-primary">Tulis artikel</button>
            <button type="button" class="btn btn-secondary">
              <i class="fas fa-camera"></i>
            </button>
            <button type="button" class="btn btn-success">Video</button>
          </div>
          <div class="button-right">
            <button type="button" class="btn btn-primary">Posting</button>
          </div>
        </div>
      </div>
    </div>
    </div>
    <div class="offset-md-4 offset-sm-0 offset-lg-0 offset-xs-0 col-md-8 col-lg-3 col-sm-12 col-xs-12">
      <div class="post-area">
        <div class="card">
          <div class="card-body">
            <div class="status-area">
              Share an article
            </div>
            <hr>
          </div>
        </div>
      </div>
    </div>

    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style scoped>
.card {
  margin: 10px 0 20px 0;
  box-sizing: border-box;
  box-shadow: 0 0 0 1px rgba(0,0,0,.15);
}

.card.hovercard {
  position: relative;
  padding-top: 0;
  overflow: hidden;
  text-align: center;
  background-color: #fff;
}

.card.hovercard .cardheader {
  background-image: url("https://www.setaswall.com/wp-content/uploads/2017/06/Linkedin-Backgrounds-18-1400-x-425.jpg");
  background-size: cover;
  height: 100px;
}

.card.hovercard .avatar {
  position: relative;
  top: -50px;
  margin-bottom: -35px;
}

.card.hovercard .avatar img {
  width: 100px;
  height: 100px;
  max-width: 100px;
  max-height: 100px;
  -webkit-border-radius: 50%;
  -moz-border-radius: 50%;
  border-radius: 50%;
  border: 5px solid rgba(255,255,255,0.5);
  background-color: #fff;
}

.card.hovercard .info {
  padding: 4px 8px 10px;
}

.card.hovercard .info .title {
  margin-bottom: 4px;
  font-size: 24px;
  line-height: 1;
  color: #000;
  vertical-align: middle;
}

a {
  color: #000;
  text-decoration: none;
}

.card.hovercard .info .desc {
  overflow: hidden;
  font-size: 12px;
  line-height: 20px;
  color: #737373;
  font-weight: bold;
}

.fas-box {
  color: #b29a53 !important;
  padding-right: 10px !important;
}

.info-bottom {
  padding: 12px 8px 12px;
  border-top: 1px solid rgba(0, 0, 0, 0.1);
  background-color: #F5F5F5;
}

.desc-2 {
  overflow: hidden;
  font-size: 13px;
  line-height: 20px;
  color: #000;
  font-weight: bold;
}

.card.hovercard .info .viewed {
  display: block;
  font-weight: 200;
  color: #0084bf;
}

.card.hovercard .bottom {
  padding: 0 20px;
  margin-bottom: 17px;
}

.post-area{
  margin: 10px 0 20px 0;
  box-sizing: border-box;
  border-radius: 4px;
  box-shadow: 0 0 0 1px rgba(0,0,0,.15);
  max-height: 100%;
  background-color: #fff;
}

.btn-custom {
  height: 32px;
  padding-top: 4px;
  border-radius: 16px;
  color: #000 !important;
  background-color: #fff !important;
  border: 1px solid #000 !important;
  box-shadow: 0 0 0 1px rgba(0,0,0,.15);
}

.btn-custom:hover {
  background-color: #F5F5F5 !important;
}

.btn-custom-primary {
  height: 32px;
  padding-top: 4px;
  font-weight: bold;
  background-color: #0073b1;
  border: 0;
}

.btn-custom-primary:hover {
  background-color: #004b7c;
}

.status-area {
  height: 75px;
  padding-top: 20px;
}

.button-left {
  float: left;
}

.button-right {
  float: right;
}

.status-area-border {
  font-size: 12px;
  color: rgba(0,0,0,.6);
  width:100%;
  text-align:right;
  border-bottom: 1px solid rgba(0,0,0,.6);
  line-height:0.1em;
  margin:10px 0 20px;
}

.status-area-border span {
  background:#F5F5F5; padding:0 10px;
}

.status-area-border strong {
  color: #000;
}

.caret-down {
  line-height: 0.1em !important;
}

.post-area-profile {
  display: inline-block;
  margin-bottom: 15px;
}

.img-avatar {
  vertical-align: top;
  width: 50px;
  height: 50px;
  border-radius: 50%;
}

.profile {
  margin-left: 7px;
  display: inline-block;
}

.profile h5 {
  font-size: 12px;
  line-height: 1;
  font-weight: bold;
}

.profile h6 {
  color: #737373;
  font-size: 12px;
  line-height: 0.9;
}

.post-area-wrapper {
  background-color: #fff;
  padding: 10px 0px;
  border: 1px solid rgba(0, 0, 0, 0.1);
  border-radius: 4px;
}

.img-custom {
  border-radius: 1px;
}

.post-area-title {
  margin: 10px 10px;
  font-weight: bold;
}

.post-area-title h6{
  font-size: 12px;
  color: #737373;
}

@media (min-width: 320px) and (max-width: 480px) {
  .btn {
    font-size: 13px;
  }
  .button-left .btn-secondary {
    float: none;
    width: 50px
  }

  .button-right {
    margin-top: 10px;
    float: right;
  }

}
</style>
