## Magento extension for boosting search results using Elasticsearch

This is an updated module (based on [baranga's fork](https://github.com/baranga/magento-elasticsearch) of the [original code](https://github.com/jreinke/magento-elasticsearch)). There has been no extensive testing; basic search- and indexing functionality has been found to be working in combination with Elastichsearch v1.2.1.

[![Build Status](https://secure.travis-ci.org/gavro/magento-elasticsearch.png?branch=master)](http://travis-ci.org/gavro/magento-elasticsearch)

![Magento Elasticsearch](http://i.imgur.com/X6quR.png)

## Installation

### Magento CE 1.7+ only

Install with [modgit](https://github.com/jreinke/modgit):

    $ cd /path/to/magento
    $ modgit init
    $ modgit clone elasticsearch https://github.com/gavro/magento-elasticsearch.git

or download package manually:

* Download latest version [here](https://github.com/gavro/magento-elasticsearch/archive/master.zip)
* Unzip in Magento root folder
* Clean cache

## Usage

* Go to System > Configuration > Catalog > Catalog Search
* Select Elasticsearch search engine
* Configure server connection parameters
* Specify index name (default is magento)
* Optionally defines your custom search parameters
* Optionally boost some product attributes in Catalog > Attributes > Manage Attributes
* Reindex catalog search index
