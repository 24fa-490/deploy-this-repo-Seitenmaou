<script>
	export let data;
	//console.log({data});
</script>

<h1>Fetched from Database</h1>

{#each data.containers as container}
	<div>
		<div class="id">{container.containernumber}</div>
		<div class="shipname">{container.nameofship}</div>
		<div class="date">{container.datecontainershipped}</div>
		<div class="size">{container.containersize}</div>
	</div>
{/each}

<span class="i">(database lives in PostgreSQL)</span>

<style>
	.id {
		margin-right: 10px;
		font-weight: bold;
	}
	.name {
		color: #999;
	}
	.i {
		font-style: italic;
	}
</style>
