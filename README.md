Dynamic-Map-Books
=================

###View The [Presentation Here](http://jonahadkins.github.io/Dynamic-Map-Books/#/)  

#####Notes & Slides For A  Esri Lightning Talk @ UC
=================
**Short Introduction**  
How we implemented 2 mapbook solutions with our client's Esri stack
  
**NSGEM Background**  
A spatially enabled enterprise system that provides access to monthly energy reporting for over 200 sites
and over 50,000 facilities worldwide. Built on top of GRX, an existing naval installation gis data viewer, NSGEM
was created to help personnel, namely decision makers and energy managers reduce overall consumption.

**Award Winner**  
Special Achievement In GIS, The _only_ federal program on the list!

**Map Book Checklist**   
* Why Mapbooks? We needed a way to visualize a lot of application info, charts, tables, and the map, in a printed format.
* Short Development Time - We had an upcoming promotion that needed to have this functionality, so needed a solution that could be implemented in less than a week.
* Content needed to be data driven - so we could start with data driven pages.  


**Fuzzy Math**  
Data driven pages within ArcMap would take care of the maps, and we saw an existing sample
add-in that explored data driven graphs. So we threw a few hundred lines of Python at it, 
and it became an semi-automated process. We still had to collate the pdf's and link them to application queries, but hey worked, and we met the deadline.

**Automation**  
We had to run this process monthly for awhile - and we knew we wanted to be fully
automated.

**Real Talk**  
We had some 'real talk' about a better solution. We were starting to implement CR for
custom and printed charts through the application, and thought if we could make a report look like a map book, it might work.

**Map Book Checklist 2**  
* ArcGIS Server - Application was in place already, so we would just need to configure the
reports to work with application queries.
* Crystal Reports - -we had access to an enterprise Navy license, and it was approved for use.- Using the Visual Studio CR Runtime
* Bytes - we found the we could create a temporary server side dataset the would store AGS map images has blobs and insert them in the final report.


**Final Map Book**  
The report renders in the application and is printable/savable an contains all the 
pertinent _time-stamped_ information for decision makers to understand energy
usage across the region.



