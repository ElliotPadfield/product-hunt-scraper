# product-hunt-scraper
A playwright based scraper for product-hunt. This scraper accepts any date as an input and scrapes the list of launches for that day.

I'm currently keeping this closed source but am actively considering making this an open-source project.

## Tooling
The crawler is based on Typescript & Playwright with Crawlee for optimizations, proxy management, and lots of other helpful utils. I'm using the Apify Actor library to serve requests inc. input management and data vizualisation.

## Use Cases

This is a fantastic tool to be able to track launches. Use the dataset to identify trands around comments and upvotes as well as the most successful product categories.

Schedule the tool to run multiple times daily to access the distribution of launch times, impact of launch time on number of upvotes, and and track changes to upvotes during the day.

You can also use the 'scrape landing pages' feature to get a list of domains for the launches which can be enriched with contact data for cold email & outreach.

## Output

It will return:

- Product name
- Product tagline
- Upvote count
- Link to Product Hunt detail page
- Comment count
- Category / Tags
- Product ID
- Full resolution product image
- Landing Page URL
- Landing Page Domain (use this for email/contact enrichment)

## Access

You can access the scraper on Apify at https://apify.com/elliotpadfield/product-hunt-scraper.

I've set up a free trial to be able to get a flavor of what you can achieve. You'll also find more detailed documentation about the inputs and outputs.

You can run one-off or scheduled tasks using the Apify dashboard or use the API to connect to tools like Clay.com.

If you have questions or suggestions around pricing, please let me know.

## Tips

If you're looking to scrape launches from today, I recommend scheduling for just after 11pm Pacific (San Fransisco) Time. As Product Hunt resets at midnight Pacific each day, this allows you to scrape the most possible results for each day. Alternatively, you can scrape the results from any previous day, using the date selectors.

If you don't need the landing page URL/domain, leave the 'Scrape Landers' option unchecked. This will speed up your crawl. 

