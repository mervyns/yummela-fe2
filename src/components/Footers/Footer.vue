<template>
  <footer
    class="pb-6"
    :class="[absolute ? 'absolute w-full bottom-0 bg-gray-900' : 'relative']"
  >
    <div class="container mx-auto px-4">
      <hr class="mb-6 border-b-1 border-gray-700" />
      <div
        class="flex flex-wrap items-center md:justify-between justify-center"
      >
        <div class="w-full md:w-4/12 px-4">
          <div
            class="text-sm text-gray-600 font-semibold py-1 text-center md:text-left"
          >
            Copyright © {{ date }}
            <a
              href="https://www.yummela.co/"
              class="text-white hover:text-gray-400 text-sm font-semibold py-1"
            >
              yummela.co
            </a>
          </div>
        </div>
        <div class="w-full md:w-8/12 px-4">
          <ul class="flex flex-wrap list-none md:justify-end justify-center">
            <li>
              <a
                href="https://yummela.co/privacy-notice"
                class="text-white hover:text-gray-400 text-sm font-semibold block py-1 px-3"
              >
                Privacy Notice
              </a>
            </li>
            <li>
              <a
                href="https://www.yummela.co/about-us"
                class="text-white hover:text-gray-400 text-sm font-semibold block py-1 px-3"
              >
                About Us
              </a>
            </li>
            <li>
              <a
                href="https://random.co"
                class="text-white hover:text-gray-400 text-sm font-semibold block py-1 px-3"
              >
                MIT License
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  props: {
    absolute: {
      type: Boolean,
      default: false,
    },
  },
  data() {
    return {
      date: new Date().getFullYear(),
    }
  },
}
</script>
