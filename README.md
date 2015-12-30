```
                     ________                            
M               M   /_  __/ /  ___                       
M M           M M    / / / _ \/ -_)                      
M M M       M M M   /_/_/_//_/\__/         __        ____
M M M M   M M M M     /  |/  /__ ________ / /  ___ _/ / /
M M M M M M M M M    / /|_/ / _ `/ __(_-</ _ \/ _ `/ / / 
M M M M M M M M M   /_/__/_/\_,_/_/ /___/_//_/\_,_/_/_/  
M M M M M M M M M     / _ \_______    (_)__ ____/ /_     
M M M M M M M M M    / ___/ __/ _ \  / / -_) __/ __/     
M M M M M M M M M   /_/  /_/  \___/_/ /\__/\__/\__/     
                                 |___/  
```

#The Department of Justice's 14141 civil rights investigations

The Civil Rights Division of the U.S. Department of Justice conducts its broad “pattern or practice” investigations of local law enforcement agencies under a 1994 law that took shape after the beating of Rodney King by white officers of the Los Angeles Police Department.

That statute, known as 14141 after its section of the U.S. Code, allows the Justice Department to investigate almost any report of police actions that suggest a pattern of violations of citizens’ constitutional civil rights. Where the allegations are upheld, the department can seek agreement with local governments on policing reforms or – as it has done more aggressively under President Barack Obama – go to the federal courts to force changes under closely monitored consent decrees.

Our story, "[Policing The Police](https://www.themarshallproject.org/2015/04/23/policing-the-police)," published by [The Marshall Project](https://www.themarshallproject.org/) with [Time.com](http://time.com/police-shootings-justice-department-civil-rights-investigations/) on April 23, 2015, examined the use of 14141 investigations during the last three presidencies.

Included in this repo is [the table](data/20150423doj_data.csv) of data The Marshall Project used to analyze and visualize the 14141 investigations since the law's inception. We also have [a current table of pattern and practice investigations](data/doj_data.csv) currently underway. If you'd like to use the data, please read on for its genealogy and caveats about its limitations.

##Data sources and caveats
This data began with [a PDF provided by the Department of Justice](data/Copy%20of%20ALL%20Authorized%2014141%20LEA%20investigations%20EVER%207-2-14%20to%20Marshal%20Project%202.pdf) in late 2014 that listed all of the 14141 investigations and their current status. To fill in the start dates and other background on the disposition of the cases, we combed through many other sources:

- Interviews with Justice Department sources.
- a [2011 Department of Justice report](https://ncjrs.gov/pdffiles1/nij/234458.pdf) on 14141 investigations.
- a [2014 Fordham Law Review study](http://ir.lawnet.fordham.edu/cgi/viewcontent.cgi?article=5011&context=flr) of "Federal Enforcement of Police Reform"
- The Civil Rights Division's Special Litigation Section's [case documents and summaries](http://www.justice.gov/crt/about/spl/findsettle.php).
- Contemperaneous news coverage in local and national publications.

We restricted our look at 14141 solely to investigations of police agencies. The statute is also applied to jails, juvenile facilities and other institutions. Because many of these cases are ongoing, the csv we created in ```data/20150423doj_data.csv``` should be considered a snapshot in time from April 23, 2015. In the coming weeks or months, this picture could change considerably as some investigations reach settlement agreements or others are opened. We'll do our best to keep [the current investigations table](data/doj_data.csv) updated.

The quality of the data sources varied greatly. The 2011 Justice Department report "Taking Stock" includes some investigations of jails, for instance, that were beyond the scope of our reporting. It was missing dates in some cases and only included months and years of when investigations began. The Fordham Law Review also had some incorrect dates, where months and days were transposed, or individual cases were absent. We went to great pains to get the most up-to-date status of the cases along with exact dates of starting and settlement. When several sources conflicted, we deferred to our DoJ sources and the original PDF we received from the department.

In the start_date column, we tried to get exact dates wherever possible. Because one of the goals of our reporting was to count the cases by presidential administration and term, if we couldn't get the date, the month and year would suffice. In those cases, the date was coded as the first of the month. For example, when you see an investigation that was begun on 11/1/1997, it was likely because the best source we could find only indicated it started in November of 1997. Tread carefully.

To determine how and when a case was settled, we used the ```status_result``` column and the date of either an agreement of some form (a consent decree or a memorandum of agreement) or a "closed with agreement" desgination from the DoJ. Based on those, we could classify the administration that closed each type of case over time. Any cases that were still being litigated or have not reached a settlement were coded as "Ongoing" and were omitted from our bar chart of case closures.

##Additional resources
For finding background information on the DOJ's pattern and practices investigations, also try the [Civil Rights Litigation Clearinghouse](http://www.clearinghouse.net/) at the University of Michigan, which posts key documents about many cases, particularly older ones.

##Contributors

* Tom Meagher, [The Marshall Project](https://www.themarshallproject.org/)
* Simone Weichselbaum, [The Marshall Project](https://www.themarshallproject.org/)
* Gabriel Dance, [The Marshall Project](https://www.themarshallproject.org/)

##Bugs
If you have questions about the data, please email Tom at ```tmeagher@themarshallproject.org``` or file a [Github issue](https://github.com/themarshallproject/doj14141/issues).
