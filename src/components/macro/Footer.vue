<template>
  <footer>
    <div class="container-top">
      <div class="container">
        <div class="info">
          <img src="../../assets/img/logo.png" alt="Logo">
          <p>A Functional HTML Template for Corporate and Businesses</p>
          <ul>
            <li>
                <div class="icons"><i class="fas fa-phone-alt"></i></div>
                +1 (305) 1234-5678
            </li>
            <li>
                <div class="icons"><i class="fas fa-envelope"></i></div>
                hello@example.com
            </li>
            <li>
                <div class="icons"><i class="fas fa-map-marker-alt"></i></div>
                Main Avenue, 987
            </li>
            <li>
                <button class="first-type">Get in Touch</button>
            </li>
          </ul>
        </div>
        <div class="about">
          <h4>About</h4>
          <ul>
            <li>> The Company</li>
            <li>> Institutional</li>
            <li>> Social and Events</li>
            <li>> Innovation</li>
            <li>> Environment</li>
            <li>> Technology</li>
          </ul>
        </div>
        <div class="services">
          <h4>Services</h4>
          <ul>
            <li>> Audit & Assurance</li>
            <li>> Financial Advisory</li>
            <li>> Analitics and M&A</li>
            <li>> Middle Marketing</li>
            <li>> Legal Consulting</li>
            <li>> Regulatory Risk</li>
          </ul>
        </div>
        <div class="support">
          <h4>Support</h4>
          <ul>
            <li>> Responsibility</li>
            <li>> Terms of Use</li>
            <li>> About Cookies</li>
            <li>> Privacy Policy</li>
            <li>> Accessibility</li>
            <li>> Information</li>
          </ul>
        </div>
      </div>
    </div>
    <div class="container-bottom">
      <div class="container">
        <div>Enjoy the low price. We are tracking any intention of piracy.</div>
        <div>2020 NEXGEN is Proudly Powered by <span>Codings</span></div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style lang="scss" scoped>
@import '../../assets/variables.scss';
.container {
    width: 60%;
    margin: 0 auto;
    display: flex;
}
.container-top {
  background-color: $woodsmoke;
  padding: 50px 0;
  .info,
  .about,
  .services,
  .support {
    width: calc(100% / 4);
    margin-right: 15px;
    ul {
      list-style: none;
      padding: 0;
      li {    
      font-size: 12px;
      color: $pumice;
      margin-bottom: 10px;
      }
    }
    h4 {
      color: white;
      font-size: 18px;
    }
  }
  .about,
  .services,
  .support {
    padding: 0 20px;
    border-radius: 5px;
    background-color: rgba($pumice, $alpha: .1);
    font-weight: 900;
  }
  .info {
    img {
      width: 100%;
    }
    p {
      color: $pumice;
      font-size: 12px;
      margin-bottom: 20px;
    }
    ul {
      list-style: none;
      padding: 0;
      li {
        display: flex;
        color: $pumice;
        margin-bottom: 10px;
        font-size: 12px;
        div.icons {
          margin-right: 10px;
        }
        button {
          margin-top: 15px;
          padding: .4rem .6rem;
          text-transform: uppercase;
          border-radius: 5px;
          box-shadow: none;
        }
        .first-type {
          color: white;
          background-color: $woodsmoke;
          border: 1px solid $elm;
        }
      }
    }
  }
}
.container-bottom {
  height: 50px;
  background-color: black;
  display: flex;
  align-items: center;
  .container {
    width: 60%;
    color: $pumice;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    span {
      color: $elm;
    }
  }
}

</style>