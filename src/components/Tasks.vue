<template>
	<div v-for="task in tasks" v-bind:key="task.id">
		<Task :task="task" />
	</div>
</template>

<script>
import Task from "./Task";
export default {
	name: "Tasks",
	components: {
		Task,
	},
	props: {
		tasks: Array,
	},
};
</script>
