# Bella's Blog Page (Github pages)

Site generator : [Jekyll](https://jekyllrb.com/)
& Theme : [chirpy](https://github.com/cotes2020/jekyll-theme-chirpy/)

### Starting Points
- [First Impression, What is github pages](https://pages.github.com/)
- [Find a theme you like, if you also choose Chirpy, then follow this tutorial](https://chirpy.cotes.page/posts/getting-started/)
### Local run server command

```bash
bundle exec jekyll s
```

### If encounter deploy failed on github
If need to [update theme](https://chirpy.cotes.page/posts/getting-started/#upgrading),edit `Gemfile`, and remove `Gemfile.lock`. And re run above command to generate new `Gemfile.lock`.
