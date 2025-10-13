<script lang="ts">
  import {
    Footer,
    FooterCopyright,
    FooterLinkGroup,
    FooterIcon,
  } from "flowbite-svelte";
  import {
    GithubSolid,
    TwitterSolid,
    LinkedinSolid,
  } from "flowbite-svelte-icons";
</script>

<Footer class="bg-ctp-crust!">
  <FooterCopyright href="https://lugo.studio/" by="Lugo Studio" year={2025} />
  <FooterLinkGroup
    class="mt-3 flex flex-wrap items-center text-sm text-ctp-text sm:mt-0"
  >
    <div
      class="mt-4 flex space-x-6 sm:justify-center md:mt-0 rtl:space-x-reverse"
    >
      <FooterIcon href="https://github.com/Lugo-Studio">
        <GithubSolid
          class="h-5 w-5 text-ctp-text hover:text-gray-900 dark:hover:text-white"
        />
      </FooterIcon>
      <FooterIcon href="https://twitter.com/GTLugo">
        <TwitterSolid
          class="h-5 w-5 text-ctp-text hover:text-gray-900 dark:hover:text-white"
        />
      </FooterIcon>
      <FooterIcon href="https://www.linkedin.com/in/gabriel-a-lugo/">
        <LinkedinSolid
          class="h-5 w-5 text-ctp-text hover:text-gray-900 dark:hover:text-white"
        />
      </FooterIcon>
    </div>
  </FooterLinkGroup>
</Footer>
