<template>
  <div class="contact-information" v-editable="blok">
    <p class="contact-information_title">{{blok.title}}</p>
    <p class="contact-information_description">{{blok.description}}</p>
  </div>
</template>
<script>
export default {
  name: 'ContactInformation',
  props: ['blok']
}
</script>
<style lang="scss">
.contact-information {
  padding: 0 $desktop-grid-gap;
}

.contact-information_title {
  font-size: 20px;
  font-weight: 500;
  color: #2c2c2c;
}

.contact-information_description {
  font-size: 16px;
  color: #2c2c2c;
  margin-top: 30px;
}

@media screen and (min-width: 1440px) {
  .contact-information {
    padding: 0 $desktop-container-spacing * 2.3;
  }
}

@media screen and (max-width: 800px) {
  .contact-information {
    padding: $mobile-container-spacing;
  }
}
</style>