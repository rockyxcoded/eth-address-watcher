<script setup>
import { ref } from 'vue'

defineProps({
  transactions: Array
})

</script>

<template>
  <div class="py-10">
    <div class="text-center">
      <p
        class="py-5"
      >A simple Ethereum Blockchain Explorer that displays the last 10 transactions with selected details</p>
    </div>

    <div class="flex flex-col">
      <div class="my-2 overflow-x-auto sm:mx-6 lg:mx-2">
        <div class="py-2 align-middle inline-block min-w-full sm:px-6 lg:px-3">
          <div class="shadow overflow-hidden border-b border-gray-200 sm:rounded-lg">
            <table class="min-w-full divide-y divide-gray-200 px-10">
              <thead class="bg-gray-50">
                <tr>
                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >Block Number</th>
                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >Address</th>
                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >Hash</th>
                  <th
                    scope="col"
                    class="px-1 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >Timestamp</th>
                </tr>
              </thead>
              <tbody class="bg-white divide-y-2 divide-gray-100">
                <tr>
                  <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">answer.number</td>
                  <td>answer.author</td>
                  <td class="text-gray-600 text-sm">answer.hash</td>
                  <td
                    class="px-2 py-1 mt-3 inline-flex text-sm leading-5 font-semibold rounded-full bg-green-100 text-green-800"
                  >answer.timestamp</td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
