<template>
	<div><ul class="list-group">
  <li class="list-group-item d-flex justify-content-between align-items-center">
		<div class='custom-control custom-checkbox'>
	<input type="checkbox" class='custom-control-input' :id="item.id"/> 
	<label class="custom-control-label" :for="item.id">xx</label>
	</div>
	<span class="badge badge-success badge-pill" v-if="item.done">完成</span>
	<span class="badge badge-warning badge-pill" v-else>未完成</span>

	 </li>
  </ul>
  </div>
</template>

<script>
	export default{
 name:'Todolist' ,
	props:{
		list:{
			type:Array,
			required:true,
			default: [],
			
		}
	}
	}
</script>

<style lang="less" scoped>
</style>