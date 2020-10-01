---
layout: default
---
# Citrix Tech Zone - Operator Role

**Author:** [Martin Zugec](https://twitter.com/martinzugec)

## Mission Statement

Responsible for all operations related to GitHub versioning and build process.

![Tech Zone process overview](/media/role-operator-overview.jpg)

## Contacts

| Technology | Primary | Secondary |
|------------|:-------:|-----------|
| GitHub | Martin Zugec | Beth Pollock |

## Adding contributors to Tech Zone

When adding new contributors to Tech Zone, it is important to make sure they've provided consent for their contribution.

1.  Make sure that SME has explained the processto contributor.
2.  Get email address associated with GitHub account.
3.  Click on "Consent settings" at the bottom right corner of [Tech Zone](https://docs.citrix.com/en-us/tech-zone.html)
4.  After authentication, click on [Dashboard](https://docs.citrix.com/en-us/settings#/dashboard/user-details) on the left side
5.  Search for new GitHub user **by email address**. Confirm that consent has been provided.
6.  Send an invitation to [Tech Zone repository](https://github.com/martinzugec-ctx/en-us-tech-zone/settings/access) by using email address associated with GitHub account
7.  Ask contributor to accept an invitation email

## Creating new branch

When creating a new branch, it is important to pay attention to naming conventions, since branch name is used for automation.

Branch name consists of following sections: `<type>_<category_name>_<article_name>`.

Following types are supported: 

*  `new` - Used when adding a new article
*  `update` - Used when updating an existing article
*  `fix` - used for changes that are not related to specific article

Category name is directly based on URL category of article. For example, for article `https://docs.citrix.com/en-us/tech-zone/build/tech-papers/antivirus-best-practices.html`, category name would be **tech-papers**. Note that it's **plural**, not singular!

Article name is directly based on HTML file of article (or markdown to be more accurate). For example, for article `https://docs.citrix.com/en-us/tech-zone/build/tech-papers/antivirus-best-practices.html`, article name would be **antivirus-best-practices**.

To update this article, branch would be called `update_tech-papers_antivirus-best-practices`.

## Synchronizing branches

When synchronizing branches between development (`martinzugec-ctx`) and production (`citrix`) GitHub organizations, follow this process.

1.  in `citrix` organization, create new branch with identical name to source branch in `martinzugec-ctx`
2.  This new branch should be always based on `master` branch
3.  Create cross-organization PR
4.  Merge changes

If there are any more changes in the future - re-synchronize these two branches again.

You MUST use intake branch to transfer changes instead of creating PR directly to `wip` or `master` branch. Markdown validation does not work across organizations and cross-org branch would never be allowed to merge.

## Release to staging

To update the staging environment, merge your changes to `wip` branch to trigger re-build. This updates [stage-docs.citrix.com](https://stage-docs.citrix.com) site. You have to be on internal citrite network to access this site.

## Release to production

To update the production environment, merge your changes to `master` branch to trigger re-build. This updates [docs.citrix.com](https://docs.citrix.com) site.

Curious about other roles and responsibilities? You can find more information [here](https://citrix.github.io/tech-marketing/projects/tech-zone/roles-and-responsibilities.html).