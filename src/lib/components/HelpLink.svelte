<script lang="ts">
  import { tabs } from "webextension-polyfill";

  function openGitHubIssuesPage(): void {
    tabs.create({
      url: "https://github.com/scolton99/tdx-extension/issues",
      active: true,
    });
    window.close();
  }
</script>

<button
  on:click={openGitHubIssuesPage}
  class="group flex items-center rounded-md px-2 py-2 text-xs font-medium text-purple hover:text-purple-light dark:text-purple-light  dark:hover:text-gray-300 transition-all duration-300 ease-in-out"
>
  <svg
    class="mr-1 h-4 w-4  "
    xmlns="http://www.w3.org/2000/svg"
    fill="none"
    viewBox="0 0 24 24"
    stroke-width="2"
    stroke="currentColor"
    aria-hidden="true"
  >
    <path
      stroke-linecap="round"
      stroke-linejoin="round"
      d="M9.879 7.519c1.171-1.025 3.071-1.025 4.242 0 1.172 1.025 1.172 2.687 0 3.712-.203.179-.43.326-.67.442-.745.361-1.45.999-1.45 1.827v.75M21 12a9 9 0 11-18 0 9 9 0 0118 0zm-9 5.25h.008v.008H12v-.008z"
    />
  </svg>
  Help
</button>
