---
layout: default
title: Exam certification
nav_order: 8
has_children: false
---

# Frequently Asked Questions (FAQ) 
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

<br/>

---

<br/>

## Azure Search: Tier upgrade or downgrade

There is no built-in support to upgrade or downgrade tiers. If you want to switch to a different tier, the approach is:

- Create a new search service at the new tier.
- Deploy your search content onto the new service. [Follow this checklist](https://learn.microsoft.com/en-us/azure/search/search-howto-move-across-regions#prepare-and-move) to make sure you have all of the content.
- Delete the old search service once you're sure it's no longer needed.

For large indexes that you don't want to rebuild from scratch, consider using the [backup and restore sample](https://github.com/Azure-Samples/azure-search-dotnet-utilities/blob/main/index-backup-restore/README.md) to move them.


