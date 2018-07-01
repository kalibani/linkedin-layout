<template>
<div class="container">
  <div class="row">
    <div class="col-md-4 col-lg-3 col-sm-12 col-xs-12">
      <div class="card hovercard">
          <div class="cardheader"></div>
          <div class="avatar">
              <img alt="" src="https://media.licdn.com/dms/image/C5603AQFqH8-QoYdjDQ/profile-displayphoto-shrink_800_800/0?e=1535587200&v=beta&t=pQeXdcVKuXVHPkXBLiFr6Ha0OKcy-jcMHyWfBnEraCw">
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
    <div class="col-md-8 col-lg-5 col-sm-12 col-xs-12">
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
            <img src="https://media.licdn.com/dms/image/C4E03AQHuIxwXZ_c_vA/profile-displayphoto-shrink_800_800/0?e=1535587200&v=beta&t=3kzlTL3vJxJugiF-shNXfCBPT6uZo6urZSGkkX77luQ" class="img-avatar" alt="Avatar image">
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
          <div class="post-area-like">
            1 Like
          </div>
          <hr>
          <div class="post-area-action">
            <div class="action">
              <i class="far fa-thumbs-up"></i>  <span>Like</span>
            </div>
            <div class="action">
              <i class="far fa-comment-alt"></i>  <span>Comment</span>
            </div>
            <div class="action">
              <i class="fas fa-share"></i>  <span>Share</span>
            </div>
          </div>
        </div>
      </div>
    </div>
    </div>
    <div class="offset-md-4 offset-sm-0 offset-lg-0 offset-xs-0 col-md-8 col-lg-4 col-sm-12 col-xs-12">
      <div class="post-area">
        <div class="card">
          <div class="card-body">
            <div class="suggestion-area">
              Add to your feed
            </div>
            <div class="post-area-profile">
              <img src="https://media.licdn.com/dms/image/C4E03AQFlmLGSxfTBlg/profile-displayphoto-shrink_800_800/0?e=1535587200&v=beta&t=UbTW3eAZLM5QIqBoT3Fq4q_kxtYgjtGfom8W0rBYkc8" class="img-avatar" alt="Avatar image">
              <div class="suggestion-profile">
                <h5>Max Levchin</h5>
                <h6>Co-Founder & CEO at Affirm, inc</h6>
              </div>
              <button type="button" class="btn btn-primary custom-secondary"><i class="fas fa-plus"></i><span>Follow</span></button>
            </div>
            <div class="post-area-profile">
              <img src="https://jurnalapps.co.id/assets/img/apps/1471509137_shopee.png" class="img-avatar" alt="Avatar image">
              <div class="suggestion-profile">
                <h5>Shopee</h5>
                <h6>Compan . Internet</h6>
              </div>
              <button type="button" class="btn btn-primary custom-secondary"><i class="fas fa-plus"></i><span>Follow</span></button>
            </div>
            <div class="post-area-profile">
              <img src="https://cdn-images-1.medium.com/max/620/1*y5xr0iGgkCctshouAs1IwA.jpeg" class="img-avatar" alt="Avatar image">
              <div class="suggestion-profile">
                <h5>Software Engineering</h5>
                <h6>Topic</h6>
              </div>
              <button type="button" class="btn btn-primary custom-secondary"><i class="fas fa-plus"></i><span>Follow</span></button>
            </div>
            <div class="suggestion-area">
              <a href="#">View all recommendations</a>
            </div>
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
  background-image: url("https://media.licdn.com/dms/image/C5616AQF3F_eW47slQQ/profile-displaybackgroundimage-shrink_350_1400/0?e=1535587200&v=beta&t=bDJGnb-ryeHT8Ov6kIEEoehOAk-Z0IqcM-Wl31yofhw");
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

.post-area-like {
  font-size: 12px;
  color: #737373;
  padding-top: 5px;
}

.post-area-action {
  display: inline-block;
}

.post-area-action .action {
  display: inline-block;
  font-size: 14px;
  font-weight: bold;
  color: #737373;
  margin-right: 10px;
}

.suggestion-area {
  margin-bottom: 10px;
}

.suggestion-profile {
  display: inline-block;
}

.suggestion-profile h5 {
  padding-top: 5px;
  font-size: 12px;
  line-height: 0.9;
  font-weight: bold;
}

.suggestion-profile h6 {
  max-width: 105px;
  color: #737373;
  font-size: 12px;
}

.suggestion-area a {
  color: #0073b1;
  font-weight: bold;
}

.custom-secondary {
  float: right;
  background-color: #fff;
  color: rgba(0,0,0,.6);
  height: 32px;
  font-size: 12px;
  padding-top: 4px;
  font-weight: bold;
  border: 1px solid rgba(0,0,0,.6) !important;
}

.custom-secondary i {
  margin-right: 10px;
}

/*
  ##Device = Mobile(landscape)
  ##Screen = B/w 320px to 480px
*/

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

/* ----------- iPad Pro ----------- */
/* Portrait and Landscape */
@media only screen
  and (min-device-width: 1024px)
  and (max-device-width: 1366px)
  and (-webkit-min-device-pixel-ratio: 1.5) {

    .custom-secondary {
      float: right;
      background-color: #fff;
      color: rgba(0,0,0,.6);
      height: 32px;
      padding-top: 4px;
      font-weight: bold;
      border: 1px solid rgba(0,0,0,.6) !important;
    }

    .custom-secondary i {
      margin-right: 0px;
    }

    .custom-secondary span {
      display: none;
    }
}

</style>
