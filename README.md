# custom-report-generator

This is a custom implementation of the WSO2 APIM Analytics Monthly Usage Report.

This implementation creates a table with the following information.

* API Name
* API Version
* UserName
* Hit Count

# Build

1) Run 'mvn clean install'
2) Copy the bundle 'org.wso2.analytics.apim.custompdf-3.1.0.jar' into {ANALYTICS_HOME}/lib
 directory
3) Set the report:implClass config in conf/dashboard/deployment.yaml to org.wso2.analytics.apim.custompdf.CustomPDFGenerator
4) Start the dashboard server, and try downloading the usage report via the admin dashboard. This should result in a PDF report with the above mentioned columns instead of the default ones. 
