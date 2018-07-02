<template>
  <div class="container-fluid">
    <hr>
    <div class="container">
      <div class="row">
        <div class="col-12">
          <div class="logo-linkedIn">
            <h1>Linked<i class="fab fa-linkedin"></i></h1>
          </div>
        </div>
        <div class="col-lg-2 col-md-4 col-sm-6 col-xs-6">
          <div class="footer">
            About
          </div>
          <div class="footer">
            Careers
          </div>
          <div class="footer">
            Advertising
          </div>
          <div class="footer">
            Mobile
          </div>
        </div>
        <div class="col-lg-2 col-md-4 col-sm-6 col-xs-6">
          <div class="footer">
            Talent Solutions
          </div>
          <div class="footer">
            Marketing Solutions
          </div>
          <div class="footer">
            Sales Solutions
          </div>
          <div class="footer">
            Small Solutions
          </div>
        </div>
        <div class="col-lg-2 col-md-4 col-sm-4 col-xs-4">
          <div class="footer">
            Community Guidelines
          </div>
          <div class="footer">
            Privacy & Terms
          </div>
          <div class="footer">
            Send feedback
          </div>
          <div class="footer">
            Safety Center
          </div>
        </div>
        <div class="col-lg-4 col-md-8 custom-md">
          <div class="footer-right">
            <i class="far fa-question-circle"></i>
            <div class="footer-right-content">
              <h5>Questions?</h5>
              <h6>Visit our Help Center</h6>
            </div>
          </div>
          <div class="footer-right">
            <i class="fas fa-cog"></i>
            <div class="footer-right-content">
              <h5>Manage your account and privacy</h5>
              <h6>Go to your Settings</h6>
            </div>
          </div>
        </div>
        <div class="col-lg-2 col-md-4 custom-md">
          <div class="select-language">
            <h5>Select Language</h5>
            <button type="button" class="btn btn-outline-primary custom-outline" name="button">
              English (English)
              <i class="fas fa-caret-down"></i>
            </button>
          </div>
        </div>
        <div class="col-12">
          <div class="copyright">
            <h1>LinkedIn Corporation &copy; 2018</h1>
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
.container-fluid {
  padding-left: 0px !important;
  padding-right: 0px !important;
}

.logo-linkedIn h1 {
  font-size: 18px;
  font-weight: bold;
}

.logo-linkedIn i {
  color: #0084bf;
  font-size: 20px;
  vertical-align: top;
  margin-left: 2px;
}

.footer {
  cursor: pointer;
  font-weight: 600;
  color: #495D6E;
  text-align: left;
  font-size: 13px;
  line-height: 25px;
  margin-bottom: 10px;
}

.footer:hover {
  color: #0084bf;
}

.footer-right {
  display: inline-block;
  margin-bottom: 20px;
}

.footer-right i {
  vertical-align: top;
  font-size: 33px;
  margin-right: 5px;
  color: #0084bf;
}

.footer-right-content {
  display: inline-block;
}

.footer-right-content h5 {
  cursor: pointer;
  margin-top: 5px;
  font-size: 19px;
  font-weight: 600;
  color: #495D6E;
}

.footer-right-content h6 {
  cursor: pointer;
  margin-top: 5px;
  color: #737373;
}

.select-language {
  cursor: pointer;
  margin-top: 5px;
  color: #495D6E;
}

.custom-outline {
  height: 34px;
  padding-top: 5px;
  border-radius: 1px;
  font-weight: bold;
  color: #0084bf;
  border-color: #0084bf;
}

.custom-outline:hover {
  background-color: #F5F5F5 !important;
}

.copyright h1 {
  cursor: pointer;
  color: #495D6E;
  text-align: left;
  font-size: 13px;
  margin-top: 10px;
  margin-bottom: 10px;
}

/*
  ##Device = Mobile(landscape)
  ##Screen = B/w 320px to 480px
*/

@media (min-width: 320px) and (max-width: 480px) {
  .footer-right {
    display: inline-block;
    margin-bottom: 10px;
  }

  .footer-right i {
    vertical-align: top;
    font-size: 18px;
    margin-right: 5px;
    color: #0084bf;
  }
  .footer-right-content {
    display: inline-block;
  }

  .footer-right-content h5 {
    cursor: pointer;
    margin-top: 5px;
    font-size: 13px;
    font-weight: 600;
    color: #495D6E;
  }

  .footer-right-content h6 {
    cursor: pointer;
    margin-top: 5px;
    color: #737373;
    font-size: 13px;
  }

  .select-language {
    font-size: 13px;
    cursor: pointer;
    margin-top: 5px;
    color: #495D6E;
  }

  .custom-outline {
    font-size: 13px;
    height: 34px;
    padding-top: 5px;
    border-radius: 1px;
    font-weight: bold;
    color: #0084bf;
    border-color: #0084bf;
  }
}

/* ----------- iPad ----------- */
/* Portrait and Landscape */
@media only screen
  and (min-device-width: 768px)
  and (max-device-width: 1024px) {

    .custom-md {
      margin-top: 18px;
    }
}
</style>
