<template>
	<v-container>
		<v-row justify="space-around">
			<v-card width="400">
				<v-card-text>
					<div class="font-weight-bold ml-8 mb-2">
						Projects
					</div>

					<v-timeline align-top dense>
						<v-timeline-item
							v-for="message in messages"
							:key="message.time"
							:color="message.color"
							small
						>
							<div>
								<div class="font-weight-normal">
									<strong
										><a class="noundie" :href="message.message" target="_blank">{{
											message.from
										}}</a></strong
									>
								</div>
							</div>
						</v-timeline-item>
					</v-timeline>
				</v-card-text>
			</v-card>
		</v-row>
	</v-container>
</template>

<script>
export default {
	name: "Skillcard",
	data: () => ({
		messages: [
			{
				from: "Irorun App",
				message: "https://friendly-hopper-4a173d.netlify.app/",
				color: "blue lighten-1",
			},
			{
				from: " Apoti Ajo",
				message: `https://jolly-stonebraker-a6a3ae.netlify.app/`,
				color: "blue lighten-1",
			},
			{
				from: " Run Tracker",
				message: `https://rippyblogger.github.io/RunTrackApp/`,
				color: "blue lighten-1",
			},
			{
				from: "Email Marketing Website Landing page",
				message: "https://rippyblogger.github.io/Deliver/",
				color: "green",
			},
			{
				from: "URL Shortner",
				message: "https://thirsty-fermat-a029ad.netlify.app/",
			},
			{
				from: "IP Tracker",
				message: "https://rippyblogger.github.io/Ip-Tracker/",
				color: "blue lighten-1",
			},
			
		],
	}),
};
</script>

<style>
.noundie {
	text-decoration: none;
}
</style>
