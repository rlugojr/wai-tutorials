---
title: Multiple Ways
status: editors-draft
order: 7
wcag_success_criteria:
  - 2.4.8
wcag_techniques:
  - G65
  - G161
  - G63
  - G127
---

Many users benefit from having different ways to access the content of a website. Some may be confused by following a long series of navigation steps to find a specific web page. Others might arrive on a page deep in the hierarchy after clicking a link on the site or other sites and want to move up the hierarchy step by step to get a better context.

## Breadcrumbs
{:.ap}

A breadcrumb navigation shows a trail from the front page of a website to the current page, with a link to every level of the hierarchy. It helps users to know where they are in the structure of the website without displaying all the sibling pages. Breadcrumb navigations are especially important on complex websites that have more than one or two levels of navigation and in cases where not every level of the navigation is immediately visible (for example when using fly-out menus).

Links in breadcrumb navigations are usually separated by arrows. If images are used for those separators, provide alternative text. The title of the current page should be the last item of the breadcrumb navigation and not linked.

Position the breadcrumb navigation near the top of the page, mark it up as a `nav` region and label it, for example “You are here:”.

{::nomarkdown}
<%= code_start() %>
{:/nomarkdown}

~~~ html
<nav class="breadcrumb" aria-label="You are here:">

		<a href="…">Home</a>

		&gt;

		<a href="…">SpaceBears</a>

		&gt;

		<span class="current">
				<span class="visuallyhidden">Current: </span>
				Cpt. Space 6 Plus
		</span>

</nav>
~~~

{::nomarkdown}
<%= code_end %>
{:/nomarkdown}

## Sitemap
{:.ap}

A sitemap is a (nested) list of all pages of a website. It can help users understand what the site contains and how content is organized. It also is an alternative to complex menu bars.

If the site map is large, it can make sense to show some levels of the hierarchy only when expanded from the user. A sitemap needs to stay updated when a page is added or deleted, should link to all sections of the site, and represent the organization of the website. See the [W3C <abbr title="Web Accessibility Initiative">WAI</abbr> sitemap](http://www.w3.org/WAI/sitemap.html) for an example.

## Search
{:.ap}

A search option helps users to find content by entering certain keywords, which is often more efficient than going through the complete navigation and identify pages whose page title relates to the topic the user has in mind. A search functionality that spell-checks the entered terms and allows synonyms further increases its usefulness for everyone, including people with disabilities.

## Multiple ways to activate functions in applications
{:.ap}

In addition to a menubar, similar functions can often be found in other sections of the application as well. For example functions can be activated by clicking icons, using the mouse context menu, or activating keyboard shortcuts.
