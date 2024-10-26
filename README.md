[![Community Extension](https://img.shields.io/badge/Community%20Extension-An%20open%20source%20community%20maintained%20project-FF4700)](https://github.com/camunda-community-hub/community)
[![Lifecycle; Incubating](https://img.shields.io/badge/Lifecycle-Proof%20of%20Concept-blueviolet)](https://github.com/Camunda-Community-Hub/community/blob/main/extension-lifecycle.md#proof-of-concept-)[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
![Compatible with: Camunda Platform 8](https://img.shields.io/badge/Compatible%20with-Camunda%20Platform%208-0072Ce)

> [!WARNING]  
> Camunda extensions found in the Camunda Community Hub are maintained by the community and are not part of the commercial Camunda product. Camunda does not support community extensions as part of its commercial services to enterprise customers.

# Camunda 8 Init and Backup Scripts

By default, the Camunda 8 applications will attempt to create Elasticsearch objects (such as [index templates](https://www.elastic.co/guide/en/elasticsearch/reference/current/index-templates.html)) during first start. Camunda applications also make use of Elasticsearch Snapshot Repositories and snapshot API's to run the official [Camunda Backup steps](https://docs.camunda.io/docs/self-managed/operational-guides/backup-restore/backup-and-restore/).  

These operations require [Elasticsearch cluster level access](https://docs.camunda.io/docs/self-managed/concepts/elasticsearch-privileges/). 

However, in some cases, because of security policies, it is not possible to grant the Camunda applications the necessary [elastic search cluster level](https://docs.camunda.io/docs/self-managed/concepts/elasticsearch-privileges/) access to initialize Elasticsearch Objects or perform backups. 

As a possible workaround to this problem, this directory contains scripts that can be run independently from a Camunda 8 installation to initialize Elasticsearch Objects and create backups for Camunda 8 Zeebe, Operate, and Tasklist. 

Scripts for Optimize are currently not available.

