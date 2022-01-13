<template>
  <section>
      <div id="results">
          <div class="container">
                <div class="title">
                    <h5>What are we doing</h5>
                    <h2><span>Results</span> in Numbers</h2>
                </div>
                <div class="numbers">
                    <ul>
                        <li><span>128</span>Certifications</li>
                        <li><span>230</span>Employees</li>
                        <li><span>517</span>Customers</li>
                        <li><span>94</span>Countries Served</li>
                    </ul>
                </div>
          </div>
      </div>
      <div id="partners">
          <div class="container">
              <ul>
                  <li><img src="../../assets/img/logo-1.png"></li>
                  <li><img src="../../assets/img/logo-2.png"></li>
                  <li><img src="../../assets/img/logo-3.png"></li>
                  <li><img src="../../assets/img/logo-4.png"></li>
                  <li><img src="../../assets/img/logo-5.png"></li>
                  <li><img src="../../assets/img/logo-4.png"></li>
              </ul>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name: "Results"
}
</script>

<style lang="scss" scoped>
@import '../../assets/variables.scss';

#results {
    width: 100%;
    height: 320px;
    background-image: url(../../assets/img/bg-7.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    background-position-y: 50%;
}
#partners {
    width: 100%;
    background-color: $woodsmoke;
    ul {
        display: flex;
        li {
            margin: 20px;
            img {
                width: 100%;
                filter: invert(.7);
            }
        }
    }
}
.container {
    width: 60%;
    margin: 0 auto;
    padding: 40px 20px;
    .title {
        text-align: center;
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
    }
    .numbers {
        margin-top: 50px;
        ul {
            display: flex;
            justify-content: space-around;
            list-style: none;
            li {
                display: flex;
                flex-direction: column;
                align-items: center;
                color: white;
                font-size: 15px;
                span {
                    color: $elm;
                    font-size: 24px;
                    font-weight: 900;
                    margin-bottom: 10px;
                }
            }
        }
    }
}
</style>