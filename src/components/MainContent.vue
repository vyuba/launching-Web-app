<script setup>
  import CoutdownContainer from './CoutdownContainer.vue';
  import formVue from "./FormItem.vue"
  import FooterB from './FooterContainer.vue';
</script>

<template>
 <div class="main-content light">

    <div class="page-title">

        <h1>We are launching soon!</h1>
        <CoutdownContainer/>

    </div><!--page-title-->
    <formVue/>
    <FooterB/>
</div><!--main-content-->
</template>