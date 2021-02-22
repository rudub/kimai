# kimai

Kimai is a free, open source and online time-tracking software. The primary configiuration includes:
- php 
- mysql
- nginx/apache (webserver)

For configuration, I will be using AWS to deploy the setup using using below services:

mysql RDS : To host the database.
Created mysql (5.7) RDS (managed instance) on AWS.
Created database kimai_database and user `userkimai` on the database.

EKS: To deploy application on k8s using helm chart.

Docker-image: using kimai2 ready image with tag `latest-prod`

Created helm chart `kimai`
In deployment template -> provided database URL in environments. 
created the chart

`helm install kimai2`

