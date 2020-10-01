---
layout: default
---
# Citrix Tech Zone - Subject Matter Expert Role

**Author:** [Martin Zugec](https://twitter.com/martinzugec)

## Mission Statement

Help with making sure that Tech Zone content is relevant to our audience and provide continuous support and guidance for our authors/contributors.

Subject matter expert is primarily responsible for following areas:

*  Act as primary Tech Zone contact and liaison for contributors
*  Help onboarding new contributors
*  Review and approve new content requests / ideas
*  Help with technical review of content

![Subject Matter Expert process overview](/media/role-sme-overview.jpg)

## Contacts

Following is current list of SMEs for different technologies:

| Technology | Primary | Secondary |
|------------|:-------:|-----------|
| Analytics | Ana Ruiz | Dan Feller |
| Endpoint Management | Frank Srp | Dan Feller |
| Networking | Matt Brooks | Dan Feller |
| Secure Workspace Access | Dan Feller | |
| Security | Florin Lazurca | Dan Feller |
| Workspace | Dan Feller | |

## Onboarding New Users

Every new contributor needs to get access to Tech Zone content repository hosted on GitHub.

To provide new contributor with access to the repository, the following requirements must be met:

*  Create GitHub account (recommended to use MFA)
*  Accept [contributors license agreement](https://docs.citrix.com/en-us/settings.html)
*  Learn [how to write](https://citrix.github.io/tech-marketing/projects/tech-zone/role-contributor.html#2---create-content) content for Tech Zone

[Following article](https://citrix.github.io/tech-marketing/projects/tech-zone/role-contributor.html#onboarding) provides detailed information how to create account.

**Next step:** Use [#tm-techzone-contributors](https://citrix.slack.com/archives/C011E3EMX8W) to request permissions for Tech Zone. Include email address of new contributor.

## New Content Requests

When contributors have new idea for an article, it needs to be reviewed first. If the idea is approved, a branch needs to be prepared before content can be created.

When reviewing the idea:

*  Make sure content and style is relevant for Citrix Tech Zone. If not, we can introduce author to other teams (Citrix Blogs, product documentation or Citrix Support).
*  Involve team lead of content development (Dan Feller) in this decision process
*  Make sure similar content does not exist already on Tech Zone. If it does - would it make sense to update it instead (for example add a new section)?

To publish content on Tech Zone, new branch needs to be created first. To request a branch, you need to provide information about article category and desired HTML file name.

When requesting file name:

*  Only alphabetical characters and dashes ("-") are allowed
*  Use name that will not change (for example don't use version numbers)
*  Use name that is relevant for search engines (for example don't use acronyms)
*  Look at other file names in the same category for consistency

**Next step:** Use [#tm-techzone-contributors](https://citrix.slack.com/archives/C011E3EMX8W) to request new branch. Include article category and name of your markdown file. Do NOT post this in existing thread, always post new message and tag `@martinz`.

## Review Content

After contributor is done with new article, it is time for technical review process. It is normal (even desirable) that this process is repeated multiple times during content development.

*  Review content for language, style, and consistency (making sure it is similar format as related Tech Zone articles)
*  Review technical accuracy of content. Invite other SMEs from engineering, consulting, or other groups to assist
*  If necessary (for example security topic), invite non-technical reviewers (for example legal)
*  Make sure there are no markdown violations
*  Make sure that images are following the right naming conventions

**Next step:** Use [#tm-techzone-contributors](https://citrix.slack.com/archives/C011E3EMX8W) to request Acrolinx analysis. Include name of your branch (or URL). You need to fix all spelling / deprecated terms and have a minimum Acrolinx score of 80 before article can be compiled in staging environment. Do NOT post this in existing thread, always post new message and tag `@anaru`.

## Review Staging Environment

When article is ready in staging, you need to review it one more time. URL of the article is same as in `docs.citrix.com`, but you need to be on an internal network and use `stage-docs.citrix.com`. Name of HTML file is identical to markdown file.

For example following file `\en-us\tech-zone\build\tech-papers\antivirus-best-practices.md` will be compiled as a web page with URL `https://stage-docs.citrix.com/en-us/tech-zone/build/tech-papers/antivirus-best-practices.html`.

Pay special attention to following:

*  All images are rendered properly
*  Navigation bar on the right side is relevant. Reorganize sections if needed
*  There are no white images on white background. If yes, add a black frame around them.

**Next step:** Use [#tm-techzone-contributors](https://citrix.slack.com/archives/C011E3EMX8W) to request release to production. Include name of your branch (or URL). Do NOT post this in existing thread, always post new message and tag `@martinz`.

Curious about other roles and responsibilities? You can find more information [here](https://citrix.github.io/tech-marketing/projects/tech-zone/roles-and-responsibilities.html).