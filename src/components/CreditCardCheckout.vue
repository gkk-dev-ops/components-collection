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
		<div class="bg-[#F1EAE9] text-gray-600 w-1/3 text-center">
			<img src="/CreditCardCheckout/hm.png" alt="H&M logo" class="w-16 mb-4 mt-6 mx-auto">
			<div>
				<h4 class="text-3xl mb-2">
					YOUR ORDER
				</h4>
			</div>
			<div class="m-2">
				<img src="/CreditCardCheckout/bag.png" alt="bag">
			</div>
			<div class="mt-4 mb-10 justify-center flex flex-row items-center gap-2">
				<div class="w-1 h-1 rounded-lg bg-gray-400"></div>
				<div class="w-1 h-1 rounded-lg bg-red-600"></div>
				<div class="w-1 h-1 rounded-lg bg-gray-400"></div>
				<div class="w-1 h-1 rounded-lg bg-gray-400"></div>
				<div class="w-1 h-1 rounded-lg bg-gray-400"></div>
			</div>
			<div>
				<h3 class="text-xl">
					TOTAL
					<div class="font-bold text-2xl">
						$145.98
					</div>
				</h3>
			</div>
		</div>
		<div class="text-gray-400 w-2/3 gap-3 flex flex-col font-bold p-24 pt-16">
			<div class="text-center">
				<h3 class="text-3xl">PAY WITH CREDIT CARD</h3>
			</div>
			<div class="justify-center mx-auto flex flex-col gap-4">
				<div class="mt-2">
					<p>Name of Card Holder:</p>
					<input
						type="text"
						placeholder="Name"
						class="bg-white p-4 border-2 border-gray-400 w-full rounded m-1">
				</div>
				<div>
					<p>Credit Card Number</p>
					<input
						type="text"
						placeholder="Card Number"
						class="bg-white p-4 border-2 border-gray-400 w-full rounded m-1">
				</div>
				<div class="flex flex-row gap-2">
					<div>
						<p>Expiration Date</p>
						<div class="flex flex-row">
						<input
							type="text"
							placeholder="MM"
							class="bg-white p-4 border-2 border-gray-400 w-16 rounded-tl rounded-bl m-1">
						<input
						type="text"
						placeholder="YYYY"
						class="bg-white p-4 border-2 border-gray-400 w-20 rounded-tr rounded-br m-1">
						</div>
					</div>
					<div>
						<p>CVC</p>
						<input
							type="text"
							placeholder="CVV"
							class="bg-white p-4 border-2 border-gray-400 w-32 rounded m-1">
					</div>
				</div>
				<button class="mt-4 bg-[#bd2725] text-white p-4 rounded active:bg-red-400">
					PAY SECURELY
				</button>
			</div>
		</div>
	</div>
</template>