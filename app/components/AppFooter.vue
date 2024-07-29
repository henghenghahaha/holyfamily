<script setup lang="ts">
const links = [{
  label: 'Resources',
  children: [{
    label: 'Home',
    to: '/'
  }, {
    label: 'Majors',
    to: '/major'
  }, {
    label: 'Course Catalogs',
    to: '/course'
  }, {
    label: 'Inquery Degree',
    to: '/inquery'
  }]
}]
</script>

<template>
  <UFooter  :ui="{top: {
    wrapper: 'bg-blue-900',
    container: 'py-8 lg:py-12'
  },}">
    <template #top>
      <UFooterColumns :links="links" :ui="{label: 'text-sm/6 font-semibold text-white dark:text-white',active: 'text-white dark:text-white font-medium',
  inactive: 'text-white dark:text-white hover:text-white dark:hover:text-white',}">
        <template #right >
          <form>
            <UFormGroup
              label="Contact us via the email below👇"
              :ui="{
              container: 'mt-3',
              label: {
                  base: 'block font-bold text-white dark:text-white'},
            }"
            >
              <p class="contactemail border rounded-3xl w-60 p-2 text-white pl-2 pr-1">
                hengworkingemail@gmail.com
              </p>
            </UFormGroup>
          </form>
        </template>
      </UFooterColumns>
    </template>
    <template #center>
      <p class="text-gray-500 dark:text-white text-sm">
        © {{ new Date().getFullYear() }} Holy Family College.
      </p>
    </template>
  </UFooter>
</template>
