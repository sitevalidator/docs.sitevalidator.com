# Site Validator Docs

This is the documentation for Site Validator.

It's built with [mkdocs](http://www.mkdocs.org), a static site generator for documentation.

We use Netlify for continuous deployment and Site Validator for continuous validation, so every time we accept a pull request for this repository the pages will be automatically rebuilt, deployed to http://docs.sitevalidator.com and validated for W3C conformance.

## Running locally

```bash
git clone https://github.com/sitevalidator/docs.sitevalidator.com.git sitevalidator-docs
cd sitevalidator-docs
pip install requirements.txt
mkdocs serve
```

Now you'll be able to view the docs at http://localhost:8000/
