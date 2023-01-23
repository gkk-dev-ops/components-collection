<template>
    <div class="morgage-calc-wrapper w-[360px] h-[600px] bg-[#E1E0DE] text-[#484541] text-l">
        <div class="calc-select w-full text-xl">
            <h2 class="p-3 bg-[#BB5CF3] text-white mb-10">
                Select a Calculation
            </h2>
            <div class="flex flex-row justify-around text-sm text-left mb-6">
                <fieldset class="flex gap-2 justify-between">
                    <input name="calculation" type="radio" checked> Payment
                    <input name="calculation" type="radio" class="ml-9"> Mortgage Amount
                </fieldset>
            </div>
        </div>
        <div>
            <div>
                <h2 class="p-3 bg-[#BB5CF3] text-white">Enter Your Information</h2>
            </div>
            <div class="info mx-10 my-4 justify-center">
                <div class="m-2">
                    <p>Mortgage Amount</p>
                    <input type="text" placeholder="$100,000" class="p-2 w-full bg-white">
                </div>
                <div class="m-2 flex w-full">
                    <div>
                        <p>Amortization</p>
                        <div class="flex flex-row">
                            <input type="text" placeholder="25" class="p-2 w-[20px]">
                            <input type="text" placeholder="yrs" class="p-2 w-[20px]">
                        </div>
                    </div>
                    <p>Interest Rate</p>
                    <div class="flex flex-row">
                        <input type="text" placeholder="4.19" class="p-2 w-1/2">
                        <input type="text" placeholder="%" class="p-2 w-1/2">
                    </div>
                </div>
                <div class="m-2 flex">
                    <div>
                        <p>Payment Frequency</p>
                        <input type="text" placeholder="Monthly" class="p-2">
                    </div>
                    <div>
                        <p>Product</p>
                        <input type="text" placeholder="5 yr closed" class="p-2">
                    </div>
                </div>
                    <p class="text-right underline w-full my-1">
                        Aditional Lump Sum Payments
                    </p>
                <div  class="text-2xl flex justify-around">
                    <button class="text-white p-3 bg-[#BB5CF3]">
                        Calculate
                    </button>
                    <button class="p-3  border-2 border-[#BB5CF3]">
                        Save
                    </button>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
