<template>
  <div class="lds-dual-ring"></div>
</template>

<script>
    export default {
        name: "loader-tiny"
    }
</script>

<style scoped>
.lds-dual-ring {
  display: inline-block;
  width: 10px;
  height: 10px;
}
.lds-dual-ring:after {
  content: " ";
  display: block;
  width: 10px;
  height: 10px;
  margin: 8px;
  border-radius: 50%;
  border: 2px solid #5347E3;
  border-color: #5347E3 transparent #5347E3 transparent;
  animation: lds-dual-ring 1.2s linear infinite;
}
@keyframes lds-dual-ring {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}


</style>
