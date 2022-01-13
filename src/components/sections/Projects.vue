<template>
  <section>
      <div class="container">
        <div class="top">
            <h5>We do more for everyone.</h5>
            <h2>Actions & <span>Projects</span></h2>
        </div>
        <nav>
            <ul>
                <li>All</li>
                <li>Institutional</li>
                <li>Social</li>
                <li>Events</li>
                <li>Innovation</li>
                <li>Environment</li>
                <li>Technology</li>
            </ul>
        </nav>
        <div class="cards-project">
            <CardProject v-for="(card, index) in projects" :key="index" :info="card"/>
        </div>
      </div>
  </section>
</template>

<script>
import CardProject from "../commons/CardProject.vue";
export default {
    name: "Projects",
    components: {
        CardProject
    },
    data() {
        return {
            projects: [
                {
                    img: "../../assets/img/project-1.jpg",
                    title: "Academic Professional program in social media",
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                },
                {
                    img: "../../assets/img/project-2.jpg",
                    title: "President's speech at the annual meeting",
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                },
                {
                    img: "../../assets/img/project-3.jpg",
                    title: "International business trip in Shanghai",
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                },
                {
                    img: "../../assets/img/project-4.jpg",
                    title: "Technology workshop with educational team",
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                },
                {
                    img: "../../assets/img/project-5.jpg",
                    title: "Donation of clothes and food to the partner NGO",
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                },
                {
                    img: "../../assets/img/project-6.jpg",
                    title: "Confraternization of the procurement team",
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/variables.scss';

.container {
    width: 60%;
    margin: 0 auto 50px;
    .top {
        text-align: center;
        margin-top: 70px;
        h5 {
            font-size: .5rem;
            color: $elm;
            text-transform: uppercase;
            font-weight: 900;
          }
          h2 {
            font-size: 40px;
            color: black;
            span {
                padding: 3px 8px;
                color: $elm;
                background-color: rgba(#52bbba, $alpha: .25);
            }
          }
    }
    nav ul {
        list-style: none;
        display: flex;
        justify-content: center;
        li {
            padding: 5px;
            margin: 10px;
            text-transform: uppercase;
        }
        li:hover {
            background-color: rgba(#52bbba, $alpha: .25);
        }
    }
    .cards-project {
        display: flex;
        flex-wrap: wrap;
    }
}
</style>