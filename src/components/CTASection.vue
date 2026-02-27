<template>
  <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
  <div class="section-wrapper">
    <div class="header">
      <div class="labelAndSubtitle">
        <div class="label">Label</div>
        <div class="title">Mandatory title about the
          <span class="GTAlina">call-to-action</span> here
        </div>
      </div>
      <div class="textBody">Optional body copy goes here.</div>
      <div class="button">
        <div>Optional button</div>
        <i class="material-icons">arrow_forward</i>
      </div>
    </div>
    <div class="CTAItem">
      <CallToActionItem ></CallToActionItem>
      <CallToActionItem ></CallToActionItem>
    </div>
  </div>
</template>

<script>
import CallToActionItem from './CTAITem.vue'

export default {
  name: "CTASection",
  components: {
    CallToActionItem
  }
}
</script>

<style scoped>
@font-face {
  font-family: GTAlpina;
  src: url('~@/assets/fonts/GTAlpina-Regular.otf');
  font-weight: 400;
}

/*mobile viewport css*/
.section-wrapper {
  display: flex;
  flex-direction: column;
  width: auto;
  min-height: 100vh;
}

.header {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  gap: 16px;
}

.labelAndSubtitle {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 8px;
}

.label {
  font-size: 14px;
  color: #39494D;
}

.title {
  font-weight: bold;
  font-size: 36px;
  line-height: 40px;
  max-width: 100%;
}

.title span {
  font-family: GTAlpina;
  font-weight: 400;
}

.textBody {
  font-size: 16px;
  color: #1E2526;
  opacity: 0.8;
}

.button {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 4px;
  font-size: 18px;
  color: #BF564D;
  cursor: pointer;
}

.CTAItem {
  flex: 1;
  display: flex;
  flex-direction: column;
  gap: 16px;
  margin-top: 32px;
}

/*desktop viewport css*/
@media (min-width: 768px) {

  .header {
    gap: 24px;
  }

  .title {
    font-size: 40px;
    line-height: 48px;
    max-width: 500px;
    horiz-align: center;
    font-weight: 600;
  }
  .title span {
    font-size: 42px;
    font-weight: 400;
  }

  .textBody {
    font-size: 19px;
  }

  .button {
    font-size: 24px;
  }

  .CTAItem {
    flex-direction: row;
    width: auto;
    margin: 30px 0 0 0;
    padding-left: 30px;
    padding-right: 30px;
    gap: 24px;
  }

  .CTAItem > * {
    flex: 1;
    height: auto;
    min-height: 300px;
  }
}
</style>
