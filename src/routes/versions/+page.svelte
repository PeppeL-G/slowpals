<script>
	
	import { versions } from "data/versions.js"
	
</script>

<h1>Versions</h1>
<p>
	On this page you can see the changes we have made to Slowpals for each
	version we have released.
</p>

{#each versions as version}
	<div>
		<h2 id="v{version.id}">{version.id} ({version.date})</h2>
		<ul>
			{#each version.changes as change}
				<li>{change}</li>
			{/each}
		</ul>
	</div>
{/each}