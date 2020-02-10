An example using splunk for data visulization in real time


Launch Splunk:
https://docs.splunk.com/Documentation/Splunk/8.0.1/SearchTutorial/StartSplunk

SPL Commands:
https://docs.splunk.com/Documentation/Splunk/8.0.1/SearchReference/WhatsInThisManual

Example DATA:
https://www.transtats.bts.gov/dataindex.asp?index=A&listorder=DATABASE
Table: Household characteristics

QUERY:
source="874851321_T_ATS_HH_CHARACTERISTICS.csv" host="DESKTOP-6IGRTFM" sourcetype="csv" | top HHID | bucket _time span=1h