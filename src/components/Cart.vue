<template>
  <div class="payment-container p-8 bg-gray-50 min-h-screen">
    <div class="mb-6">
      <h2 class="text-xl font-semibold">Payment Method</h2>
      <p class="text-sm text-gray-500">Select your payment option</p>
    </div>

    <div class="bg-white shadow rounded-lg p-6">
      <div class="flex flex-col space-y-4">
        <div class="flex items-center">
          <input
            type="radio"
            id="creditCard"
            name="paymentMethod"
            class="mr-2"
          />
          <label for="creditCard" class="font-medium">Credit/Debit Card</label>
        </div>
        <div class="flex items-center">
          <input type="radio" id="paypal" name="paymentMethod" class="mr-2" />
          <label for="paypal" class="font-medium">PayPal</label>
        </div>
        <div class="flex items-center">
          <input type="radio" id="bankTransfer" name="paymentMethod" class="mr-2" />
          <label for="bankTransfer" class="font-medium">Bank Transfer</label>
        </div>
      </div>
    </div>

    <div class="bg-white shadow rounded-lg p-6 mt-6">
      <h3 class="text-lg font-semibold mb-4">Card Information</h3>
      <form>
        <div class="mb-4">
          <label for="cardNumber" class="block text-sm font-medium mb-1">Card Number</label>
          <input
            type="text"
            id="cardNumber"
            placeholder="1234 5678 9012 3456"
            class="w-full border border-gray-300 rounded-lg p-2"
          />
        </div>
        <div class="mb-4">
          <label for="expiryDate" class="block text-sm font-medium mb-1">Expiry Date</label>
          <input
            type="text"
            id="expiryDate"
            placeholder="MM/YY"
            class="w-full border border-gray-300 rounded-lg p-2"
          />
        </div>
        <div class="mb-4">
          <label for="cvv" class="block text-sm font-medium mb-1">CVV</label>
          <input
            type="text"
            id="cvv"
            placeholder="123"
            class="w-full border border-gray-300 rounded-lg p-2"
          />
        </div>
        <button class="mt-4 px-6 py-2 text-white bg-orange-500 rounded-lg">
          Complete Payment
        </button>
      </form>
    </div>
  </div>
</template>

<script setup>
</script>

<style  >
 
</style>
