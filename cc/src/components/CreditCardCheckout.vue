<script>
export default {
  data() {
  	return {
	    tmp: "tmp"
  	}
	}
}
</script>
<template>
    <div class="w-[968px] h-[600px] bg-white flex flex-row">
		<div class="bg-red-200 text-gray-400 w-1/3">
			<img src="/CreditCardCheckout/hm.png" alt="H&M logo">
			<div>
				<h4>
					YOUR ORDER
				</h4>
			</div>
			<img src="/CreditCardCheckout/bag.png" alt="bag">
			<div>
				Coursele goes here
			</div>
			<div>
				<h3>
					TOTAL
					$145.98
				</h3>
			</div>
		</div>
		<div class="text-gray-400 w-2/3 gap-3 flex flex-col font-bold p-24">
			<div class="text-center">
				<h3 class="text-3xl">PAY WITH CREDIT CARD</h3>
			</div>
			<div>
				<div class="mt-2">
					<p>Name of Card Holder</p>
					<input
						type="text"
						placeholder="Name"
						class="bg-white p-2 border-2 border-gray-400">
				</div>
				<div>
					<p>Credit Card Number</p>
					<input
						type="text"
						placeholder="Card Number"
						class="bg-white p-2 border-2 border-gray-400">
				</div>
				<div>
					<div>
						<p>Expiration Date</p>
						<div class="flex flex-row gap-2">
						<input
							type="dropdown"
							class="bg-white p-2 border-2 border-gray-400 w-16">
						<input
						type="dropdown"
						class="bg-white p-2 border-2 border-gray-400 w-16">
						</div>
					</div>
					<div>
						<p>CVC</p>
						<input
							type="text"
							class="bg-white p-2 border-2 border-gray-400">
					</div>
				</div>
			</div>
		</div>
	</div>
</template>