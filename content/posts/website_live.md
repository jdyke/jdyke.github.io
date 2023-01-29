+++
title = "New Personal Website is Live"
date = "2023-01-29T08:20:07-05:00"
author = "Jason Dyke"
authorTwitter = "jasonadyke" #do not include @
cover = ""
tags = ["", ""]
keywords = ["", ""]
description = ""
showFullContent = false
readingTime = false
hideComments = false
color = "" #color from the theme settings
+++

Over my parental leave I migrated my personal website from [Wix](wix.com) to a [Hugo](https://gohugo.io) site hosted on GitHub pages. Wix ended up costing too much for the value it provided, but I'm sure it's great for professional companies who need a no code solution.

This site runs entirely on [GitHub Pages](https://pages.github.com) which offers free hosting, automatic updates via GitHub actions, generation and rotation of SSL certificates, and best of all gives me full control over the layout and content of my own personal website.

The Hugo theme I landed on is [Terminal](https://github.com/panr/hugo-theme-terminal) which is minimal with no frills. There are a lot of cloud options available on where to host a Hugo website since it is static in nature. You can pick AWS S3, GCP GCS, Azure storage, etc. Normally I would go that route and deploy to a cloud storage service and configure a load balancer for SSL, but I wanted something where I had to do as little as possible. Enter [GitHub Pages](https://gohugo.io/hosting-and-deployment/hosting-on-github/).

Per the Hugo documentation: "GitHub provides free and fast static hosting over SSL for personal, organization, or project pages directly from a GitHub repository via its GitHub Pages service and automating development workflows and build with GitHub Actions." After migrating my domain from Wix to [GCP Cloud Domains](https://cloud.google.com/domains/docs/overview) I was ready to deploy.

To deploy and configure end to end I followed the below steps:

1. Wrote the content in Markdown
2. Created a GitHub repo with my username and "github.io": [jdyke.github.io](https://github.com/jdyke/jdyke.github.io)
3. Followed Steps [here](https://gohugo.io/hosting-and-deployment/hosting-on-github/)
4. Read GitHub's [documentation](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages) about custom domains
5. Configured DNS via the [docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site#configuring-an-apex-domain-and-the-www-subdomain-variant)
6. WAITED A DAY!! <- This is key for DNS to propagate and GitHub to fully deploy SSL and infrastructure.
7. Verified my domain via the [docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/verifying-your-custom-domain-for-github-pages)

Now to update my website it is as simple as merging code into the `main` branch and allow the [GitHub Action](https://github.com/jdyke/jdyke.github.io/blob/main/.github/workflows/gh-pages.yml) to deploy.
