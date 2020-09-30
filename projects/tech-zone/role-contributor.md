---
layout: default
---
# Citrix Tech Zone - Contributor Role

**Author:** [Martin Zugec](https://twitter.com/martinzugec)

## Welcome to Tech Zone

Welcome to the documentation project for [techzone.citrix.com](https://techzone.citrix.come)! Citrix Tech Zone is home for technical, in-depth articles that are inspired and driven by technical communities and enthusiasts. Whether you are an architect, consultant, engineer, or technical IT manager, you have come to the right place!

Tech Zone has always been oriented towards technical community, but now you can help us to make it better by suggesting changes or even writing the whole articles to share with fellow Citrix fans.

![Tech Zone process overview](/media/role-contributor-overview.jpg)

## Contact Tech Zone administrators

If you need any help, reach out to Tech Zone team. Preferred method of contacting Citrix Tech Zone team is through one of the dedicated Slack channels. For Citrix employees, use an internal Slack channel [#tm-techzone-contributors](https://citrix.slack.com/archives/C011E3EMX8W). For everyone else, use the [Tech Zone Slack channel](https://worldofeuc.slack.com/messages/CLKSAPFUG) at [World of EUC](https://communityinviter.com/apps/worldofeuc/world-of-euc-project) workspace.

If you prefer to use email, you can also reach out to us using [email](mailto:Tech-Content-Feedback@citrix.com).

## Onboarding

Before you can start writing new articles, you need to create a GitHub account and get permissions to Tech Zone content repository. Citrix Tech Zone backend is based on GitHub from Microsoft.
After you account is created with required permissions, you will also need to access contibutors agreement and let us know if you want your name displayed as contributor.

### Create an account

There are two different methods how you can become one of the contributors, depending on whether or not you are a Citrix employee.

#### Citrix employees

1.  Create your GitHub account with two-factor authentication enabled
2.  Accept contributors agreement: [https://docs.citrix.com/en-us/settings.html](https://docs.citrix.com/en-us/settings.html). **This is a required step!**
3.  Send us your GitHub user name (see [Contact Tech Zone administrators](#contact-tech-zone-administrators) section)
4.  Wait for validation email – you have to accept this invitation to become one of the Tech Zone contributors
5.  Make sure that correct name and email address is configured in your GitHub Desktop (`File -> Options -> Git`)

#### Everybody else

Follow this [simple guide](https://citrix.github.io/tech-marketing/projects/tech-zone/crowdsourcing.html) to become one of our contributors.

## 1 - Request a branch

To make any changes to Tech Zone, you have to use a dedicated branch (think about it as an isolated clone of Tech Zone only to be used for your new article or update of an existing article). Branch is required for new articles, but also if you are going to update an existing article.

Another approach is to use you own fork of Tech Zone and just create a pull request, but this approach is recommended only for advanced GitHub users. If you are familiar with private forks and concept of pull requests, you can use this method.

1.  Use one of the dedicated Slack channels to request a new branch. For new article, specify section of Tech Zone (e.g. Tech Insight) and title of the article (e.g. "Workspace app"). For existing, simply paste a URL.
2.  Wait for link to your new branch. You get it through Slack or by email from Tech Zone team.
3.  When you click on link, GitHub web editor opens with article you are working on. Read [Visual Studio Code (VSC) guide](https://citrix.github.io/tech-marketing/projects/tech-zone/visual-studio-code-guide.html) to learn how to create a local copy of this branch for editing.

Your request for new branch will be reviewed by one of our subject matter experts (SME). SME is going to become your best friend - he will be your primary contact for everything Tech Zone related, help you with the content creation and take care of your doing the whole review and release process.

## 2 - Create content

As many other large companies (for example Microsoft or Amazon), we are using de-facto industry standard language called markdown to create Tech Zone content. Markdown language is a simple, lightweight language that is easy to learn and allows us to create dynamic content. Think about markdown as a text-to-HTML conversion tool. It is highly recommend to read the [most common mistakes](#most-common-mistakes) section first - there is a learning curve and this short list can greatly help you to quickly learn this language.

As a markdown editor, we recommend to use [Visual Studio Code (VSC)](https://citrix.github.io/tech-marketing/projects/tech-zone/visual-studio-code-guide.html). Don't be discouraged by Visual Studio in name - this tool is not only for developers, but useful as a general text editor. Be aware that editing GitHub content in browser is not supported at the moment and you need to make sure that correct name/email is configured in GitHub Desktop.

### Writing text

To learn more about markdown syntax, you can read many articles online and read some of the (many) available [cheatsheets](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

Few additional recommendations:

*  Keep your sentences short--26 words or fewer
*  Write in a personal, friendly style. Do not use the style of academic discourse. Avoid using unusual words if there is a simpler variant
*  Write in present tense. For example, "the product reports the result" instead of "the product will report the result."

**IMPORTANT:** Only edit your article and image files. Many sections of the Tech Zone (e.g. landing page) are generated automatically and you don't need to care about them.

### Adding images

Our readers love images, so include as many as you need to get your message across. All images must be placed in the **/media** folder of the Tech Zone repo and you can upload them through GitHub website.

**IMPORTANT:** Make sure that you are using the right branch AND right naming conventions when uploaded files. Don't use web GitHub.com to upload images, instead use the Visual Studio Code. Naming conventions are important for Tech Zone, file names are used as part of release automation.

To add images to your article, you need to do following:

1.  Prepare images using the right naming conventions (instructions below). This is important for our automation
2.  Upload images to section /media folder (this is under learn/design/build folder). Make sure you are using the [correct branch](#using-the-right-fork--branch)
3.  Reference those images in your markdown code (instructions below)

Image conventions:

*  Use PNG format for images
*  Only lower-case characters and dashes (`-`) are allowed. Underscore is reserved (see below)
*  Use basic grayscale colors and icons / diagrams from brand team to create diagrams. Look at other Tech Zone content to follow same style and format.
*  When your image has white background (e.g. screenshots from Citrix Cloud), add a 1px black frame around that picture. White on white does not look good.
*  File name is using format `(category-name)_(article-name)_(image-name)`, where `category-name` and `article-name` are based on URL of the target article. For example tech-briefs_workspace-app_overview.png. “Category” is identical to category section of URL (e.g. ‘’/reference-architectures/”) and “article name” is identical to file name of the article (.md or .html file). `image-name` can be any format that you prefer, however it is recommended to use descriptive names.
*  Underscore character (`_`) is used as delimiter and you should not use it in image name. Feel free to use hyphen in image name instead. Each image file name should contain exactly 2 underscore characters.

When you are referencing your images in markdown language, you can use two different syntaxes.

For simple images (screenshots), use format `![descriptive text](image URL)` with relative URL, for example `/en-us/tech-zone/design/media/design-decisions_provisioning-solutions_diagram-explicit.png`.

For images that should open full screen after clicking them, use format `[![descriptive text](image URL)](image URL)`. This will open image after reader clicks on it. This is typically recommended for images such as diagrams.

### Using tables

Tables are discouraged for modern articles - it is complicated to maintain them in markdown, they have limited functionality (e.g. markdown doesn't support bullet points in tables or multiple paragraphs) and articles with tables are penalized by search engines like Google or Bing (content is marked as not being mobile friendly). If you really need to include a table in your article, use one of the many online generators (for example [this one](https://www.tablesgenerator.com/markdown_tables)).

Generally - if you need to use multiple paragraphs of text, bullet points inside tables or multiple nested tables, you should consider to break down table to use native markdown format. If each cell of your table contains only one word or one sentence, table is perfectly valid option.

## 3 - Review and Release Content

When you are ready for content review, contact Tech Zone team. After technical, styling and grammar reviews are complete, you content will be released. Before asking for review - please make sure there are no markdown violations in your file (this is reported by Visual Studio Code). Subject matter expert will help you and guide you through review process.

## Most Common Mistakes

For contributors, basic understanding of markdown language and versioning (GitHub) is required. When working on Tech Zone content, we have seen few issues that are frequently occurring and we would like to cover them in this section.

### Using the right fork / branch

Versioning systems (like Git or Subversion) are useful for professional developers (especially for large and complicated projects), however they can be confusing for non-developers. While learning about versioning systems, pull requests and protected branches is definitely worth your time, you should follow few simple rules when working on Tech Zone content if you are not 100% comfortable with these advanced concepts:

*  For any change to Tech Zone, you need a branch - this is required so that you don't impact other contributors. If you don't have a branch, contact one of the administrators
*  Make sure you are using "martinzugec-ctx" fork (not your personal or Citrix fork)
*  Never try to make any changes to `wip` or `master` branches (protected branches)

**To fix:** Always confirm that you are using the right branch before making any changes.

### Changes not uploaded to GitHub

When you make changes on your local machine, you need to not only save them (`commit` in git terminology), but also upload to central database (`push` in git terminology). Always make sure that you are doing both commit and push operations.

**Note:** All your content development is done in a dedicated branch. You can push changes as often as you want and there is nothing that you can do that would have negative impact on Tech Zone.

### Spaces after list markers

Standard markdown syntax requires one space after list character. Tech Zone implementation requires 2 spaces after list character. This should be correctly reported by Visual Studio Code if you have followed all instructions in configuration guide.

    - One Space - NOT correct
    -  Two spaces - correct

### Absolute links to docs.citrix.com

Normal format of links in markdown language is `[text](https://url.com)`. However, when referencing content hosted on docs.citrix.com, you should use relative links only, starting with `/en-us/`. For example if you want to reference `https://docs.citrix.com/en-us/citrix-virtual-apps-desktops-service.html`, you should use syntax `[Citrix Virtual Apps and Desktops service](/en-us/citrix-virtual-apps-desktops-service.html)`. This is important to support other languages - relative links are automatically converted to localized language if page is available.

Curious about other Tech Zone roles and responsibilities? You can find more information [here](https://citrix.github.io/tech-marketing/projects/tech-zone/roles-and-responsibilities.html).