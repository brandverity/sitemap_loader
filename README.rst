sitemap_loader
=============

A script to discover, download and parse sitemap files. For more details on sitemaps, check out: http://www.sitemaps.org/

Usage
====

You can invoke the script by passing domains in on the command line:
::
 > sitemap_loader www.example.com foobar.com

Or you can specify a file containing a newline separated list of domains like so:
::
 > sitemap_loader -f domain_list.txt

The script will print the discovered url lists to stdout and will print any errors encountered to stderr. You can capture both seperately by using redirection:
::
 > sitemap_loader example.com 1> results 2> errors
