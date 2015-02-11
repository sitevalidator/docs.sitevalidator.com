# Frequently Asked Questions

## What is Site Validator?</h3>

Site Validator is a site-wide markup validation tool. It allows you to check the validity of the markup of several pages from your website, and gives you a summary of the most common errors and warnings, with a single click.

## Why not just use the official W3C validators?

When you need to validate the HTML and CSS markup of a big site, submitting each of its individual pages on the W3C <a href="http://validator.w3.org/">HTML</a> and <a href="http://jigsaw.w3.org/css-validator/">CSS</a> validators is a slow process. Site Validator provides a simpler, faster way to validate several pages at once. Just enter your main URL and our spider will take care of crawling your site in search for pages to validate.

Also, Site Validator gives you a summary report with the grouped common errors, so you can get a big picture of what's going wrong on the markup of the site.

## Why can't some sites be scraped?

When you submit an URL for validation, we send a web spider to visit the site and get its links. Sometimes, this process that is called "scraping" fails, and it can be due to a number of reasons. Here are the most typical ones:</p>

<dl>
  <dt>Authorization required</dt>
  <dd>Sites must be publicly accessible to be validated.</dd>
  <dt>Could not be found (404)</dt>
  <dd>The URL you provided could not be found.</dd>
  <dt>Connection timed out</dt>
  <dd>The site is taking too long to respond. Retry again later, when the remote server has less traffic.</dd>
  <dt>Too many requests to remote server</dt>
  <dd>The remote server is denying us access because it is rate limiting us. Contact your sys admin to relax this rate limiting, or try again later.</dd>
</dl>

<p>If none of this explains the reason why your site is not being scraped, <a href="mailto:support@sitevalidator.com">contact us</a> and we'll help you find the cause.</p>

## How do credits work?

<p>
  For every single validation that you make using our service, you're charged 1 credit. So, for example, if you validate HTML on a site that has 30 web pages, you spend 30 credits.
  If you validate HTML and CSS, then you spend 2 credits per page, that is, 60 credits in total.
</p>
<p>
  Once you spend all your credits, you can't make more validations until your credits are recharged.
</p>

## How can I recharge my credits?

<p>
  You can have your credits recharged with a monthly or yearly subscription.
</p>
<p>
  Check out the <a href="https://app.sitevalidator.com/pricing">Plans and pricing</a> page to see what plan is best for you. If you're not sure about how many validations you need, you can buy packs of validations.
</p>

## Is there an open source version?

<p>
  Yes! There's a free, standalone version that you can install on your computer. It's packed as a Ruby gem and it's open source, so you can examine the code and contribute to it if you wish.
</p>
<p>
  You can find the <a href="https://github.com/sitevalidator/site_validator">site_validator gem at Github</a>.
</p>
