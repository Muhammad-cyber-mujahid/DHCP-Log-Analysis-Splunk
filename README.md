# DHCP-Log-Analysis-Splunk

Overview

This project uses Splunk to analyze DHCP logs from the MACCDC2012 dataset to detect network-based threats. The dataset, dhcp.log.gz (1 MB), contains DHCP transactions with events, capturing IP assignments and device activity. It’s designed to help SOC analysts practice identifying suspicious network behaviors like unauthorized devices or reconnaissance.

Goals

-Detect network threats such as unauthorized devices, IP spoofing or reconnaissance using Splunk queries.
-Build skills in crafting queries to analyze DHCP log fields 
-Document findings with clear explanations, queries, and visualizations.
-Simulate a real-world network security scenario to enhance threat-hunting capabilities.


Steps

1. Download dhcp.log.gz from securitydatasets.com and extract to dhcp.log.
2. Upload dhcp.log to Splunk Cloud 
3. Verify data with index=user_activity_index source=dhcp.log | stats count (100–1000 events).
4. Run queries to detect threats 
5. Create dashboards to visualize patterns 
6. Document findings in docs/ with queries and screenshots.
7. Save results and images in screenshots/ and update GitHub repo.
8. Compile a report with insights and recommendations.


Requirements

Splunk Cloud (free trial) for log analysis.
7-Zip to extract dhcp.log.gz.
dhcp.log (1 MB) with extracted fields.
GitHub repo for storing docs and screenshots.
