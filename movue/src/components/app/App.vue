<template>
    <div class="app">
        <div class="content">
          <Appinfo />
          <div class="surch-panel">
            <Surchpanel />
            <AppFilter />
          </div>
          <MovueList />
          <MovueForm />
        </div>
    </div>
</template>
<script>
import Appinfo from "../app-info/appinfo.vue";
import Surchpanel from "../serch-panel/Surchpanel.vue";   
import AppFilter from "../appfilter/AppFilter.vue";
import MovueList from "../movue-list/MovueList.vue";
import MovueForm from "../movue-add-form/MovueForm.vue";
export default {
    components:{
    Appinfo,
    Surchpanel,
    AppFilter,
    MovueList,
    MovueForm
}
}
</script>
<style>
.app{
    height: 100vh;
    color: black;
}
.content{
    width: 1000px;
    min-height: 700px;
    background-color: white;
    margin:0 auto;
    padding: 5rem 0px;
}
.surch-panel{
    margin-top: 2rem;
    padding: 1.5rem;
    background-color: #fcfaf5;
    border-radius: 15px;
 box-shadow:
  0 2.8px 2.2px rgba(0, 0, 0, 0.034),
  0 6.7px 5.3px rgba(0, 0, 0, 0.048),
  0 12.5px 10px rgba(0, 0, 0, 0.06),
  0 22.3px 17.9px rgba(0, 0, 0, 0.072),
  0 41.8px 33.4px rgba(0, 0, 0, 0.086),
  0 100px 80px rgba(0, 0, 0, 0.12)
}
    
</style>