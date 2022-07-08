# AWSLakeFormationSystemAPI
System API to integrate with AWS LakeFormation and search LakeFormation database and/or tables by lf tags 

# Pre-requisites:
- Check out AWSGlueLakeFormationJavaClient from the following git location https://github.com/mulesoft-consulting/AWSGlueLakeFormationJavaClient.git
- Run mvn clean install to build and publish it into your local/remote artifact repo

# How to run:
- Ensure you have the right version of AWSGlueLakeFormationJavaClient mentioned in pom.xml
- Run this as any other mule api
- Invoke the endpoint /lakeFormation/searchDatabaseByLFTags with the following query parameters
  - awsAccessKey
  - awsSecretKey
  - lfTagKey
  - lfTagValues
- Invoke the endpoint /lakeFormation/searchTablesByLFTags with the following query parameters
  - awsAccessKey
  - awsSecretKey
  - lfTagKey
  - lfTagValues
