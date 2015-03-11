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

•	http://www.gpo.gov/fdsys/pkg/BILLS-112hr4261ih/xml/BILLS-112hr4261ih.xml
•	http://www.gpo.gov/fdsys/pkg/BILLS-112hr4261ih/html/BILLS-112hr4261ih.htm
•	http://www.gpo.gov/fdsys/pkg/BILLS-112hr4261ih/pdf/BILLS-112hr4261ih.pdf
•	http://www.gpo.gov/fdsys/pkg/BILLS-112hr4261ih.zip

 

