<script>
	
	import { versions } from "data/versions.js"
	
	const latestVersion = versions[0]
	const now = new Date()
	
</script>

<footer>
	© {now.getFullYear()} Peter Larsson-Green |
	<a href="/versions">Version {latestVersion.id}</a>
</footer>

<style>
	
	footer{
		text-align: center;
	}
	
	a{
		color: black;
	}
	
	a:hover{
		color: rgb(72, 72, 72);
	}
	
</style>