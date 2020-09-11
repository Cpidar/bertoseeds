<template>
  <div class="uk-section-muted uk-section uk-section-xlarge">
    <div class="uk-position-relative">
      <div class="uk-margin-medium uk-container">
        <div class="tm-grid-expand uk-child-width-1-1 uk-grid uk-grid-stack" uk-grid>
          <div class="uk-width-1-1@m uk-first-column">
            <h2
              class="uk-position-relative uk-width-2xlarge uk-margin-auto uk-text-center"
              style="z-index: 1;"
            >
              <a href="/themes/wordpress/2020/kitchen-daily/index.php?post_type=recipe">120 recipes</a>
              everyone can make. Browse through
              <a href="/themes/wordpress/2020/kitchen-daily/index.php?page_id=52">all categories</a> and pick your favorite dish for every occasion.
            </h2>
            <div
              class="uk-position-relative uk-margin-xlarge uk-margin-remove-bottom uk-text-center"
              style="z-index: 1;"
            >
              <div
                class="uk-child-width-auto uk-flex-center uk-grid-small uk-grid-match uk-grid"
                uk-grid
              >
                <div v-for="item in items" :key="item.id">
                  <a
                    class="el-item uk-panel uk-margin-remove-first-child uk-transition-toggle uk-link-toggle uk-display-block"
                    href="https://demo.yootheme.com/themes/wordpress/2020/kitchen-daily/?recipe_cat=breakfast"
                  >
                    <div class="uk-inline-clip uk-border-rounded">
                      <img
                        src="/themes/wordpress/2020/kitchen-daily/wp-content/themes/yootheme/cache/recipes-category-breakfast-intro-a798ed6a.webp"
                        srcset="/themes/wordpress/2020/kitchen-daily/wp-content/themes/yootheme/cache/recipes-category-breakfast-intro-a798ed6a.webp 140w, /themes/wordpress/2020/kitchen-daily/wp-content/themes/yootheme/cache/recipes-category-breakfast-intro-a492e654.webp 280w"
                        sizes="(min-width: 140px) 140px"
                        data-width="140"
                        data-height="93"
                        class="el-image uk-transition-scale-up uk-transition-opaque"
                        alt
                      />
                    </div>

                    <div
                      class="el-title uk-h6 uk-margin-small-top uk-margin-remove-bottom"
                    >{{item.name}}</div>
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div
        class="uk-visible@m tm-grid-expand uk-child-width-1-1 uk-margin-remove-vertical uk-grid uk-grid-stack"
        uk-grid
      >
        <div class="uk-grid-item-match uk-width-1-1@m uk-visible@m uk-first-column" id="page#1-1-0">
          <div class="uk-panel uk-width-1-1">
            <div
              id="page#1-1-0-0"
              class="uk-visible@m uk-position-absolute uk-width-1-1"
              uk-parallax="y: 0,-120;"
              style="left: -3vw; top: -550px; transform: translateY(-7px);"
            >
              <img
                src="/themes/wordpress/2020/kitchen-daily/wp-content/themes/yootheme/cache/home-categories-01-b77126e9.webp"
                srcset="/themes/wordpress/2020/kitchen-daily/wp-content/themes/yootheme/cache/home-categories-01-b77126e9.webp 360w, /themes/wordpress/2020/kitchen-daily/wp-content/themes/yootheme/cache/home-categories-01-0a6edc85.webp 720w"
                sizes="(min-width: 360px) 360px"
                data-width="360"
                data-height="778"
                class="el-image"
                alt
                target="!*"
              />
            </div>

            <div
              id="page#1-1-0-1"
              class="uk-visible@m uk-position-absolute uk-width-1-1 uk-text-right"
              uk-parallax="y: 0,-120;"
              style="left: 80px; top: -295px; transform: translateY(0px);"
            >
              <img
                src="/themes/wordpress/2020/kitchen-daily/wp-content/themes/yootheme/cache/home-categories-02-facb8f28.webp"
                srcset="/themes/wordpress/2020/kitchen-daily/wp-content/themes/yootheme/cache/home-categories-02-facb8f28.webp 550w, /themes/wordpress/2020/kitchen-daily/wp-content/themes/yootheme/cache/home-categories-02-e7f9893e.webp 768w, /themes/wordpress/2020/kitchen-daily/wp-content/themes/yootheme/cache/home-categories-02-a4c02ad2.webp 1024w, /themes/wordpress/2020/kitchen-daily/wp-content/themes/yootheme/cache/home-categories-02-73ec4577.webp 1100w"
                sizes="(min-width: 550px) 550px"
                data-width="550"
                data-height="808"
                class="el-image"
                alt
                target="!*"
              />
            </div>
          </div>
        </div>
      </div>

      <div
        class="tm-section-title uk-position-center-left uk-position-medium uk-text-nowrap uk-visible@xl"
      >
        <div class="tm-rotate-180">My Categories</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["items"],
};
</script>
