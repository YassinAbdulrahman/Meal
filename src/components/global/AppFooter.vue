<template>
  <div id="footerapp">
    <div class="footer">
      <div class="container">
        <div class="row">
          <div class="col-lg-3">
            <div class="footer_logo">
              <img src="../../assets/companylogo.svg" alt="companylogo" />
            </div>
          </div>
          <div class="col-lg-2">
            <div class="footer_page">
              <ul>
                <h2>primary pages</h2>
                <li><a>home</a></li>
                <li><a>about us</a></li>
                <li><a>team</a></li>
                <li><a>contact us</a></li>
              </ul>
            </div>
          </div>
          <div class="col-lg-3">
            <div class="footer_page">
              <ul>
                <h2>primary pages</h2>
                <li><a>home</a></li>
                <li><a>about us</a></li>
                <li><a>team</a></li>
                <li><a>contact us</a></li>
              </ul>
            </div>
          </div>
          <div class="col-lg-4">
            <div class="footer_contact">
              <h3>SUBSCRIBE TO OUR NEWSLETTER</h3>
              <p>
                The latest news, articles, and resources, sent to your inbox
                weekly.
              </p>
              <form>
                <input type="text" placeholder="Enter your email" />
                <input type="submit" value="Subscribe" />
              </form>
            </div>
          </div>
        </div>
        <div class="footer_soical">
          <div>
            <h5>&copy 2022 MEAL Center</h5>
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
  padding: 100px 0;
  &_logo {
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  &_page {
    display: flex;
    justify-content: center;
    align-items: center;
    ul {
      h2 {
        margin-bottom: 30px;
        color: #7b88a8;
        font-size: 13px;
        line-height: 1.4;
        font-weight: 700;
        letter-spacing: 1px;
        text-transform: uppercase;
      }
      li {
        text-align: left;
        a {
          display: inline-block;
          margin-top: 4px;
          margin-bottom: 8px;
          padding-top: 8px;
          padding-right: 6px;
          padding-bottom: 8px;
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
    h3 {
      margin-bottom: 30px;
      color: #7b88a8;
      font-size: 13px;
      line-height: 1.4;
      font-weight: 700;
      letter-spacing: 1px;
      text-transform: uppercase;
    }
    p {
      margin-top: 4px;
      margin-bottom: 20px;
      padding-top: 8px;
      padding-right: 6px;
      padding-bottom: 8px;
      color: #fff;
      font-size: 16px;
      line-height: 1.3;
    }
    input[type="text"] {
      min-height: 56px;
      margin-right: 10px;
      margin-bottom: 0px;
      padding-top: 20px;
      padding-bottom: 20px;
      padding-left: 20px;
      display: inline-block;
      padding: 8px 12px;
      margin-bottom: 10px;
      font-size: 14px;
      line-height: 1.42857143;
      color: #333333;
      background-color: #ffffff;
      border: 1px solid #cccccc;
      width: 57%;
      &:focus {
        outline: none;
        border: none;
      }
    }
    input[type="submit"] {
      min-height: 56px;
      min-width: 140px;
      padding-right: 32px;
      padding-left: 32px;
      background-color: #6a35ff;
      display: inline-block;
      padding: 9px 15px;
      background-color: #3898ec;
      color: white;
      border: 0;
      line-height: inherit;
      text-decoration: none;
      cursor: pointer;
      border-radius: 0;
    }
  }
  &_soical {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 100px;
    padding-top: 32px;
    border-top: 1px solid hsla(0, 0%, 100%, 0.18);
    font-size: 15px;
    h5{
        color: #7b88a8;
        font-size: 18px ;
    }
    &_subsocial {
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