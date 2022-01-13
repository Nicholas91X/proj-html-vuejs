<template>
  <section>
      <div class="container">
            <h5>Our Business Area</h5>
            <h2>Excellence in <span>Services</span></h2>
            <div class="text-area">
                <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowned professionals. These are some options that you can hire.</p>
                <button class="first-type">See All</button>
            </div>
            <div class="cards-area">
                <CardServices v-for="(card, index) in services" :key="index" :info="card"/>
            </div>
            <div class="bullets">
                <img src="../../assets/img/bullets.png" alt="">
            </div>
      </div>
  </section>
</template>

<script>
import CardServices from "../commons/CardServices.vue";
export default {
    name: "BusinessArea",
    components: {
        CardServices
    },
    data() {
        return {
            services: [
                {
                    "img": "../../assets/img/svg-1.svg" ,
                    "title": "Audit and Assurance" ,
                    "text": "Lorem, ipsum dolor sit amet consectetur adipisicing elit."
                },
                {
                    "img": "../../assets/img/svg-1.svg" ,
                    "title": "Financial Advisory" ,
                    "text": "Lorem, ipsum dolor sit amet consectetur adipisicing elit."
                },
                {
                    "img": "../../assets/img/svg-1.svg" ,
                    "title": "Analitics and M&A" ,
                    "text": "Lorem, ipsum dolor sit amet consectetur adipisicing elit."
                },
                {
                    "img": "../../assets/img/svg-1.svg" ,
                    "title": "Middle Marketing" ,
                    "text": "Lorem, ipsum dolor sit amet consectetur adipisicing elit."
                },
                {
                    "img": "../../assets/img/svg-1.svg" ,
                    "title": "Legal Consulting" ,
                    "text": "Lorem, ipsum dolor sit amet consectetur adipisicing elit."
                },
                {
                    "img": "../../assets/img/svg-1.svg" ,
                    "title": "Regulatory Risk" ,
                    "text": "Lorem, ipsum dolor sit amet consectetur adipisicing elit."
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/variables.scss';

section {
    background-color: $gray-nurse;
    .container {
        width: 60%;
        margin: 0 auto;
        padding: 50px 0;
        position: relative;
        h5 {
            font-size: .5rem;
            color: $elm;
            text-transform: uppercase;
            font-weight: 900;
        }
        h2 {
            font-size: 40px;
            span {
                padding: 3px 8px;
                color: $elm;
                background-color: rgba(#52bbba, $alpha: .25);
            }
        }
        .text-area {
            display: flex;
            justify-content: space-between;
            align-items: center;
            p {
                width: 75%;
                font-size: .75rem;
            }
            button {
                width: 75px;
                height: 30px;
                margin: 0 10px;
                text-transform: uppercase;
                border-radius: 5px;
                box-shadow: none;
            }
            .first-type {
                color: white;
                background-color: $elm;
            }
        }
        .cards-area {
            display: flex;
            flex-wrap: wrap;
            margin-top: 20px;
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