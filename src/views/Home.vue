<template>
  <div>
    <div class="mainContainer">
      <OutletScreenTmpl :userName="userName" :customerName="customerName" :outlets="outlets" />
    </div>
  </div>
</template>

<script>
import LoginTmpl from "@/components/Login.vue";
import OutletScreenTmpl from "@/components/OutletScreen";

export default {
  name: "home",
  components: {
    OutletScreenTmpl
  },
  setup() {
    const userName = "pind";
    const customerName = "Pind";
    const outlets = [{ name: "Pind", outletID: "BANGALORE" }];
    return { userName, customerName, outlets };
  }
};
</script>
