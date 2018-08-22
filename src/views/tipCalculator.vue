<template>
<div class="container mt-3 mt-sm-5" id="cal">
  <div class="row justify-content-center mb-4">
    <div class="col-md-4">
      <div class="input-group">
        <div class="input-group-addon">$</div>
        <input class="form-control" type="number" v-model="input"/>
      </div>
    </div>
  </div>
  <div class="row justify-content-center" v-if="input">
    <div class="col-md-6">
      <table class="table">
        <thead>
          <tr>
            <th></th>
            <th>15%</th>
            <th>18%</th>
            <th>20%</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <th>Tip</th>
            <td>${{ fifteen }}</td>
            <td>${{ eighteen }}</td>
            <td>${{ twenty }}</td>
          </tr>
          <tr>
            <th>Total</th>
            <td>${{ tFifteen }}</td>
            <td>${{ tEighteen }}</td>
            <td>${{ tTwenty }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</div>
</template>
<script>
// @ is an alias to /src
import Cal from '@/components/Cal.vue'

export default {
  name: 'cal',
  components: {
    Cal
  }
}
</script>
<style>
.input-group-addon,
.form-control {
  font-size: 30px;
}
</style>