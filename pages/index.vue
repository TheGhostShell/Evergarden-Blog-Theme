<template>
  <div>
    <hero />
    <div class="main-content">
      <div class="container">
        <div class="columns is-multiline is-centered">
          <div class="column is-12">
            <box />
            <pagination />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Box from '@/components/Body/Box.vue'
import Pagination from '@/components/Body/Pagination.vue'
import Hero from '@/components/Body/Hero.vue'
export default {
  layout: 'blog',
  components: {
    Box,
    Pagination,
    Hero
  }
}
</script>

<style lang="scss" scoped>
/* github.com/plasticneko */
/* bulma css framework by jeremy thomas (github.com/jgthms | bulma.io) */

/* basic formatting changes */

body,
.section {
  background-color: whitesmoke;
}

.pagination-next,
.pagination-previous,
.pagination-link {
  background-color: #fff;
}

.footer {
  margin-top: 2rem;
}

.footer-top-shadow {
  background-color: #fff;
  border-top: 1px solid transparent;
  box-shadow: 0 1px 2px rgba(10, 10, 10, 0.1);
}

.card-wrapper {
  padding-bottom: 20px;
}

.post-wrapper {
  padding-bottom: 40px;
}

.post-header img,
.content-header img {
  padding-bottom: 20px;
}

.continue-reading {
  padding: 30px;
}

.post-content-details {
  padding-bottom: 20px;
}

.content-wrapper p {
  padding-bottom: 15px;
}

.end-content-nav-wrapper {
  padding-bottom: 20px;
}

.end-post-details {
  padding-top: 15px;
  padding-bottom: 15px;
}

/* edits made to the bulma framework */

/* centering card-header-title text(1):
   ensures bottom shadow remains */
.card-header-fix-center {
  box-shadow: 0 1px 2px rgba(10, 10, 10, 0.1);
}

/* centering card-header-title text(2):
   ensures the header text remains of similar quality */
.card-header-title-fix {
  flex-grow: 1;
  font-weight: 700;
  padding: 0.75rem;
}

/* giving corners to the box styling */
.box {
  border-radius: 0px;
}
</style>
