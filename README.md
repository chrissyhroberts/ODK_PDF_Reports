# ODK_PDF_Reports

This is a proof of concept example of how a simple R script can be used to do automate some archiving and reporting capabilities when using Open Data Kit as a tool for electronic data collection. 

The following scripts are bare bones to demonstrate the core functionality of a master control script which pipes to an R markdown document in order to carry out any necessary tasks of data handling, analysis and report/chart generation. 

It is also useful for creating an archive of PDF files that can replace paper copies of forms in institutional repositories. Often ethics boards will request copies to be deposited locally and these files may be valuable in that respect. 


The first script will download everything from an ODK aggregate server via the java ODK briefcase tool. It will then create a csv file in standard 'tidy' format. Then the script will iteratively work through the csv file, sending calls to the markdown script and telling it to make a report in pdf, binding the data together with any images captured in the media folder. This being markdown, it could also output HTML (i.e. web pages), Slides, Word documents and so on. 

These scripts are rough around the edges and intentionally left at beta to show only the minimum necessary steps to achieve the basic function.

You’ll need to install latex and pandoc. I used homebrew, but many options for this.
Also need ODK briefcase java app. 

