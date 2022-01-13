<template>
  <section>
      <div class="container">
          <div class="message">
                <h5>Send a Message</h5>
                <h2>Get in <span>Touch</span></h2>
                <p>We will respond to your message as soon as possible</p>
                <div class="form">
                    <form action="">
                       <input id="name" type="text" placeholder="Name">
                       <input id="e-mail" type="text" placeholder="E-mail">
                       <input id="phone" type="text" placeholder="Phone">
                       <select name="more-info" id="more-info"></select>
                       <input type="text" name="message" id="message" placeholder="Message">
                       <button class="first-type">Send</button> 
                    </form>
                </div>
          </div>
          <div class="contact">
              <div class="contact-info">
                  <h4>Example Inc.</h4>
                  <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                  <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
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
                        <button class="second-type">View Map</button>
                    </li>
                  </ul>
              </div>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name: "SendMessage"
}
</script>

<style lang="scss" scoped>
@import '../../assets/variables.scss';
.container {
    width: 60%;
    margin: 0 auto;
    display: flex;
    padding: 50px;
    .message {
        width: 70%;
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
          p {
              font-size: 12px;
          }
          form {
            margin-top: 20px;
            #name, 
            #e-mail,
            #phone {
                width: 240px;
                margin-bottom: 15px;
                margin-right: 10px;
                padding: 10px;
                background-color: lightgrey;
                border: none;
              }
            #more-info {
                width: 260px;
                margin-bottom: 15px;
                margin-right: 10px;
                padding: 8px;
                background-color: lightgrey;
                border: none;
              }
            #message {
                width: 510px;
                height: 100px;
                background-color: lightgrey;
                border: none;
                padding: 10px;
                margin-bottom: 15px;
            }
            button {
                padding: .4rem .8rem;
                text-transform: uppercase;
                border-radius: 5px;
                box-shadow: none;
            }
            .first-type {
                color: white;
                background-color: $elm;
            }
          }
    }
    .contact {
        width: 30%;
        .contact-info {
            padding: 0 15px;
            h4 {
                font-size: 18px;
            }
            p {
                font-size: 12px;
            }
            ul {
                list-style: none;
                padding: 0;
                margin-top: 20px;
                li {
                    font-size: 15px;
                    display: flex;
                    align-items:baseline;
                    color: $elm;;
                    div.icons {
                        display: flex;
                        justify-content: center;
                        align-items: center;
                        width: 30px;
                        height: 30px;
                        border-radius: 50%;
                        background-color: rgba(#52bbba, $alpha: .25);
                        margin-right: 8px;
                        margin-bottom: 10px;
                    }
                    button {
                        padding: .4rem .8rem;
                        text-transform: uppercase;
                        border-radius: 5px;
                        box-shadow: none;
                        margin-top: 15px;
                    }
                    .second-type {
                        color: $elm;
                        background-color: white;
                        border: 1px solid $elm;
                    }
                }
            }
        }
    }
}
</style>