<template>
  <div class="left-side">
    <figure class="logotype">
      <img src="/assets/logo.svg" alt="Логотип компании ВСЕМ ЕДА">
    </figure>     
    <div class="input-search">
      <input type="text" v-bind:value="searchAddress" class="edit-adress" />
      <!-- <div class="address-items">
        <ul>
          <li> <img src="/assets/cil_location-pin.svg" alt="Иконка навигации"> <span>ул. Петровско-Разумовская 17</span></li>
          <li> <img src="/assets/cil_location-pin.svg" alt="Иконка навигации"> <span>ул. Сибирский проезд 10, к.2</span></li>
          <li> <img src="/assets/cil_location-pin.svg" alt="Иконка навигации"> <span>ул. Перервинский бульвар 27, к.1</span></li>
        </ul>
      </div> -->
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      searchAddress: 'ул. Петровско-Разумовская 17'
    }
  }
}
</script>

<style>

</style>