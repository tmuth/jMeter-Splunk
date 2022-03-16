# jMeter-Splunk
jMeter examples to load-test Splunk or send sample data to Splunk via HEC

- Download and install Apache jMeter https://jmeter.apache.org/
- Open the .jmx file with the jMeter GUI
- Edit User Defined Variables > SPLUNK_HOST & MGT_PORT
- Edit Thread Group > HTTP Authorization Manager > username and password
- (optional) Edit Thread Group > Random Controller > searches to include the searches you want to run

## Files / Test Plans
- jMeter-Splunk-vm-io-test.jmx - This test plan sends Splunk searches as REST calls to load-test a Splunk deployment
- HEC-Metrics.jmx - This test plan sends data to Splunk in the form of a metrics V3 (Splunk 8.0+) HEC payload. 
- Send-Metrics-DSP-HEC.jmx - Similar to the HEC-Metrics test plan with a slight modification to send to DSP via HEC
- access-combined-jMeter-Splunk.jmx - This sends buttercup games data in access_combined format via HEC
