<template>
	<div>
 <h1>app根组件</h1>
 <TodoList :list="todolist"></TodoList>
 </div>
</template>

<script>
	import TodoList from './components/todolist.vue'
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
export default{
	data(){return
	{
		todolist:[
			{ id:1,task:'1',done:false },
			{ id:2,task:'2',done:false },
			{ id:3,task:'3',done:true }
		]
	}},
	components:{ TodoList }
	
}
</script>


<style lang="less" scoped>

</style>
