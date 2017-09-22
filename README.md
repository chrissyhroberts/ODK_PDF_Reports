# ODK_PDF_Reports

Several of my users have asked me if there is a simple way to convert individual records from ODK in to PDF files. This is pretty useful if you are running ODK for scientific research studies where ethics boards insist that data collection sites retain hard copies of data forms.

I’ve written these scripts for my own use but thought that they might be useful to some others who have similar need. They are a pair of R scripts, one in R markdown. The first will download everything via java ODK briefcase tool and create a csv file. Then they iteratively work through the csv file, sending calls to the markdown script and telling it to make a report in pdf, binding the data together with any images captured in the media folder.

I’m no hardcore programmer, so these scripts are rough around the edges. Feel free to mod, improve and repost.

You’ll need to install latex and pandoc. I used homebrew, but many options for this.

