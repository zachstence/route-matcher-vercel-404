<script lang="ts">
  const links = [
    { href: "/project/a/b/c/page/edit", label: "Edit" },
    { href: "/project/a/b/c/page/settings", label: "Settings" },
    { href: "/org_abc123/project/a/b/c/page", label: "View" },
  ] as const;
</script>

Home

{#each links as { label, href }}
  <a style="display: block" {href}>{label}</a>
{/each}
