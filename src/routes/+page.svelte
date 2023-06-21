<script>
	import Navbar from '../lib/Navbar.svelte';
	import DayHoursCard from '../lib/DayHoursCard.svelte';
	import WeekHoursCard from '../lib/WeekHoursCard.svelte';
	import ActivityLog from '../lib/ActivityLog.svelte';
</script>

<div>
	<Navbar />
	<div class="m-4 grid md:grid-cols-3 gap-4">
		<div class="col-span-2">
			<h1 class="mb-4 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Overview</h1>
			<div class="flex flex-row gap-4">
				<DayHoursCard />
				<WeekHoursCard />
			</div>
		</div>
		<div>
			<h1 class="mb-4 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Activity Log</h1>
			<div class="flex flex-row gap-4">
				<ActivityLog />
			</div>
		</div>
	</div>
</div>
