<template>
  <header class="mx-auto max-w-5xl bg-white min-h-[60px]">
    <nav
      class="flex items-center justify-between px-4 sm:px-6 lg:px-4"
      aria-label="Top"
    >
      <!-- Logo -->

      <a href="">
        <img src="/logo.webp" class="size-14" alt="" />
      </a>

      <!-- Nav Links -->
      <div class="flex items-center">
        <a
          v-for="link in navigation"
          :key="link.name"
          class="rounded hover:bg-[#d6efff] font-body text-[13px] font-semibold text-[#3d3d3d] py-2 px-3 block whitespace-no-wrap"
          :href="link.href"
        >
          {{ link.name }}
        </a>
      </div>

      <!-- Call to action -->
      <div>
        <a
          class="bg-[#0071BC] text-white cursor-pointer hover:bg-opacity-70 font-body font-semibold text-[13px] rounded-md text-[#06071C] py-2 px-5"
          href=""
          >Contact Us
        </a>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  data() {
    return {
      navigation: [
        { name: "Home", href: "#" },
        { name: "About", href: "#" },
        { name: "Services", href: "#" },
        { name: "Testimonial", href: "#" },
      ],
    };
  },
};
</script>
