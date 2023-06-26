<script lang="ts">
	import dayjs from 'dayjs'; // ES 2015
	const date = dayjs();
	let currentTime = date;
	const updateTime = () => {
		currentTime = dayjs();
	};
	setInterval(updateTime, 1000);
</script>

<main class="grid grid-cols-[30vw_70vw] h-screen w-screen bg-[#56585d] text-white">
	<ul>
		<!-- TODO List -->
	</ul>

	<div>
		{date.format('DD MMM YYYY')}
		{currentTime.format('HH:mm:ss A')}
		<!-- Clock -->
	</div>
</main>
