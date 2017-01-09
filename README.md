# RSS Sitemap for Textpattern CMS
RSS Sitemap for most recent articles to be used with an XML Sitemap. Objective: increasing your SEO.


XML Sitemaps are intented to describe all the pages of a website. 
But they suffer from an indexation infrequent by bots. Fortunately, RSS Sitemaps are used for most recent pages and are read daily by bots (that's the reason for their existence).

To be use in conjonction with an XML Sitemap (rah_sitemap plugin or other handmade solution):

__Note__: you will need [the aks_header plugin](http://forum.textpattern.com/viewtopic.php?id=31479) in order to set the correct xml header for your RSS sitemap.

Copy/paste this [form template](https://github.com/cara-tm/RSS-Sitemap-for-Textpattern-CMS/blob/master/form/sitemap_articles_rss) into a new form named __sitemap_article_rss__.

Copy/Paste this [page template](https://github.com/cara-tm/RSS-Sitemap-for-Textpattern-CMS/blob/master/page/sitemap_rss) into a new page named __sitemap_rss__.

Finally, associate this page to a new section named __sitemap-rss__ (This page will be never indexed by bots).

That's all.

Notify this RSS page (__/sitemap-rss__) into your Google Search Console account to tell the bot to crawl it.
Because a blank page with a '304 Not Modified' header will be send if no recent articles are present, please first time submit this page to Google when creating new articles.

The __siemap_article_rss__ form invokes the new (TXP 4.7.0) `<txp:evaluate />` tag. [Check the second file option for previous Textpattern CMS versions](https://github.com/cara-tm/RSS-Sitemap-for-Textpattern-CMS/tree/master/form).

##Informations

[Google recommends use both XML and alternative sitemaps for SEO optimisation.](http://googlewebmastercentral.blogspot.ca/2014/10/best-practices-for-xml-sitemaps-rssatom.html)
