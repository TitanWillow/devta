<script setup>
import { DevtaLogo, hf10_banner_1032x600 } from "../../assets";
import TopBarButtons from "../../components/TopBarButtons/TopBarButtons.vue";

const IS_ELECTRON = window.IS_ELECTRON || false;
</script>

<template>
  <div class="m-0 p-0 w-100">
    <!-- <Sidebar /> -->
    <div class="container py-3 py-md-5 justify-content-start justify-content-xl-center" :style="IS_ELECTRON && 'height: calc(100vh - 54px) !important'">
      <div class="h1">
        <img class="img" :src="DevtaLogo" />
        <strong>Devta</strong>
      </div>
      <p class="p-1 text-muted lead text-center">
        Elevate your development experience with Devta, the ultimate tool for simplifying and enhancing your daily tasks. <br />
        Choose an option from the menu to start working. <br />
        <strong>We do not send any data you submit to any server.</strong> <br />
        <strong>
          <em><u>All data validation, processing and formatting is done in your browser.</u></em>
        </strong>
        <br />
        <em>You may check out the source code on our Github Repo!</em>
      </p>
      <div class="d-flex w-100 gap-2 justify-content-center align-items-center">
        <TopBarButtons />
      </div>
      <br />
        <div style="font-family: monospace" class="col-12 col-lg-5 p-4 text-lg-start text-center">
          <hr />
          <span class="pt-2">
            This deployment is intended for demonstration purposes only. It is based on a fork of the original open-source project and may include modifications or enhancements. For the official project, please refer to the original repository linked above.
          </span>
        </div>
        <div class="col"></div>
      </div>
    </div>
</template>

<style scoped src="./style.css"></style>
