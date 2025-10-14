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

<footer class="md:pb-6 md:px-4">
  <Footer class="bg-transparent! max-md:text-center!">
    <FooterCopyright href="https://lugo.studio/" by="Lugo Studio" year={2025} />
    <FooterLinkGroup
      class="mt-0 flex flex-wrap justify-center text-sm text-ctp-text"
    >
      <div class="mt-4 md:mt-0 flex space-x-8 rtl:space-x-reverse">
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
</footer>
