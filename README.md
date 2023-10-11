## Exercise 1 - Migrating and refactoring orders service of an e-commerce app
### Requirements:
- Have managed scaling as much as possible
- Decoupling solution components to maximize resilience
- Have centralized monitoring and logging
### Proposed Solution:
![image](https://github.com/mostafaibrahim24/architecting-solutions-aws-exercises/assets/78238174/be645d0a-f56a-46a0-abe2-34d49d77f5dc)

## Exercise 2 - Data analytics solution for a menu website
### Requirements:
- Provide HTTPS endpoint for data collection
- Prefer using AWS managed services as there is shortage in staff
- Prefer services with per-usage billing, not per-time billing
- Have cross-region data replication and encryption
- Use different storage classes to save on cost and encryption
### Proposed Solution:
![image](https://github.com/mostafaibrahim24/architecting-solutions-aws-exercises/assets/78238174/4dd1496c-cc0b-405d-84e3-05257f8b1e3b)
- Firehose for data ingestion
- S3, cross-region replication (CRR)
- S3 intelligent tiering enabled
- Athena to have interactive query service that you can use to analyze data in S3 by using SQL and you pay only for the queries that you run
- Choosing QuickSight over managed-grafana because of the shortage in staff and they already know how to use QuickSight and have a license
