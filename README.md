# netlify-website-template

Example of PyLadies Website theme powered by Netlify with [a standard pull request template](github.com/pyladies/netlify-website-template/PULL_REQUEST_TEMPLATE). You can preview the template [here](https://distracted-payne-504b82.netlify.app/).

## What is Netlify?

Netlify is a simple tool to use for continuous integration and continuous development (CI/CD). It allows you to specify custom build commands as well as run checks in your pull requests. You can additionally get a deploy preview of your website capturing the changes generated in a pull request on a Netlify hosted url. Here's [an example pull request](https://github.com/pyladies/netlify-website-template/pull/1) to see the checks and deploy.

## Setting up you website with Netlify

1. Fork the repo.
2. We advise replacing `master` with `main` as the [default branch](https://docs.github.com/en/github/administering-a-repository/setting-the-default-branch). 
3. Register for a Netlify account. [Open source teams qualify for free OSS accounts](https://www.netlify.com/legal/open-source-policy/), use your `pyladies` chapter email address when creating your account. You'll need to host a Netlify badge on your website. Please note that any overages will be additionally charged.
4. Setup your site with [these directions](https://www.netlify.com/blog/2016/10/27/a-step-by-step-guide-deploying-a-static-site-or-single-page-app/). As this is a simple html and css website there is no need for custom build steps.
4. If you have requested a [custom domain](https://github.com/pyladies/pyladies/README.md) you can configure that within [your Netlify site](https://www.netlify.com/blog/2020/03/26/how-to-set-up-netlify-dns-custom-domains-cname-a-records/).

## Template Information

- Main file you'll update is `index.html` where you can add organizer information, your own chapter branding, contact links for your chapter, and replace the skyline image. 
- You'll want to place organizer photos can be placed in the `images/bios` directory and update the `images/skyline.jpg` with your own desired skyline image.
- If you rename the skyline image modify the `style.css` to point it to the image, look for the `.skyline` css rule.

## Local Development

If you'd like to see your changes locally you can use `Python3` to serve up the content by:

```bash
$ cd /root-of-forked-directory
$ python -m http.server # Defaults to port 8000, you can change by providing an additional integer for the desired port
```

## Option: Hosting your website on GitHub pages

GitHub provides a free hosted page for each [GitHub user](https://pages.github.com/) available at `github_username.github.io`. If using a custom domain, you can use Netlify as your CI/CD tool and instead of configuing your custom domain on the Netlify site you can add a `CNAME` into the root of your website repository (e.g. `pyladieschicago.github.io` repo name).

## Questions?

Ask for help in the [PyLadies Slack](slackin.pyladies.com) in the `#project-tech-infra` channel.

## Acknowledgements

[PyLadies NYC](http://nyc.pyladies.com/) created this theme initially, thank you!
