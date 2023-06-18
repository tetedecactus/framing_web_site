<template>
    <!-- <Layout>
      <section class="contact" id="contact">
        <Map />
        <div class="container mx-auto">
          <div class="contact-container">
            <div class="flex justify-center">
              <div class="w-3/4 md:w-9/12 lg:w-9/12 xl:w-9/12">
                <div class="contact-card">
                  <div>
                    <h2><span>Contact Us</span></h2>
                  </div>
                  <div class="item flex justify-end md:flex-row flex-wrap">
                    <img class="check" src="@/assets/images/phone_icon.png" width="25" height="25" alt="phone-logo" />
                    <p>1-780-271-6505</p>
                  </div>
                  <div class="item flex justify-end md:flex-row flex-wrap">
                    <img class="check" src="@/assets/images/position_icon.png" width="25" height="25" alt="position-logo" />
                    <p>9151 Shaw Way, Edmonton, Alberta</p>
                  </div>
                  <div class="item flex justify-end md:flex-row flex-wrap">
                    <img class="check" src="@/assets/images/mail_icon.png" width="25" height="25" alt="mail-logo" />
                    <p class="email"><a href="mailto:EastClawConstructionInc@hotmail.com">EastClawConstructionInc@hotmail.com</a></p>
                  </div>
                </div>
              </div>
              <div class="lg:w-9/12 md:w-9/12 sm:w-full">
                <TrackVisibility>
                  {({ isVisible }) =>
                    <div class={isVisible ? "animate__animated animate__fadeIn" : ""}>
                      <form ref="form" @submit="sendEmail">
                        <div class="flex justify-center">
                          <div class="px-1 w-10/12 md:w-6/12">
                            <input type="text" name="user_name" placeholder="First Name" required class="w-full" />
                          </div>
                          <div class="px-1 w-10/12 md:w-6/12">
                            <input type="text" name="user_name" placeholder="Last Name" required class="w-full" />
                          </div>
                          <div class="px-1 w-10/12 md:w-6/12">
                            <input type="email" name="user_email" placeholder="Email Address" required class="w-full" />
                          </div>
                          <div class="px-1 w-10/12 md:w-6/12">
                            <input type="tel" name="phone-number" placeholder="Phone No." required class="w-full" />
                          </div>
                          <div class="px-1 w-full">
                            <textarea rows="6" name="message" placeholder="Message" required class="w-full"></textarea>
                            <button type="submit" class="btn"><span>Send</span></button>
                            <ToastContainer />
                          </div>
                        </div>
                      </form>
                    </div>
                  }
                </TrackVisibility>
              </div>
            </div>
          </div>
        </div>
      </section>
    </Layout> -->
  </template>
  
  <!-- <script>
  import { ToastContainer, toast } from 'react-toastify';
  import 'react-toastify/dist/ReactToastify.css';
  import emailjs from '@emailjs/browser';
  import TrackVisibility from 'react-on-screen';
  import Layout
   -->