<template>
  <div>
    <div class="header-block">
      <div class="left-block">
        <LeftBlock />
      </div>
      <div class="right-block">
        <RightBlock />
      </div>
    </div>
    <nav>
      <div class="nav-block-btn">
        <div class="btn-nav active">Все</div>
        <div class="btn-nav">Суши</div>
        <div class="btn-nav">Пицца</div>
        <div class="btn-nav">Бургеры</div>
        <div class="btn-nav">Фастфуд</div>
        <div class="btn-nav">Шашлыки</div>
        <div class="btn-nav">Азиатская</div>
        <div class="btn-nav">Десерты</div>
        <div class="btn-nav">Здоровая еда</div>
        <div @mouseover="ExpandArrow" @mouseout="ExpandArrow" class="btn-nav btn-expand">Еще
          <Expand 
          :colorHover="colorHover" />
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
import LeftBlock from '../items/LeftBlock';
import RightBlock from '../items/RightBlock';
import Expand from '../items/Expand';

export default {
  components: { Expand, LeftBlock, RightBlock },
  data() {
    return {
      colorHover: 'white'
    }
  },
  methods:{
    ExpandArrow: function(){
      this.colorHover = this.colorHover != 'white' ? 'white' : 'black';
    }
  }

};
</script>

<style>
</style>