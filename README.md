Rock-Wiki-EPub
==============

A tool to post process Rock's wiki's *.md files into something suitable for epub creation using pandoc.

## Requirements
To build the final epub using Pandoc you'll need the following
* [CommandLineParser](http://commandline.codeplex.com/) - Install-Package CommandLineParser
* [Pandoc](http://johnmacfarlane.net/pandoc/installing.html)

## Steps

1. Pull the latest [Rock-ChMS.wiki](git@github.com:SparkDevNetwork/Rock-ChMS.wiki.git) repo
2. Build this project and run the `RockWikiToPandocEpub.exe -w [PATH_TO_WIKI] -p [PATH_TO_PANDOC]` executable.
3. Run the `run.bat` file that the previous step created in the `[PATH_TO_WIKI]/tmp` folder.
4. If satisfied, move the `rockdev.epub` out of the tmp folder and delete the tmp folder.

If you want a PDF, just open the epub in [Adobe Digital Editions](http://www.adobe.com/products/digital-editions/download.html) and then use the Print button to print to a PDF writer.  
Sorry, I tried setting up LaTex in Pandoc to do direct to PDF printing and finally gave up in light of this process.
