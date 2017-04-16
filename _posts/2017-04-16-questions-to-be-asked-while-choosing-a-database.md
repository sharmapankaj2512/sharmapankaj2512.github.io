---
published: false
---
## Questions to be asked while choosing a database

Databases now a days have become a problem of plenty. Relational, key-value, document, DHT etc just too many to choose from. With microservices now main stream it is even more important to choose the right database for the right job. 

I have always found this task of choosing the right database a bit dauting. One approach that I always employ is to narrow down on a set of database features that the microservice would need. Since we are talking about a microservice it should be relatively easier to come with such a list.

From time and again I have noticed that the feature set that I have narrowed down on is a subset of questions shared below. Note that this is not a comprehensive questionaire and I am keeping CAP theorem out of picture for now, rather it is meant to act more as checklist to set the tone of your discussion.

Structure - it is important to figure out upfront how the data would be stored/accessed
Scalability - is it really required?
Consitency - is it ok if stale data is served to end user?
Transactions - many databases out there that support distributed transactions
Indexing - not all databases support indexing
Joins - not all databases support joins
Query-ability - how easy it is to query?
Low-latency - 

Do remember choosing a database that offers strong gaurantees can potentially increase latency.