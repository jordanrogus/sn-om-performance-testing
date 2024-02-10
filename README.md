# sn-om-performance-testing

Features:
1. Create TMF622 Product Orders from a Product Offering generating test data from data in the instance
2. Activate jobs to generate N (default 1-10) orders every 5 minutes in non-production instances to create test data/performance checks. Secondary job is available to approve X% of orders, and the framework is setup to enable auto-fulfillment if subflows are generated and associated to OOTB OM decision tables
3. Enables custom payloads to be saved and used to generate N orders through the 'Custom Payloads' table with access to dynamically change query parameters
   
Dependencies:
Order Management for Telecom, Media & Tech v6.0.0

Instructions:
Update application properties, especially the "x_648117_order_man.basic_auth_config" property to a valid basic auth config sysId for the instance w/ access to run TMF APIs
