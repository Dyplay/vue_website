<!-- Where the HTML is provided -->

<template>
  <div id="app">
   <Navv/>

    <div class="auth-wrapper">
      <div class="auth-inner">
          <Loginn />
      </div>
    </div>
  </div>
</template>

<!-- The Logic of Javascript -->

<script>
import nav from './components/nav.vue'
// import home from './components/home.vue'
import login from './components/login.vue'

export default {
  name: 'App', 
    components: {
      'Navv': nav,
//      'Homee': home,
      'Loginn': login
    }
}
</script>

<!-- Style css where the css stylehseet is provided -->

<style>
    @import url('https://fonts.googleapis.com/css?family=Fira+Sans:400,500,600,700,800');

    * {
      box-sizing: border-box;
    }

    body {
      background: #1c8ef9 !important;
      min-height: 100vh;
      display: flex;
      font-weight: 400;
      font-family: 'Fira Sans', sans-serif;
    }

    h1, h2, h3, h4, h5, h6, label, span {
      font-weight: 500;
      font-family: 'Fira Sans', sans-serif;
    }

    body, html, #app, #root, .auth-wrapper {
        width: 100%;
        height: 100%;
    }


    #app {
        text-align: center;
    }

    .navbar-light {
      background-color: #ffffff;
    }


    .auth-wrapper {
      display: flex;
      justify-content: center;
      flex-direction: column;
      text-align: left;
    }


    .auth-inner {
      width: 405px;
      margin: auto;
      background: #ffffff;
      box-shadow: 0px 14px 80px rgba(34, 35, 58, 0.2);
      padding: 40px 55px 45px 55px;
      border-radius: 20px;
    }


    .auth-wrapper h3 {
      text-align: center;
      margin: 0;
      line-height: 1;
      padding-bottom: 20px;
    }


    .custom-control-label {
      font-weight: 400;
    }

    .forgot-password,
    .forgot-password a {
      text-align: right;
      font-size: 13px;
      padding-top: 10px;
      color: #7f7d7d;
      margin: 0;
    }

    .forgot-password a {
      color: #167bff;
    }

</style>
