<template>
  <header>
      <div id="header-top">
            <div id="header-top__left">
                <i class="fas fa-clock"></i>
                <div id="opening-time">Open Hours: Mon - Sat - 9:00 - 18:00</div>
            </div>
            <div id="header-top__right">
                <div id="phone-number">
                    <i class="fas fa-phone-alt icons"></i>
                    +1 (305) 1234-5678
                </div>
                <div id="mail">
                    <i class="fas fa-envelope icons"></i>
                    hello@example.com
                </div>
                <div id="social">
                    <ul>
                        <li><i class="fab fa-facebook"></i></li>
                        <li><i class="fab fa-twitter"></i></li>
                        <li><i class="fab fa-linkedin"></i></li>
                    </ul>
                </div>
            </div>
      </div>
      <div id="header-bottom">
        <div id="logo">
            <img src="../../assets/img/logo.png" alt="">
        </div>
        <div id="navbar">
            <nav>
                <ul>
                    <li>Home</li>
                    <li>Services</li>
                    <li>About</li>
                    <li>Projects</li>
                    <li>Results</li>
                    <li><button>Get in Touch</button></li>
                </ul>
            </nav>
        </div>
      </div>
      <Hero/>
  </header>
</template>

<script>
import Hero from "../sections/Hero.vue";
export default {
    name: "Header",
    components: {
        Hero
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/global.scss';
@import '../../assets/variables.scss';
#header-top {
    width: 100%;
    background-color: $woodsmoke;
    display: flex;
    padding: 10px;
    &__left {
        justify-content: center;
        #opening-time {
            margin-left: .25rem;
        }
    }
    &__right {
        justify-content: center;
        #phone-number {
            .icons {
                vertical-align: top;
                margin-right: .25rem;
            }
        }
        #mail {
            margin: 0 1.25rem;
            .icons {
                vertical-align: top;
                margin-right: .25rem;
            }
        }
        #social {
            ul {
                display: flex;
                justify-content: center;
                li:nth-child(2) {
                    margin: 0 1.25rem;
                }
            }
        }
    }
    &__left,
    &__right {
        width: 50%;
        color: $pumice;
        display: flex;
    }

}
#header-bottom {
    width: 100%;
    position: absolute;
    padding: 1rem;
    display: flex;
    justify-content: center;
    align-items: center;
        #logo {
            width: 40%;
            text-align: center;
        }
        #navbar {
            width: 60%;
        }
        img {
            width: 30%;
            margin-left: 100px;
        }
        nav ul {
            display: flex;
            justify-content: center;
            align-items: center;
            margin-right: 150px;
            li {
                text-transform: uppercase;
                margin: 0 .75rem;
            }
        }
}
</style>