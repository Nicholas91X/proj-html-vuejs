<template>
  <section>
    <div class="container">
            <div class="container__info">
              <div class="sub-container">
                <h5>About the network</h5>
                <h2><span>The</span> Company</h2>
                <div class="text-area">
                  <p>For twelve years we have been providing audit and warranty, financial advice, taxes and related services to select clients.</p>
                </div>
                <div class="network-info">
                  <div class="network-card">
                    <h4>Tradition</h4>
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
                  <div class="network-card">
                    <h4>Security</h4>
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
                  <div class="network-card">
                    <h4>Certificate</h4>
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
                  <div class="network-card">
                    <h4>Expertise</h4>
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
                </div>
                <div class="network-buttons">
                  <button class="first-type">Get in Touch</button>
                  <button class="second-type">Read More</button>
                </div>
              </div>
            </div>
            <div class="container__image">
              <img src="../../assets/img/about-4.jpg" alt="">
            </div>
            <div class="bullets">
                <img src="../../assets/img/bullets.png" alt="">
            </div>
    </div>
  </section>
</template>

<script>
export default {
    name: "AboutArea"
}
</script>

<style lang="scss" scoped>
@import '../../assets/variables.scss';

section {
    background-color: black;
    .container {
        width: 100%;
        position: relative;
        display: flex;
        &__info {
          width: 50%;
          display: flex;
          justify-content: flex-end;
          .sub-container {
            width: 60%;
            padding: 50px 20px;
          }
          h5 {
            font-size: .5rem;
            color: $elm;
            text-transform: uppercase;
            font-weight: 900;
          }
          h2 {
            font-size: 40px;
            color: white;
            span {
                padding: 3px 8px;
                color: white;
                background-color: rgba(#52bbba, $alpha: .25);
            }
          }
          .text-area {
            p {
                font-size: .75rem;
                color: $pumice;
            }
          }
          .network-info {
              display: flex;
              flex-wrap: wrap;
          }
          .network-card {
              width: calc(100% / 2 - 30px);
              margin: 10px;
                h4 {
                  color: white;
                  font-size: 18px;
                }
                p {
                  color: $pumice;
                }
          }
          .network-buttons {
            margin-top: 30px;
            button {
                margin: 0 10px;
                padding: .4rem .8rem;
                text-transform: uppercase;
                border-radius: 5px;
                box-shadow: none;
                }
            .first-type {
                color: white;
                background-color: $elm;
                }
            .second-type {
                color: white;
                background-color: black;
                border: 1px solid $elm;
                }
          }
        }
        &__image {
          width: 50%;
          padding: 0;
          img {
            width: 100%;
          }
        }
        .bullets {
            position: absolute;
            left: 50%;
            transform: translateX(-50%);
            bottom: -20px;
            width: 100px;
            height: 40px;
            overflow: hidden;
            z-index: 9999;
            img {
                width: 100%;
            }
        }
    }
}
</style>