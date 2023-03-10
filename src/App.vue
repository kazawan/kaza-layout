<template>
  <superbody win-size="24px" iphone-size="32px" >
    <krow gutter="10" mb="10" mt="10"  >
    <kcol span="8" xs="0" animation animation-delay=".1">
      <div class="header">
        #1-HEADER
      </div>
      
    </kcol>
    <kcol span="8" xs="24" animation animation-delay=".2" >
      <div class="header">
        #2-HEADER
      </div>
      
    </kcol>
    <kcol span="8" xs="24" animation animation-delay=".3" >
      <div class="header">
        #3-HEADER
      </div>
      
    </kcol>
  </krow>

  <krow gutter="10" mb="10">
    <kcol span="6" xs="0" md="24" animation animation-delay=".4">
      <div class="side">SIDE</div>
    </kcol>
    <kcol span="18" xs="24" md="0" animation animation-delay=".5">
      <div class="main">
        MAIN
      </div>
    </kcol>
  </krow>

  <krow gutter="10" mb="10">
    <kcol span="24" animation animation-delay=".1" >
      <div class="footer">
        FOOTER
      </div>
    </kcol>
  </krow>
  </superbody>
  
</template>


<script setup>
import krow from './components/kaza-layout/kRow.vue'
import kcol from './components/kaza-layout/kCol.vue'
import superbody from './components/kaza-layout/kSuperbody.vue'
</script>

<style lang="less">
.root {
  box-sizing: border-box;
}

.contianer {
  width: 50%;
  display: inline-block;
}

.header {
  width: 100%;
  
  background-color:#EAB543 ;
  border-radius: 5px;
  margin-bottom: 10px;
  font-size: 1rem;
}

.side{
  width: 100%;
  height:800px ;
  background-color:#55E6C1 ;
  border-radius: 10px;
}

.main{
  .side;
  background-color: #FC427B;
  font-size: 1rem;
  // paddingj: 0;
}

.footer{
  .header;
  background-color:  #2C3A47;
  color: white;
}
</style>