
<template>
<div class="page">
  <select v-model="selected">
    <option>option</option>
    </select>
<AppUserList >
  <template #userlist="{list: users,remove}">
  <AppCardView :list="users">
  <template #secondrow="{ item: user}">
<AppButton @click="remove(item)">{{user.name.first}}</AppButton>

  </template>  
  </AppCardView> 
  </template>
</AppUserList>
</div>
</template>

<script>
import AppUserList from "./components/AppUserList";
import AppButton from "./components/AppButton";
import AppCardView from "./components/AppCardView";


export default{
  data(){
    return{
      selected:"first"
    }
  },
  components:{
    AppUserList,
   AppButton ,
   AppCardView
  }
};
</script>