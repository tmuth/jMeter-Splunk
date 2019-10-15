# jMeter-Splunk
jMeter examples to load-test Splunk

- Download and install Apache jMeter https://jmeter.apache.org/
- Open the .jmx file with the jMeter GUI
- Edit User Defined Variables > SPLUNK_HOST & MGT_PORT
- Edit Thread Group > HTTP Authorization Manager > username and password
- (optional) Edit Thread Group > Random Controller > searches to include the searches you want to run

