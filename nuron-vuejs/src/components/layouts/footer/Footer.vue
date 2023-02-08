<template>
  <div>
    <!-- Start Footer Area -->
    <div
      :class="[
        `rn-footer-one bg-color--1 mt--100 mt_md--80 mt_sm--80`,
        data.showFooterBrand ? 'rn-section-gapBottom' : 'rn-section-gap',
      ]"
    >
      <div v-if="data.showFooterBrand" class="footer-top">
        <div class="container">
          <div class="row">
            <ul class="nu-brand-area">
              <li>
                <img
                  :src="require(`@/assets/images/brand/brand-01.png`)"
                  alt="nuron-brand_nft"
                />
              </li>
              <li>
                <img
                  :src="require(`@/assets/images/brand/brand-03.png`)"
                  alt="nuron-brand_nft"
                />
              </li>
              <li>
                <img
                  :src="require(`@/assets/images/brand/brand-06.png`)"
                  alt="nuron-brand_nft"
                />
              </li>
              <li>
                <img
                  :src="require(`@/assets/images/brand/brand-07.png`)"
                  alt="nuron-brand_nft"
                />
              </li>
              <li>
                <img
                  :src="require(`@/assets/images/brand/brand-04.png`)"
                  alt="nuron-brand_nft"
                />
              </li>
              <li>
                <img
                  :src="require(`@/assets/images/brand/brand-02.png`)"
                  alt="nuron-brand_nft"
                />
              </li>
              <li>
                <img
                  :src="require(`@/assets/images/brand/brand-01.png`)"
                  alt="nuron-brand_nft"
                />
              </li>
              <li>
                <img
                  :src="require(`@/assets/images/brand/brand-03.png`)"
                  alt="nuron-brand_nft"
                />
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="container">
        <div class="row gx-5">
          <div class="col-lg-3 col-md-6 col-sm-6 col-12">
            <div class="widget-content-wrapper">
              <div class="footer-left">
                <logo />
                <p class="rn-footer-describe">
                  Created by gamers for gamers to take advantage of
                  buying/selling game collectibles as NFTs
                </p>
              </div>
            </div>
          </div>

          <div class="col-lg-3 col-md-6 col-sm-6 col-12 mt_mobile--40">
            <div class="footer-widget widget-quicklink">
              <h6 class="widget-title">Nuron</h6>
              <ul class="footer-list-one">
                <li class="single-list">
                  <router-link to="#">Top Games</router-link>
                </li>
                <li class="single-list">
                  <router-link to="#">New Games</router-link>
                </li>
                <li class="single-list">
                  <router-link to="#">All Games</router-link>
                </li>
                <li class="single-list">
                  <router-link to="#">Auctions</router-link>
                </li>
              </ul>
            </div>
          </div>

          <div class="col-lg-3 col-md-6 col-sm-6 col-12 mt_md--40 mt_sm--40">
            <div class="footer-widget widget-information">
              <h6 class="widget-title">Information</h6>
              <ul class="footer-list-one">
                <li class="single-list">
                  <router-link to="#">Gamer's Explore</router-link>
                </li>
                <li class="single-list">
                  <router-link to="#">GameLink Token</router-link>
                </li>
                <li class="single-list">
                  <router-link to="#">About Us</router-link>
                </li>
                <li class="single-list">
                  <router-link to="#">FAQ</router-link>
                </li>
              </ul>
            </div>
          </div>

          <div class="col-lg-3 col-md-6 col-sm-6 col-12 mt_md--40 mt_sm--40">
            <div class="footer-widget">
              <h6 class="widget-title">Recent Sold Out</h6>
              <ul class="footer-recent-post">
                <li class="recent-post">
                  <div class="thumbnail">
                    <router-link to="/product/1">
                      <img
                        :src="
                          require(`@/assets/images/portfolio/portfolio-01.jpg`)
                        "
                        alt="Product Images"
                      />
                    </router-link>
                  </div>
                  <div class="content">
                    <h6 class="title">
                      <router-link to="/product/1">#21 The Wonder</router-link>
                    </h6>
                    <p>Highest bid 1/20</p>
                    <span class="price">0.244SSC</span>
                  </div>
                </li>
                <li class="recent-post">
                  <div class="thumbnail">
                    <router-link to="/product/2">
                      <img
                        :src="
                          require(`@/assets/images/portfolio/portfolio-02.jpg`)
                        "
                        alt="Product Images"
                      />
                    </router-link>
                  </div>
                  <div class="content">
                    <h6 class="title">
                      <router-link to="/product/2">Diamond Dog</router-link>
                    </h6>
                    <p>Highest bid 1/20</p>
                    <span class="price">0.022SSC</span>
                  </div>
                </li>
                <li class="recent-post">
                  <div class="thumbnail">
                    <router-link to="/product/3">
                      <img
                        :src="
                          require(`@/assets/images/portfolio/portfolio-03.jpg`)
                        "
                        alt="Product Images"
                      />
                    </router-link>
                  </div>
                  <div class="content">
                    <h6 class="title">
                      <router-link to="/product/3">Morgan11</router-link>
                    </h6>
                    <p>Highest bid 1/20</p>
                    <span class="price">0.892SSC</span>
                  </div>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- End Footer Area -->

    <!-- Start Copyright Area -->
    <div class="copy-right-one ptb--20 bg-color--1">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-lg-6 col-md-12 col-sm-12">
            <div class="copyright-left">
              <span>©2023 GameLink, Inc. All rights reserved.</span>
              <ul class="privacy">
                <li>
                  <router-link to="/terms-condition">Terms</router-link>
                </li>
                <li>
                  <router-link to="/privacy-policy">Privacy Policy</router-link>
                </li>
              </ul>
            </div>
          </div>
          <div class="col-lg-6 col-md-12 col-sm-12">
            <div class="copyright-right">
              <social-links />
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- End Copyright Area -->

    <div class="mouse-cursor cursor-outer" />
    <div class="mouse-cursor cursor-inner" />

    <!-- Start Top To Bottom Area  -->
    <back-to-top @click="scrollTop" />
    <!-- End Top To Bottom Area  -->
  </div>
</template>

<script>
import BackToTop from '@/components/layouts/footer/BackToTop'
import Logo from "@/components/logo/Logo";
import SocialLinks from "@/components/social/SocialLinks";

export default {
  name: 'Footer',
  components: { SocialLinks, Logo, BackToTop },
  props: {
    data: {
      default: null
    }
  },
  methods: {
    scrollTop() {
      window.scrollTo(0, 0);
    }
  }
}
</script>
