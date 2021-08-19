<template>
	<v-container>
		<v-row justify="space-around">
			<v-card width="400">


				<v-card-text>
					<div class="font-weight-bold ml-8 mb-2">
						Experience
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
									<strong>{{ message.from }}</strong> @{{ message.time }}
								</div>
								
								<div class="shiftdown">{{ message.message }}</div>
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
	name: "Jobcard",
	data: () => ({
		messages: [
			{
				from: "TEK EXPERTS, LAGOS, NIGERIA",
				message: `CLOUD SUPPORT ENGINEER`,
				time: "MAY 2020 – OCT 2020",
				color: "deep-purple lighten-1",
			},
			{
				from: "ADDOSSER MICROFINANCE BANK, 32. LEWIS STREET",
				message: "SYSTEMS ADMINISTRATOR",
				time: "JULY 2018 – MAY 2020",
				color: "green",
			},
			{
				from: "ST. ANTHONY'S SENIOR SCONDARY SCHOOL",
				message: "DIGITAL CAPACITY CENTER ADMIN",
				time: "DECEMBER 2016 – MAY 2017",
				color: "deep-purple lighten-1",
			},
            {
				from: "GATEWAY ICT LIMITED,",
				message: "JUNIOR NETWORK ADMINISTRATOR",
				time: "AUGUST 2015 – JANUARY 2016",
				color: "deep-purple lighten-1",
			}
		],
	}),
};
</script>

<style>

.shiftdown{
	margin-top: 1rem
}
</style>
