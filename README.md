# sitemap

GPO is pleased to release [sitemaps](https://www.govinfo.gov/sitemaps) for govinfo. These sitemaps are functionally similar to the existing FDsys sitemaps, though the structure has been streamlined to make it easier to track updates to specific collections.

Where FDsys had a `sitemap_year/year_collection_sitemap.xml` format, govinfo provides each sitemap at the `collection_year` level more directly. 


Please provide feedback on this repository as we seek to make the govinfo sitemaps more useful to all of our users.

govinfo sitemaps provide direct access to the details pages, where the different formats of content and metadata may be downloaded, including through the use of the package-level mods.xml file, located at https://www.govinfo.gov/metadata/pkg/{accessID}/mods.xml.

```
<url>
  <loc>
  https://www.govinfo.gov/app/details/BILLS-115hjres93ih
  </loc>
  <lastmod>2017-06-21T19:58:14.558Z</lastmod>
  <changefreq>monthly</changefreq>
  <priority>1.0</priority>
</url>
```

The mods.xml file for the sample sitemap entry may be found at:
https://www.govinfo.gov/metadata/pkg/BILLS-115hjres93ih/mods.xml
