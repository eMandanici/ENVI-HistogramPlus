# ENVI-HistogramPlus
Generating a histogram with a user defined bin size in ENVI

This extension for the ENVI software by Harris produces the histogram of a single band selected by the user. Differently from the basic statistic function implemented in ENVI, the user can manually set the minimum and maximum values and the bin size of the histogram. Furthermore, the Histogram Plus extension automatically neglects the "Data ignore value" eventually set in the header file, preserving the possibility of selecting an additional standard mask.

The resulting histogram is finally displayed in a statistics-like window, with a graphic section and a text one. Through the 'Options -> Preferences' menu, the user can set the numeric format of the text report. The plot can also be saved as an image file or added to a new ENVI Plot Window.
Furthermore this result window can be programmatically called by the IDL procedure "envi_report_histogram_plus, x, y", where "x" and "y" are one-dimensional arrays or scalar pointers.

The extension, compiled with IDL 8.0, applies both to ENVI Standard and ENVI Classic interfaces,

- to use it in the Classic interface, where it adds an item in the 'Basic Tools -> Statistics' menu, the "histogramplus.sav" file must be copied in the '...\Exelis\ENVI50\classic\save_add' directory;

- similarly, in ENVI 4.8, the file must be copied in the '...\ITT\IDL\IDL80\products\envi48\save_add' directory;

- to use it in the new ENVI 5 Standard interface, where it adds a tool in the 'Extensions' toolbox, the file must be copied in the '...\Exelis\ENVI50\extensions' directory.



*********************
   Update history
*********************

***** First version 2 July 2012
Core functionality.

***** Update 5 September 2012
Backward compatibility with ENVI 4.8 and minor bug fixing.

***** Update 24 October 2012
Unique sav file for both ENVI interfaces and new statistics-like result window.

***** Update 25 October 2012
Hotfix: wrong values of mean and std dev were printed in the report.

***** Update 21 April 2013
Fix problems with very large images.

***** Update 2 March 2018
Available on GitHub!
