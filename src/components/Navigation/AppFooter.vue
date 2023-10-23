<template>
    <div>
      <div>
        <footer class="tw-bg-dark-100 tw-px-6 tw-py-12 tw-mt-8">
          <div class="">
            <div class="tw-grid lg:tw-grid-cols-4 md:tw-grid-cols-2 tw-grid-cols-1 tw-gap-5">
              <div class="">
                <span class="tw-text-white tw-text-[80px] tw-font-bold tw-sepia">fooder</span>
              </div>
  
              <div class="">
                <h4 class="tw-text-primary tw-text-sm tw-underline">COMPANY</h4>
                <ul class="list-unstlyed">
                  <!-- <li><router-link to="/privacy-policy"> About Us</router-link></li> -->
                  <li>
                    <router-link to="/">
                      Privacy Policy</router-link
                    >
                  </li>
                  <li>
                    <router-link to="/"
                      >Terms and Conditions</router-link
                    >
                  </li>
                  <li><router-link to="/">Careers</router-link></li>
                  <li><router-link to="/">Contact Us</router-link></li>
                </ul>
              </div>
  
              <div class="">
                <h4 class="tw-text-primary tw-text-sm tw-underline">MY ACCOUNT</h4>
                <ul class="list-unstlyed">
                  <li><router-link to="/">View Cart</router-link></li>
                  <li><router-link to="/">Sign In</router-link></li>
                  <li>
                    <router-link to="/">Sign Up</router-link>
                  </li>
                </ul>
              </div>
  
              <div class="">
                <h4 class="tw-text-primary tw-text-sm tw-underline">CUSTOMER SERVICE</h4>
  
                <p class="tw-text-gray-400 tw-mb-0 tw-text-sm">Got Question? Email us</p>
                <h4 class="tw-text-white tw-text-sm ">
                  <a href="mail-to:support@e-sharzy.com" class="tw-text-white tw-no-underline"
                    >support@fooder.com</a
                  >
                </h4>
                <div class="mt-4">
                  <h6 class="tw-text-gray-400 tw-text-sm">Social Media</h6>
                  <div class="d-flex mt-2" style="gap: 10px">
                    <a target="_blank" href="/">
                      <i
                        class="fa fa-youtube-play tw-text-red-500"
                        style="font-size: 18px"
                        aria-hidden="true"
                      ></i>
                    </a>
                    <a target="_blank" href="/">
                      <i
                        class="fa fa-twitter tw-text-blue-400"
                        style="font-size: 18px"
                        aria-hidden="true"
                      ></i>
                    </a>
                    <a target="_blank" href="/">
                      <i
                        class="fa fa-facebook tw-text-blue-700"
                        style="font-size: 18px"
                        aria-hidden="true"
                      ></i>
                    </a>
                    <a target="_blank" href="/">
                      <i
                        class="fa fa-instagram tw-text-red-400"
                        style="font-size: 18px"
                        aria-hidden="true"
                      ></i>
                    </a>
                    <a target="_blank" class="text-white" href="">
                      <i-icon icon="ic:baseline-tiktok" width="18px" />
                    </a>
                  </div>
                </div>
              </div>
            </div>
  
            <div class="">
              <hr class="tw-w-6/12 tw-mx-auto tw-border-gray-400" />
              <p class="text-center tw-text-gray200 small tw-mb-0">
                Copyright {{ thisYear }} © fooder. All rights reserved.
              </p>
            </div>
          </div>
        </footer>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {};
    },
    computed: {
      thisYear() {
        const yearToday = new Date().getFullYear();
        return yearToday;
      },
    },
  };
  </script>
  
  <style scoped>
  ul  {
    padding-left: 0;
  }
  
  ul li a {
    color: var(--gray-400);
    font-size: 13px;
    text-decoration: unset;
  }
  </style>
  