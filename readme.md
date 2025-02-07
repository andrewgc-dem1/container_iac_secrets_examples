Scan Image 2-7-25
- veracode scan --source  juliantotzek/verademo1-tomcat --type image --output scan-verademo.json --format json 
- veracode scan --source  juliantotzek/verademo1-tomcat --type image --output scan-verademo-table.txt --format table 

Scan IaC
- veracode scan --source https://github.com/bridgecrewio/terragoat --type repo --output iac.json --format json
- veracode scan --source https://github.com/bridgecrewio/terragoat --type repo --output iac-table.txt --format table
- veracode scan --source https://github.com/helm/charts --type repo --output iac.json --format json


Scan directory
- veracode scan --source insecure-test --type directory --output directory.json --format json
- veracode scan --source insecure-test --type directory --output directory-table.txt --format table

SBOM generation
- veracode sbom --source https://github.com/veracode/verademo --type repo --output verademo-sbom-cyclondx.json --format cyclonedx-json
- veracode sbom --source https://github.com/bridgecrewio/terragoat --type repo --output iac-sbom-cyclondx.json --format cyclonedx-json
- veracode sbom --source insecure-test --type directory --output directory-sbom-cyclondx.json --format cyclonedx-json

Bicep to arm
- az bicep build -f {file_name}.bicep
