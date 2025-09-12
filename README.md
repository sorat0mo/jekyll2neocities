## An easy to use, minimal, text focused Jekyll theme

[BearlyJekyll](https://github.com/sorat0mo/bearlyjekyll) imitates the very popular [Bear Blog](https://bearblog.dev/). It is a blogging platform that focuses on *your words*. **No ads, no tracking, almost no scripts.** It's also tiny and has a small footprint, which makes it suitable for free and budget hosts. With Jekyll, you can focus on writing your posts, let the engine do the rest for you.

This theme is a modification of [jekyllBear](https://github.com/knhash/jekyllBear/) by [knhash](https://knhash.in/).

## Disclosure

I solicited help from GitHub Copilot in helping me modify the original code. If you see snippets of your code being used here but I have not credited you, inform me.

## What's Changed?

1. Removed Life in Weeks.

2. More themes. Each of theme are unique and offers good visibility in both light and dark mode(Except geek which is always dark)

3. Removed original link animation and external link arrows. Replaced with underline for responsiveness (just like bear).

4. Added giscus for comments. It's optinal, if you don't want it, you can remove it.

5. Added limited CSP via injecting `<meta>` tags in `<head>`.

6. Added RSS and Fediverse verification.

7. Added post search to blog feed. Also added post navigation (previous and next) between posts.

8. You can use blog feed as homepage. The homepage for your blog will be list of your posts.

## Configuration

| Key                         | Description                                                                                                                                                                                                                                                                                                                                                |
|-----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `title`                     | The name of your site/blog.                                                                                                                                                                                                                                                                                                                                |
| `description`               | The subheader of your site, also used for SEO.                                                                                                                                                                                                                                                                                                             |
| `url`                       | The hostname for your site. If you are hosting on GitHub Pages, this will be your pages url, for example, `https://examples.github.io`                                                                                                                                                                                                                     |
| `baseurl`                   | The baseurl/folder your site is located. Set this to `""` if your site is located at the root of your url (see example above)                                                                                                                                                                                                                              |
| `use_CSP`                   | Implement limited CSP for GitHub Pages. Set to false IF you are serving CSP Headers elsewhere (e.g. Cloudflare/Vercel/Your server)                                                                                                                                                                                                                    |
| `orig_theme_author`         | Show Credits to jekyllBear's author, knhash?                                                                                                                                                                                                                                                                                                               |
| `author`                    | Your name.                                                                                                                                                                                                                                                                                                                                                 |
| `author_url`                | The link to jump to when clicking your name in the footer. If you did not set this, the site base url is used.                                                                                                                                                                                                                                             |
| `copyright`                 | Copyright text.                                                                                                                                                                                                                                                                                                                                            |
| `copyright_url`             | Link to the copyright/license. Leave empty if you don't have a link.                                                                                                                                                                                                                                                                                       |
| `fediverse_verify`          | An array of url to put in `` to verify your control of the website on Fediverse. Ignore if unused.                                                                                                                                                                                                                                                         |
| `site_theme`                | The color palette/theme you want. bear is the default. Current theme: bear, pine, sunset, geek                                                                                                                                                                                                                                                             |
| `blog_as_home`              | This setting is a boolean (true/false). If set to true, your homepage will become the blog feed instead. If set to false, there will be a home page and a dedicated blog page for your posts. You can edit the home page's content at `index.md`. The blog page can have a different slug than `/blog`, edit `permalink: /blog` in `blog.md` to customize. |
| `blog_tagline`              | Some lines to display atop your blog feed.                                                                                                                                                                                                                                                                                                                 |
| `giscus`                    | This group of settings is to be used if you want to add comments to your blog posts. Comment out **all** of them if you do not wish to add comments to your posts.                                                                                                                                                                                         |
| `links` and `special_links` | More links on the header. Use `links` for webpages and files in your website. Use `special_links` for external links.                                                                                                                                                                                                                                      |

## About CSP
It is a secure header meant to protect your site from XSS attacks. If you decide to add any extra resources (CSS stylesheets, external scripts), you need to add them to the CSP to whitelist them.

## To-do

- [x] Fix CSS problems
- [x] Add more themes
- [x] Add RSS feeds
- [x] Add fediverse verification
- [x] Add post search
- [x] Add post navigation
- [ ] Add blogroll/webring
- [ ] Write a detailed tutorial

## Contributing to upstream
The codebase in this differs too much from upstream, so I think it's best leave it alone. However, if you really want to, feel free to merge changes to jekyllBear.

## Deploying the site
If you use Neocities, there is `deploy2neocities.yml` in .github/workflows. You need to set the Repository Secret in *Settings* -> *Secrets and variables* -> *Actions* -> *Repository Secrets*. The name should be `NEOCITIES_API_KEY`. You can get the API key in the API tab under your site's settings page. You don't have to do anything else.

If you're looking to use it with GitHub Pages, you have 2 options:

1. Directly edit the workflow file that comes with this repo.

2. Use the one GitHub provides.

### Optional
You can use a headless CMS with this theme and almost any SSG. Check [Chris Ayers' Guide](https://chris-ayers.com/2025/06/26/mobile-cms-on-github-pages/) for more info. I did not implement headless CMS for the sake of simplicity. Though if I happen to use GitHub pages as blog again... This may happen.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
