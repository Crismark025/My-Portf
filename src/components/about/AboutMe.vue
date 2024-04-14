<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio:
						'Hey there, Im Crismark Im passionate about crafting robust and user=friendly web applications from start to finish. with a strong foundation in both front-end and back-end technologies, I bring creativity and problem-solving skills to every project I work on.',
				},
				{
					id: 2,
					bio:
						'On the front end, I specialize in creating responsive and intuitive user interfaces using HTML5, CSS3, and JavaScript frameworks like React.js and Vue.js. I pay close attention to user experience design principles to ensure that every interaction is seamless and engaging',
				},

				{
					id: 3,
					bio:
						'When it comes to the back end, Im proficient in building scalable and efficient server-side systems using languages like Node.js, Python, and Java. I have experience working with databases such as MySQL, MongoDB, and PostgreSQL, ensuring that data management is secure and optimized.',
				},
			],
		};
	},
};
</script>

<template>
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About profile image -->
		<div class="w-full sm:w-1/4 mb-7 sm:mb-0">
			<img
				src="@/assets/images/cs.jpg"
				class="rounded-xl w-96"
				alt=""
			/>
		</div>

		<!-- About details -->
		<div class="w-full sm:w-3/4 text-left">
			<p
				v-for="bio in bios"
				:key="bio.id"
				class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg"
			>
				{{ bio.bio }}
			</p>
		</div>
	</div>
</template>
