# wrong-links
A Python script that helps you find internal links pointing to the wrong page (for SEO).
All you need is your All Inlinks report from Screaming Frog, and the keyword ranking reports from aHrefs or SEMrush (or anywhere as long as the columns are renamed to [Keyword | Ranking Position | Top Ranking URL]. Delete all other columns).

Upload these two CSV files and the script/tool will output these three CSV files:

Multiple Destinations: When the same keyword/phrase links to more than one URL/page. The script has built in cleanup to help with navigation links (it's best to filter those out of the crawl in the first place) and common phrases like "click here". But you'll probably still have to do a little cleanup (e.g. "see our article"). You'll see the anchor text, destination, number of links with that anchor text to that destination, the percentage of that anchor text linking to that destination (compared to other destination/s) and the source URL containing the link.

Inconsistencies by Most Links: When the page being linked to is not the page/url with the most links. You'll see the anchor text, destination, recommended destination, anchor text, number of links, and the "reason" a different URL is being recommended as a better link destination (e.g. "this other page has ten links and this page only has 1".) The script does a good job of cleaning up noise, like pages that link to themselves with a Table of Contents, category pages or pagination URLs. You may have some manual cleanup to do as well.

Inconsistencies by Ranking: When the page being linked to is not the page ranking the highest (often because another has more links and/or is better optimized). The two inconsistencies report will have a lot of overlap. Important: Don't just give a Jr. SEO or content person this data and say "fix it" because sometimes you don't actually want the page that is ranking highest to rank the highest. Use this to identify and fix cannibalization issues or optimization problems.

Here's all you need to do:
1. Go to the link here and make a copy of the Colab Notebook: https://lnkd.in/g-PRNGZc

2. Press the "Play" button.

3. Scroll down to the area where you upload your two files, starting with All Inlinks and then the Rankings report.

4. Be ready to save the three resulting CSV files. The save windows should automatically pop-up, one at a time.
