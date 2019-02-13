<template>
  <div class="cal">
      </div>
  </template>
  <script>

export default {
  name: "cal",
  data: function(){ 
      return {input: null }
  },
computed: {
    fifteen: function() {
      return (this.input * 0.15).toFixed(2);
    },
    eighteen: function() {
      return (this.input * 0.18).toFixed(2);
    },
    twenty: function() {
      return (this.input * 0.2).toFixed(2);
    },

    tFifteen: function() {
      return (this.input + +this.fifteen).toFixed(2);
    },
    tEighteen: function() {
      return (this.input + +this.eighteen).toFixed(2);
    },
    tTwenty: function() {
      return (this.input + +this.twenty).toFixed(2);
    }
  }
};
</script>
      


<style>
.input-group-addon,
.form-control {
  font-size: 60px;
  }
  
  </style>