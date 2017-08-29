# sitemap

Sitemaps can be used to crawl and harvest content from FDsys and are available from http://www.gpo.gov/smap/fdsys/sitemap.xml and http://www.gpo.gov/smap/bulkdata/sitemapindex.xml.
 
More information about GPO's sitemap implementation is available at http://www.gpo.gov/help/index.html#sitemaps.htm. 
 
For example, sitemaps can be used to facilitate access to House legislative measures using predictable URLs over HTTP. The sitemap file for Congressional bills from 2012 is available at http://www.gpo.gov/smap/fdsys/sitemap_2012/2012_BILLS_sitemap.xml. 
 
Within the sitemap, the location of the "More Information" page for each bill is specified in the <loc> element. 
 
Example:
 
```
<url>
  <loc>http://www.gpo.gov/fdsys/pkg/BILLS-112hr4261ih/content-detail.html</loc> 
    <lastmod>2012-03-31T05:45:12.000Z</lastmod> 
    <changefreq>monthly</changefreq> 
    <priority>1.0</priority> 
 </url>
```

Content and metadata for each bill can be harvested from FDsys by creating predictable URLS with information that is derived from the <loc> element within FDsys XML sitemaps. All content and metadata files are also contained within a ZIP file.  
 
Example: 

-	http://www.gpo.gov/fdsys/pkg/BILLS-112hr4261ih/xml/BILLS-112hr4261ih.xml
-	http://www.gpo.gov/fdsys/pkg/BILLS-112hr4261ih/html/BILLS-112hr4261ih.htm
-	http://www.gpo.gov/fdsys/pkg/BILLS-112hr4261ih/pdf/BILLS-112hr4261ih.pdf
-	http://www.gpo.gov/fdsys/pkg/BILLS-112hr4261ih.zip


Additional metadata is displayed on the UI for granule-level More Information pages. Users are able to access the granule-level pages from the FDsys UI, but the sitemap points to package-level More Information pages. In order to obtain metadata, we recommend using the MODS XML metadata file. The MODS XML metadata file can be accessed directly using the pattern below and it is also contained within the ZIP file. 

Example: 
- http://www.gpo.gov/fdsys/pkg/BILLS-112hr4261ih/mods.xml
- http://www.gpo.gov/fdsys/pkg/CHRG-103hhrg71118/mods.xml

More Information page and Content Detail page are two names for the same UI HTML page. The term Content Detail apppears in the file name while links on the UI use the term More Information.


##govinfo sitemaps
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
