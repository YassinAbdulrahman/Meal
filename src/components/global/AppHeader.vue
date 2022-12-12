<template>
  <div class="header">
    <nav class="navbar navbar-expand-lg">
      <div class="container">
        <router-link to="/">
          <a class="navbar-brand">
            <img src="../../assets/MEAL_Center_Logo.png" alt="logo" />
          </a>
        </router-link>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav m-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <router-link to="/" exact
                ><a class="nav-link active" aria-current="page"
                  >Home</a
                ></router-link
              >
            </li>
            <li class="nav-item">
              <router-link to="/about"
                ><a class="nav-link" href="#">About</a></router-link
              >
            </li>
            <li class="nav-item">
              <router-link to="/about"
                ><a class="nav-link" href="#">Contact us</a></router-link
              >
            </li>
            <li class="nav-item">
              <router-link to="/about"
                ><a class="nav-link" href="#">Contact us</a></router-link
              >
            </li>
          </ul>
          <a class="bottom" href="#">get started</a>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "appheader",
};
</script>

<style lang="scss" scoped>
// start header
.header {
  font-family: DMSans-R;
  background-color: #f8faff;
  & .navbar {
    & .navbar-brand {
      & img {
        width: 250px;
      }
    }
    & .navbar-nav {
      & .nav-item {
        font-family: DMSans-M;
        & a {
          font-size: 16px;
          padding-right: 22px;
          padding-left: 22px;
          font-weight: 500;
          letter-spacing: -0.01em;
          &:hover {
            color: #6a35ff;
          }
        }
      }
    }
    & .bottom {
      display: inline-block;
      background: #6a35ff;
      color: #fff;
      min-height: 52px;
      padding-right: 30px;
      padding-left: 30px;
      display: grid;
      place-items: center;
      text-transform: capitalize;
      transition: box-shadow 300ms ease, background-color 300ms ease;
      text-transform: capitalize;
      &:hover {
        background-color: #5a27e7;
        box-shadow: 8px 8px 20px 0 rgb(106 53 255 / 32%);
      }
    }
  }
}
</style>