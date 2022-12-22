<template>
  <div id="footerapp">
    <div class="footer">
      <div class="container">
        <div class="row">
          <div class="col-lg-3">
            <div class="footer_logo">
              <img src="../../assets/mealcenterlogo.svg" alt="companylogo" />
            </div>
          </div>
          <div class="col-lg-3">
            <div class="footer_page">
              <ul>
                <h2>Primary Pages</h2>
                <li><a>Home</a></li>
                <li><a>About us</a></li>
                <li><a>Services</a></li>
              </ul>
            </div>
          </div>
          <div class="col-lg-3">
            <div class="footer_page">
              <ul>
                <h2>Pages</h2>
                <li><a>protiofilio</a></li>
                <li><a>Team</a></li>
                <li><a>Learning Zone</a></li>
                <li><a>Contact us</a></li>
              </ul>
            </div>
          </div>
          <div class="col-lg-3">
            <div class="footer_contact">
              <h3></h3>
               <ul>
                <h2>Contact us:</h2>
                <li><img src="../../assets/email.svg" alt="email icon"> <a href="mailto:info@mealcenter.org">info@mealcenter.org</a></li>
                <li><img src="../../assets/Phone.svg" alt="phone icon"><a href="Tel:+967774354278">+967 774354278</a></li>
              </ul>
            </div>
          </div>
        </div>
        <div class="footer_soical">
          <div>
            <h5>&copy; 2022 MEAL Center</h5>
          </div>
          <div class="footer_soical_subsocial">
            <ul>
              <li>
                <a href="#"
                  ><img
                    src="../../assets/footer_socialmedia_one.svg"
                    alt="footer_socialmedia"
                /></a>
              </li>
              <li>
                <a href="#"
                  ><img
                    src="../../assets/footer_facebook.svg"
                    alt="footer_facebook"
                /></a>
              </li>
              <li>
                <a href="#"
                  ><img
                    src="../../assets/footerinstagram.svg"
                    alt="footerinstagram"
                /></a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.footer {
  background-color: #182135;
  font-family: DMSans-R;
  padding: 50px 0 15px 0;
  &_logo {
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: flex-start;
    img{
      width: 300px;
    }
  }
  &_page {
    display: flex;
    justify-content: center;
    align-items: center;
    ul {
      h2 {
        margin-bottom: 10.2px;
        color: #2680C2;
        font-size: 18px;
        line-height: 1.4;
        letter-spacing: 1px;
        text-transform: capitalize;
        text-align: left;
        font-family: DMSans-B;

      }
      li {
        text-align: left;
        a {
          display: inline-block;
          margin-top: 4px;
          margin-bottom: 12px;
          color: #fff;
          font-size: 16px;
          background-color: transparent;
          cursor: pointer;
          text-transform: capitalize;
          &:hover {
            color: #7b88a8;
          }
        }
      }
    }
  }
  &_contact {
    text-align: left;
    h2 {
      margin-bottom: 10px;
      color: #2680C2;
      font-size: 18px;
      line-height: 1.4;
      letter-spacing: 1px;
      text-transform: capitalize;
      font-family: DMSans-B;
    }
    li{
      margin-bottom: 10px;
      img{
        margin-right: 5px;
      }
      a{
        color: #EBEFFA;
      }
    }
  }
  &_soical {
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    border-top: 1px solid hsla(0, 0%, 100%, 0.18);
    font-size: 15px;
    h5{
        color: #7b88a8;
        font-size: 18px ;
    }
    &_subsocial {
      padding-top: 20px;
      ul {
        display: flex;
        justify-content: center;
        align-items: center;
        li{
           margin-right: 10px;
        }
      }
    }
  }
}
</style>