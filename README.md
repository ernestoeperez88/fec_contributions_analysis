# Federal Election Commission Data Analysis

This data describes the finances of candidates running for election in 2016, and it details contributions from individual and organizations to campaigns disclosed to the FEC. The data files can be downloaded from [here](http://www.fec.gov/finance/disclosure/ftpdet.shtml#a2015_2016). We use the files found in the Data File and Format Description columns.

Here's a quick summary of the tables:

  * **cm** contains committee information
  * **cn** contains candidate information
  * **ccl** contains linkage between committees and candidates
  * **itcont** contains individual contributions to committees
  * **itpas2** contains contributions between committees
  * **itoth** links between committees

This ipython notebook makes use of Spark's DataFrame to perform some basic SQL queries on the FEC dataset  as well as taking advantage of its operators to implement K-means clustering. It finally uses the folium python package to visualize the cluster centrs found by the algorithm (unfortunatelly the maps are not rendered correctly by github. Sample output images were added to the repository).
