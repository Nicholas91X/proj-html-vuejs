<template>
    <section>
        <div id="hero-text-area">
            <h1>Ready <span>Team</span></h1>
            <p>No matter what your company needs, we will be ready to assist you in the best possible way.</p>
            <div class="info-buttons">
                <button class="first-type">Get in Touch</button>
                <button class="second-type">Read More</button>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Hero"
}
</script>

<style lang="scss" scoped>
@import '../../assets/variables.scss';
    section {
        height: 550px;
        background-image: url(../../assets/img/bg-parallax.png);
        background-position: center;
        background-position-y: -60px;
        background-size: 200%;
        background-repeat: no-repeat;
        position: relative;
        #hero-text-area {
            width: 35%;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            text-align: center;
            h1 {
                font-size: 60px;
                margin-bottom: 20px;
                span {
                    padding: 3px 8px;
                    color: $elm;
                    background-color: rgba(#52bbba, $alpha: .25);
                }
            }
            p {
                margin-bottom: 30px;
                font-size: 1rem;
            }
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
                color: $elm;
                background-color: white;
                border: 1px solid $elm;
                }
            }
        }
</style>