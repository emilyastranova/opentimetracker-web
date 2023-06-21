<script>
	import { Timeline, TimelineItem, Button, Activity, ActivityItem } from 'flowbite-svelte';
	let activities = [
		{
			title:
				'Tyler <a href="/" class="font-semibold text-primary-600 dark:text-primary-500 hover:underline">Clocked out</a>: End of day',
			date: 'just now',
			alt: 'image alt here',
			src: 'https://tylerharrison.dev/images/user-3.jpg'
		}
	];
</script>

<!-- Align elements to right -->
<div>
<Timeline>
	<TimelineItem title="Clocked in (current)" date="Monday, 08:46PM 06/20/23">
		<p class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400">Working remotely</p>
		<Button color="red"
			>Clock out<svg
				class="ml-2 w-3 h-3"
				fill="currentColor"
				viewBox="0 0 20 20"
				xmlns="http://www.w3.org/2000/svg"
				><path
					fill-rule="evenodd"
					d="M12.293 5.293a1 1 0 011.414 0l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-2.293-2.293a1 1 0 010-1.414z"
					clip-rule="evenodd"
				/></svg
			></Button
		>
	</TimelineItem>
	<TimelineItem title="Clocked out" date="Friday, 05:14PM 06/16/23">
		<p class="text-base font-normal text-gray-500 dark:text-gray-400">Out</p>
	</TimelineItem>
	<TimelineItem title="Clocked in" date="Friday, 01:02PM 06/16/23">
		<p class="text-base font-normal text-gray-500 dark:text-gray-400">Working remotely</p>
	</TimelineItem>
	<TimelineItem title="Clocked out" date="Friday, 12:05PM 06/16/23">
		<p class="text-base font-normal text-gray-500 dark:text-gray-400">Lunch break 🍎</p>
	</TimelineItem>
	<TimelineItem title="Clocked in" date="Friday, 09:05AM 06/16/23">
		<p class="text-base font-normal text-gray-500 dark:text-gray-400">Working in office</p>
	</TimelineItem>
</Timeline>
</div>