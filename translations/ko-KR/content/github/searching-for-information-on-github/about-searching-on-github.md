---
title: About searching on GitHub
intro: 'Use our powerful search tools to find what you''re looking for among the many repositories, users, and lines of code on {{ site.data.variables.product.product_name }}.'
redirect_from:
  - /articles/using-the-command-bar/
  - /articles/github-search-basics/
  - /articles/search-basics/
  - /articles/searching-github/
  - /articles/advanced-search/
  - /articles/about-searching-on-github
versions:
  free-pro-team: '*'
  enterprise-server: '*'
---

You can search globally across all of {{ site.data.variables.product.product_name }}, or scope your search to a particular repository or organization.

- To search globally across all of {{ site.data.variables.product.product_name }}, type what you're looking for into the search field at the top of any page, and choose "All {{ site.data.variables.product.prodname_dotcom }}" in the search drop-down menu.
- To search within a particular repository or organization, navigate to the repository or organization page, type what you're looking for into the search field at the top of the page, and press **Enter**.

{% note %}

**참고:**

- {{ site.data.reusables.search.required_login }}
- {{ site.data.variables.product.prodname_pages }} sites are not searchable on {{ site.data.variables.product.product_name }}. However you can search the source content if it exists in the default branch of a repository, using code search. For more information, see "[Searching code](/articles/searching-code)." For more information about {{ site.data.variables.product.prodname_pages }}, see "[What is GitHub Pages?](/articles/what-is-github-pages/)"

{% endnote %}

After running a search on {{ site.data.variables.product.product_name }}, you can sort the results, or further refine them by clicking one of the languages in the sidebar. For more information, see "[Sorting search results](/articles/sorting-search-results)."

{{ site.data.variables.product.product_name }} search uses an ElasticSearch cluster to index projects every time a change is pushed to {{ site.data.variables.product.product_name }}. Issues and pull requests are indexed when they are created or modified.

### Types of searches on {{ site.data.variables.product.prodname_dotcom }}

You can search the following types of information across all public {{ site.data.variables.product.product_name }} repositories, and all private {{ site.data.variables.product.product_name }} repositories you have access to:

- [Repositories](/articles/searching-for-repositories)
- [Topics](/articles/searching-topics)
- [Issues and pull requests](/articles/searching-issues-and-pull-requests)
- [Code](/articles/searching-code)
- [Commits](/articles/searching-commits)
- [Users](/articles/searching-users){% if currentVersion == "free-pro-team@latest" %}
- [Packages](/github/searching-for-information-on-github/searching-for-packages){% endif %}
- [Wikis](/articles/searching-wikis)

### Searching using a visual interface

Alternatively, you can search {{ site.data.variables.product.product_name }} using the {{ site.data.variables.search.search_page_url }} or {{ site.data.variables.search.advanced_url }}.

The {{ site.data.variables.search.advanced_url }} provides a visual interface for constructing search queries. You can filter your searches by a variety of factors, such as the number of stars or number of forks a repository has. As you fill in the advanced search fields, your query will automatically be constructed in the top search bar.

![Advanced Search](/assets/images/help/search/advanced_search_demo.gif)

### Searching across {{ site.data.variables.product.prodname_enterprise }} and {{ site.data.variables.product.prodname_dotcom_the_website }} simultaneously

If you use {{ site.data.variables.product.prodname_enterprise }} and you're a member of a {{ site.data.variables.product.prodname_dotcom_the_website }} organization using {{ site.data.variables.product.prodname_ghe_cloud }}, your {{ site.data.variables.product.prodname_enterprise }} site administrator can enable {{ site.data.variables.product.prodname_github_connect }} so that you can search across both environments at the same time. For more information, see "[Enabling {{ site.data.variables.product.prodname_unified_search }} between {{ site.data.variables.product.prodname_enterprise }} and {{ site.data.variables.product.prodname_dotcom_the_website }}](/enterprise/admin/guides/developer-workflow/enabling-unified-search-between-github-enterprise-server-and-github-com)."

You can only search across both environments from {{ site.data.variables.product.prodname_enterprise }}. To scope your search by environment, you can use a filter option on the {{ site.data.variables.search.advanced_url }} or you can use the `environment:` search prefix. To only search for content on {{ site.data.variables.product.prodname_enterprise }}, use the search syntax `environment:local`. To only search for content on {{ site.data.variables.product.prodname_dotcom_the_website }}, use `environment:github`.

Your {{ site.data.variables.product.prodname_enterprise }} site administrator can enable {{ site.data.variables.product.prodname_unified_search }} for all public repositories, all private repositories, or only certain private repositories in the connected {{ site.data.variables.product.prodname_ghe_cloud }} organization.

If your site administrator enables {{ site.data.variables.product.prodname_unified_search }} in private repositories, you can only search in the private repositories that the administrator enabled {{ site.data.variables.product.prodname_unified_search }} for and that you have access to in the connected {{ site.data.variables.product.prodname_dotcom_the_website }} organization. Your {{ site.data.variables.product.prodname_enterprise }} administrators and organization owners on {{ site.data.variables.product.prodname_dotcom_the_website }} cannot search private repositories owned by your account. To search the applicable private repositories, you must enable private repository search for your personal accounts on {{ site.data.variables.product.prodname_dotcom_the_website }} and {{ site.data.variables.product.prodname_enterprise }}. For more information, see "[Enabling private {{ site.data.variables.product.prodname_dotcom_the_website }} repository search in your {{ site.data.variables.product.prodname_enterprise }} account](/articles/enabling-private-github-com-repository-search-in-your-github-enterprise-server-account)."

### 더 읽을거리

- "[Understanding the search syntax](/articles/understanding-the-search-syntax)"
- "[Searching on GitHub](/articles/searching-on-github)"