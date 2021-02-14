<template>
  <div>
    <div class="card has-background-dark has-text-light">
      <div class="card-content ">
        <div class="media">
          <div class="media-content">
            <p class="title is-4 has-text-light	">Movie • Nite</p>
            <p class="subtitle is-6 has-text-light">
              <a
                href="#"
                class="has-text-success"
                target="_blank"
                >Github</a
              >
            </p>
          </div>
        </div>

        <div class="content">
          #
          <br /><br />
          <code>Version {{ version }}</code
          ><br />
          <a
            href="#"
            target="_blank"
            class="has-text-success"
            >Changelog</a
          >
          <br /><br />
          <p class="subtitle is-6 has-text-light ">
            #
            <span class="has-text-weight-bold has-text-info">#</span>
          </p>
          <a
            class="button is-dark is-small"
            href="#"
            target="_blank"
          >
            <b-icon icon="github"></b-icon>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      version: null
    };
  },
  mounted() {
    var pckg = require("../package.json");
    this.version = pckg.version;
  }
};
</script>

<style></style>
