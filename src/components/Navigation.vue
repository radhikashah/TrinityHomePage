<script setup>
    import IconCart from './icons/IconCart.vue'
    import IconSerch from './icons/IconSearch.vue'
</script>

<template>
  <nav>
    <ul class="nav-list justify-end hidden xl:flex">
      <li><a href="#">Location</a></li>
      <li><a href="#">Subscribe</a></li>
      <li><a href="#">Contact Us</a></li>
      <li>
        <a class="tel" href="tel:+8668300796">
            Call Us: 866.830.0796
        </a>
      </li>
      <li><a href="#"><IconCart /></a></li>
      <li><a href="#"><IconSerch /></a></li>
      <li><a href="#">Sign In</a></li>
    </ul>
    <ul class="nav-list justify-end hidden xl:flex">
      <li><a href="#">Consulting</a></li>
      <li><a href="#">Technology</a></li>
      <li><a href="#">Staffing</a></li>
      <li><a href="#">Software</a></li>
      <li><a href="#">Training</a></li>
      <li><a href="#">Industries</a></li>
      <li><a href="#">News</a></li>
      <li><a href="#">About Us</a></li>
      <li><a href="#">Careers</a></li>
    </ul>



    <div class="mobile-navigation xl:hidden flex item-center gap-4 p-4 text-center">
        <a href="/contactus" aria-label="Contact Us">
            <svg width="30" height="30.219" viewBox="0 0 39.359 30.219">
                <g id="Group_4470" data-name="Group 4470" transform="translate(-2.959 -62.383)">
                    <g id="Group_4469" data-name="Group 4469" transform="translate(3.459 62.883)">
                        <path id="Path_6081" data-name="Path 6081" d="M34.988,61H3.371A3.377,3.377,0,0,0,0,64.371V86.848a3.377,3.377,0,0,0,3.371,3.371H34.988a3.377,3.377,0,0,0,3.371-3.371V64.371A3.377,3.377,0,0,0,34.988,61Zm-.466,2.248L19.251,78.519,3.848,63.248ZM2.248,86.382V64.826L13.072,75.558Zm1.589,1.589L14.668,77.14l3.8,3.763a1.124,1.124,0,0,0,1.586,0l3.7-3.7L34.522,87.971Zm32.275-1.589L25.339,75.61,36.112,64.837Z" transform="translate(0 -61)" fill="#707070" stroke="#707070" stroke-width="1"></path>
                    </g>
                </g>
            </svg>
        </a><a href="/search" aria-label="Search">
            <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 56.966 56.966">
                <path xmlns="http://www.w3.org/2000/svg" d="M55.146 51.887L41.588 37.786A22.926 22.926 0 0046.984 23c0-12.682-10.318-23-23-23s-23 10.318-23 23 10.318 23 23 23c4.761 0 9.298-1.436 13.177-4.162l13.661 14.208c.571.593 1.339.92 2.162.92.779 0 1.518-.297 2.079-.837a3.004 3.004 0 00.083-4.242zM23.984 6c9.374 0 17 7.626 17 17s-7.626 17-17 17-17-7.626-17-17 7.626-17 17-17z" fill="#8f8d8d" data-original="#000000"></path>
            </svg>
        </a><a href="/locations" aria-label="Locations">
            <svg width="30" height="30" viewBox="0 0 28.266 39.779">
                <g id="Group_47" data-name="Group 47" transform="translate(0.5 0.5)">
                    <g id="Group_42" data-name="Group 42" transform="translate(0 0)">
                        <g id="Group_41" data-name="Group 41">
                            <path id="Path_4737" data-name="Path 4737" d="M390.633,428.089a13.635,13.635,0,0,0-11.6,20.8l10.822,17.44a1.136,1.136,0,0,0,.965.537h.009a1.138,1.138,0,0,0,.966-.552l10.546-17.609a13.636,13.636,0,0,0-11.71-20.618Zm9.76,19.452-9.589,16.009-9.839-15.855a11.369,11.369,0,1,1,19.428-.154Z" transform="translate(-377 -428.089)" fill="#707070" stroke="#707070" stroke-miterlimit="10" stroke-width="1"></path>
                        </g>
                    </g>
                    <g id="Group_44" data-name="Group 44" transform="translate(6.817 6.817)">
                        <g id="Group_43" data-name="Group 43" transform="translate(0 0)">
                            <path id="Path_4738" data-name="Path 4738" d="M398.567,442.839a6.817,6.817,0,1,0,6.817,6.817A6.824,6.824,0,0,0,398.567,442.839Zm0,11.376a4.56,4.56,0,1,1,4.552-4.559A4.563,4.563,0,0,1,398.567,454.215Z" transform="translate(-391.75 -442.839)" fill="#707070" stroke="#707070" stroke-miterlimit="10" stroke-width="1"></path>
                        </g>
                    </g>
                </g>
            </svg>
        </a><a href="/login" aria-label="Login">
            <svg width="30" height="30" viewBox="0 0 46.13 40.599">
                <g id="Group_46" data-name="Group 46" transform="translate(0.25 0.25)">
                    <path id="Path_4739" data-name="Path 4739" d="M569.2,799.162h24.241a1.337,1.337,0,0,0,1.285-.969l5.346-18.713a1.337,1.337,0,0,0-1.285-1.7h-32.67l-.955-4.3a1.337,1.337,0,0,0-1.305-1.047h-8.02a1.337,1.337,0,0,0,0,2.673h6.948l4.826,21.717a4.009,4.009,0,0,0,1.593,7.689h24.237a1.337,1.337,0,0,0,0-2.673H569.208a1.336,1.336,0,0,1,0-2.673Zm27.815-18.713-4.583,16.039H570.28l-3.564-16.039Z" transform="translate(-554.505 -772.429)" fill="#707070" stroke="#707070" stroke-miterlimit="10" stroke-width="0.5"></path>
                    <path id="Path_4740" data-name="Path 4740" d="M612.028,914.5a4.01,4.01,0,1,0,4.01-4.01A4.015,4.015,0,0,0,612.028,914.5Zm4.01-1.336A1.337,1.337,0,1,1,614.7,914.5,1.338,1.338,0,0,1,616.038,913.159Z" transform="translate(-598.662 -878.407)" fill="#707070" stroke="#707070" stroke-miterlimit="10" stroke-width="0.5"></path>
                    <path id="Path_4741" data-name="Path 4741" d="M693.328,914.5a4.01,4.01,0,1,0,4.01-4.01A4.015,4.015,0,0,0,693.328,914.5Zm4.01-1.336A1.337,1.337,0,1,1,696,914.5,1.338,1.338,0,0,1,697.338,913.159Z" transform="translate(-661.071 -878.407)" fill="#707070" stroke="#707070" stroke-miterlimit="10" stroke-width="0.5"></path>
                </g>
            </svg>
        </a><a class="drawer-toggle" href="" aria-label="Moble Nav Toggle">
            <svg data-name="Group 50" width="30" height="30" viewBox="0 0 34.052 26.077">
                <g id="Group_49" data-name="Group 49" transform="translate(0 0)">
                    <g id="Group_48" data-name="Group 48">
                        <rect id="Rectangle_3688" data-name="Rectangle 3688" width="34.052" height="4.822" transform="translate(0 21.254)" fill="#707070"></rect>
                        <rect id="Rectangle_3689" data-name="Rectangle 3689" width="34.052" height="4.822" transform="translate(0 10.627)" fill="#707070"></rect>
                        <rect id="Rectangle_3690" data-name="Rectangle 3690" width="34.052" height="4.822" fill="#707070"></rect>
                    </g>
                </g>
            </svg>
        </a>
    </div>
  </nav>
</template>