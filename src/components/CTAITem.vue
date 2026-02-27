<template>
  <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
<div class="CTAItem">
  <div class="frame">
    <div class="text">
      <div class="CTATitle">Title</div>
      <div class="CTABody">Supporting text about the call-to-action goes here</div>
    </div>
    <div class="button">
      <i class="material-icons">arrow_forward</i>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: "CallToActionItem"
}
</script>

<style scoped>
/* mobile viewport css section - mobile first*/
.CTAItem {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  min-height: 200px;
  background-image:
      linear-gradient(to bottom, transparent 50%, rgba(5,0,0,0.7)),
      url("../assets/CTAPicture.jpg");
  background-position: center;
  background-size: cover;
  border-radius: 4px;
  padding: 1rem;
}

.frame {
  display: flex;
  flex-direction: row;
  margin-top: auto;
  gap: 1rem;
  width: 100%;
}

.text {
  width: auto;
  gap: 8px;
}

.CTATitle {
  font-weight: bold;
  font-size: 22px;
  height: 24px;
  color: white;
}

.CTABody {
  font-size: 17px;
  color: #FAFAFA;
  opacity: 0.5;
}

.button {
  width: 48px;
  height: 48px;
  flex-shrink: 0;
  border-radius: 4px;
  border: 2px solid rgba(255, 255, 255, 0.33);
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: auto;
}
.button:hover{
  cursor: pointer;
}

.material-icons {
  color: white;
  font-size: 20px;
  cursor: pointer;
}
/*desktop viewport css*/
@media (min-width: 768px) {
  .frame {
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
  }

  .text {
    width: auto;
  }

  .CTATitle {
    font-size: 28px;
    height: auto;
  }

  .CTABody {
    font-size: 14px;
    height: 24px;
  }

  .button {
    width: 40px;
    height: 40px;
    align-self: center;
  }
  .material-icons{
    height: 20px;
    width: 20px;
  }
}

</style>
