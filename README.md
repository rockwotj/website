# redash.io

Currently this is a mashup of a Jekyll website and 2 GitBooks:

- [Main website](https://github.com/getredash/website/tree/master/website) (Jekyll)
- [User Guide](https://github.com/getredash/website/tree/master/user-guide) (GitBook)
- [On Premise Setup and Maintenance Guide](https://github.com/getredash/website/tree/master/onpremise) (GitBook)

The website is built and hosted with Netlify. When deployed, it runs the [bulid script](https://github.com/getredash/website/blob/master/bin/build):

```bash
# Build the website
jekyll build -s website/ 
# Build the user guide and place it in the Jekyll output folder:
gitbook build user-guide _site/help
# Build the on-premise guide and place it in the Jekyll output folder:
gitbook build onpremise _site/help-onpremise
```

Each part can be developed separately using each tool's live preview (`serve` command).

Eventually we will switch the website to [Hugo](https://gohugo.io) based setup. Maybe the GitBooks as well.
