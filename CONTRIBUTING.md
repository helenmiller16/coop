# Guidelines for contributing to The Coop blog

We welcome submissions from any members of the [Coop Community](https://research.fhcrc.org/coop/en.html)!

The content below includes:
- [What kind of posts are appropriate for our blog?](#what-kind-of-posts-are-appropriate-for-our-blog)
- [Required content for a blog post](#required-content-for-a-blog-post)
- [Contribute via email](#contribute-via-email)
- [Contribute via GitHub](#contribute-via-github)
- [Adding yourself as a contributor](#adding-yourself-as-a-contributor)
- [Errata](#errata) (for the Coop blog maintainers: reviewing posts, publishing, and changing site layout)

## What kind of posts are appropriate for our blog?

Each post published here belongs to at least one of our three main categories:
 - *Community*: announcements and explanations about Coop events and programs
 - *Technical*: descriptions of tools and approaches used by our data-intensive research community and support staff
 - *Science*: reports on new and interesting research findings from our community using data and computational methods

Possible content includes:
- repost content from your own blog
- description of a new data-oriented tool you're using
- report from a community group meeting
- announcements about events
- anything else you think would be of interest to the broader community!

For some ideas, check out our [GitHub issues for potential blog topics](https://github.com/fredhutch/coop/issues?q=is%3Aissue+is%3Aopen+label%3Apost). Also feel free to file an issue if there is a topic you'd like to see discussed!

## Required content for a blog post

- **Title:** A short, catchy description of to entice readers
- **Category:** Community, Technical, or Science, as described [above](#what-kind-of-posts-are-appropriate-for-our-blog)
- **Tags:** Suggested keywords that can help readers find information from among our blog posts
- **Blog content:** This is the body of the blog post! We recommend relatively short posts (no more than five paragraphs), equivalent to a three minute read. Pictures and links to other sites are also great!

## Contribute via email

If you'd like to submit a blog post and don't want to deal with technical details, please email your [content](#required-content) to `coophelp` at `fredhutch.org`

## Contribute via GitHub

This blog is published through [GitHub](https://github.com), and we are happy to accept submissions via pull requests. If you are new to GitHub or haven't worked collaboratively, please feel free to email `coophelp` at `fredhutch.org` to meet with one of the Coop blog maintainers to walk you through the process.

- Fork the [repository](https://github.com/FredHutch/coop)
- In your fork, create a new branch with a name that reflects your blog post (e.g., `python-december`)
- Copy the [markdown blog post template](/drafts/TEMPLATE-post-title.md) to a new file named to reflect your post (e.g., `python-december.md`)
- Modify the header and body of the template to reflect [required content](#required-content), save to the [drafts folder](/drafts/), and commit to your branch
- Submit a PR to the `gh-pages` branch in [this repository](https://github.com/FredHutch/coop)

The Coop blog maintainers will review your content and ask for clarification if needed. When everyone is satisfied, we'll accept the pull request and arrange for the post to be published.

## Adding yourself as a contributor

More information coming soon!

## Errata

The information below is for maintainers of this blog (members of the team coop-blog-maintainers). This includes:
- [Reviewing and publishing blog posts](#reviewing-and-publishing)
- [Formatting and layout](#formatting-and-layout)

### Reviewing and publishing

Submitted posts are reviewed, edited, and published by the Coop blog maintainer team.

For team members:

- Pull requests (PR) are accepted from contributors forking the repository and adding a new file to the [drafts folder](#drafts).
- Review the pull request to ensure all [required content](#required-content) is present, and also edit for grammar, spelling, and formatting.
- Accept/merge the PR when the content meets requirements, ensuring the file is located in the [drafts folder](#drafts).
- Change the filename to include the required [`YEAR-MONTH-DAY-title.md` format](https://mmistakes.github.io/minimal-mistakes/docs/posts/) and ensure the [front matter](https://jekyllrb.com/docs/front-matter/) is accurately formatted. Extra notes on front matter:
  - `categories` should be one or more of `Science`, `Technical`, `Community` (note capitalization)
  - `tags` should be lowercase
  - `last_modified_at` is only required to override the date in the filename
- If necessary, build the site locally to [render posts in the drafts folder](https://jekyllrb.com/docs/posts/#drafts) prior to publishing.
- Publish the post by moving it to the [posts folder](/posts/), and notify the submitter when it is available.
- If a submission is received via email, one of the team members will create a new branch and add the post to the drafts folder, then create the pull request and proceed as described above.

### Tags

Tags should appear in lowercase, and may represent a variety of different characteristics.

### Formatting and layout

- This blog renders from the `gh-pages` branch.
- The template for the blog is [Minimal Mistakes Jekyll theme](https://github.com/mmistakes/minimal-mistakes). The following links and language were included in the original README and are copied here for convenience:
  - Please see [this page](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) for additional information on configuration.
  - If you have a question about using Jekyll, start a discussion on the [Jekyll Forum](https://talk.jekyllrb.com/) or [StackOverflow](https://stackoverflow.com/questions/tagged/jekyll).
  - [Ruby 101](https://jekyllrb.com/docs/ruby-101/)
  - [Setting up a Jekyll site with GitHub Pages](https://jekyllrb.com/docs/github-pages/)
  - [Configuring GitHub Metadata](https://github.com/jekyll/github-metadata/blob/master/docs/configuration.md#configuration) to work properly when developing locally and avoid `No GitHub API authentication could be found. Some fields may be missing or have incorrect data.` warnings.
- Additional modifications for the blog theme are from:
  - [Bioinformatics Interest Group (FHBig)](https://fredhutch.github.io/FHBig/)
  - [Fred Hutch Biomedical Data Science Wiki](https://sciwiki.fredhutch.org)