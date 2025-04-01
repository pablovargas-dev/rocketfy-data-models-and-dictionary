     

### <a id="documentation-body"></a>

![Hackolade image](Modulo-dropshipping/image1.png?raw=true)

MongoDB Physical Model
----------------------

#### Schema for:

Model name: Modulo Dropshipping y productos

Author: Rocketfy Development Team

Version: 1.0

### <a id="contents"></a>

*   [Table of Contents](#contents)
*   [1\. Model](#model)
*   [2\. Databases](#containers)
    *   [2.1 rocketfy](#6f94401a-8e31-4b31-9268-15061668a1b5)
        
        [2.1.2. Collections](#6f94401a-8e31-4b31-9268-15061668a1b5-children)
        
        [2.1.2.1 unified\_inventories](#7dbbb739-9112-4fed-8747-72e93d10c0d8)
        
        [2.1.2.2 unified\_variations](#d074212d-2fa6-426a-91f6-8ae358bcca95)
        
        [2.1.2.3 warehouse\_imports](#d9546eb8-72ab-4118-ac98-345b9b52d0e6)
        
        [2.1.2.4 wearehouse\_products](#0caea05c-4c87-43e4-9955-63f1a5327efe)
        
        [2.1.2.5 customers](#ec559fb7-4dbc-4d80-912e-a1628c5130b4)
        
        [2.1.2.6 unified\_products](#9e7d9462-9ccb-449b-a053-38685a5f26cd)
        
*   [3\. Relationships](#relationships)
    *   [3.7 products-variations](#0ad7ae99-e80c-4e35-a43c-7126b3c4ab03)
    *   [3.8 products-inventories](#fae6f210-947b-4b1e-8e59-f676ff6e0aa2)
    *   [3.9 customers-products](#42ea0620-581d-4451-9973-7e6dc61a8648)
    *   [3.10 warehouse\_imports-warehouse\_products](#ca9bfddb-da39-4704-82d6-5f7fc21a64d0)

### <a id="model"></a>

## 1\. Model

### 1.1 Model **Rocketfy**

#### 1.1.1 **Rocketfy** Entity Relationship Diagram

![Hackolade image](Modulo-dropshipping/image2.png?raw=true)

#### 1.1.2 **Rocketfy** Properties

##### 1.1.2.1 **Details** tab

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td><span>Model name</span></td><td>Rocketfy</td></tr><tr><td><span>Target</span></td><td>MongoDB</td></tr><tr><td><span>DB version</span></td><td>v8.0</td></tr><tr><td><span>Lineage capture</span></td><td></td></tr></tbody></table>

##### 1.1.2.2 **Options** tab

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

#### 1.1.3 **Rocketfy** DB Definitions

### <a id="containers"></a>

## 2\. Databases

### <a id="6f94401a-8e31-4b31-9268-15061668a1b5"></a>

### 2.1 Database **rocketfy\_dropshipping**

#### 2.1.1 **rocketfy\_dropshipping** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Database name</td><td>rocketfy</td></tr><tr><td>Activated</td><td>true</td></tr></tbody></table>

### <a id="6f94401a-8e31-4b31-9268-15061668a1b5-children"></a>

#### 2.1.2 **rocketfy\_dropshipping** Collections

### <a id="7dbbb739-9112-4fed-8747-72e93d10c0d8"></a>

##### 2.1.2.1 Collection **unified\_inventories**

###### 2.1.2.1.1 **unified\_inventories** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>unified_inventories</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#6f94401a-8e31-4b31-9268-15061668a1b5><span class="name-container">rocketfy</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.1.2 **unified\_inventories** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#49690ee3-a80c-40fd-a8df-9f81d77e3fb6 class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk, fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#785f4717-9805-4185-bfc7-75bf3ffe663c class="margin-0">quantity</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d5273cca-65db-48d5-b773-f2816bc1f382 class="margin-0">variation_id</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#061236f8-0897-433a-b435-74465ca06ae5 class="margin-0">unit_price</a></td><td class="no-break-word">numeric,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1282a4b9-fdeb-49c0-a56c-efadae5e5097 class="margin-0">total</a></td><td class="no-break-word">double</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fbd4523f-f9ba-4d37-a853-3ff71a309176 class="margin-0">reservation</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#99a6be47-395e-4ecb-9383-1eddca31d9c4 class="margin-0">created_time</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d65281cf-017e-45ee-ab5a-7cee34ece257 class="margin-0">toMigrate</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ba1124b8-1c93-4daa-af4e-0639cb082959 class="margin-0">establishment_identifier</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="49690ee3-a80c-40fd-a8df-9f81d77e3fb6"></a>

###### 2.1.2.1.2.1 Field **\_id**

###### 2.1.2.1.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr><tr><td>Foreign collection</td><td><a href=#9e7d9462-9ccb-449b-a053-38685a5f26cd>unified_products</a></td></tr><tr><td>Foreign field</td><td><a href=#f8acffc8-769b-4713-ae33-d525e050fb49>inventory_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr></tbody></table>

### <a id="785f4717-9805-4185-bfc7-75bf3ffe663c"></a>

###### 2.1.2.1.2.2 Field **quantity**

###### 2.1.2.1.2.2.1 **quantity** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>quantity</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="d5273cca-65db-48d5-b773-f2816bc1f382"></a>

###### 2.1.2.1.2.3 Field **variation\_id**

###### 2.1.2.1.2.3.1 **variation\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>variation_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="061236f8-0897-433a-b435-74465ca06ae5"></a>

###### 2.1.2.1.2.4 Field **unit\_price**

###### 2.1.2.1.2.4.1 **unit\_price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>unit_price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="1282a4b9-fdeb-49c0-a56c-efadae5e5097"></a>

###### 2.1.2.1.2.5 Field **total**

###### 2.1.2.1.2.5.1 **total** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>total</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>113.82999999999998</td></tr></tbody></table>

### <a id="fbd4523f-f9ba-4d37-a853-3ff71a309176"></a>

###### 2.1.2.1.2.6 Field **reservation**

###### 2.1.2.1.2.6.1 **reservation** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>reservation</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>324</td></tr></tbody></table>

### <a id="99a6be47-395e-4ecb-9383-1eddca31d9c4"></a>

###### 2.1.2.1.2.7 Field **created\_time**

###### 2.1.2.1.2.7.1 **created\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1742616772</td></tr></tbody></table>

### <a id="d65281cf-017e-45ee-ab5a-7cee34ece257"></a>

###### 2.1.2.1.2.8 Field **toMigrate**

###### 2.1.2.1.2.8.1 **toMigrate** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>toMigrate</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="ba1124b8-1c93-4daa-af4e-0639cb082959"></a>

###### 2.1.2.1.2.9 Field **establishment\_identifier**

###### 2.1.2.1.2.9.1 **establishment\_identifier** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>establishment_identifier</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>rocketfy_customer_supremeshopco_569741167</td></tr></tbody></table>

###### 2.1.2.1.3 **unified\_inventories** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">establishment_identifier_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">establishment_identifier_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">undefined('ascending')</td><td class="table-column-indexes">undefined('descending')</td></tr><tr><td>Background indexing</td><td class="table-column-indexes"></td><td class="table-column-indexes">true</td></tr></tbody></table>

### <a id="d074212d-2fa6-426a-91f6-8ae358bcca95"></a>

##### 2.1.2.2 Collection **unified\_variations**

###### 2.1.2.2.1 **unified\_variations** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>unified_variations</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#6f94401a-8e31-4b31-9268-15061668a1b5><span class="name-container">rocketfy</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.2.2 **unified\_variations** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#9950b4f8-54a7-48e0-9612-f77fc94596f8 class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk, fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#10897209-bd3e-4f55-8c72-e61d8878a941 class="margin-0">inventory_id</a></td><td class="no-break-word">string,objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8f2d217a-7cc9-4fd5-95cf-df17f80876ba class="margin-0">product_id</a></td><td class="no-break-word">string,objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#31c3370b-67c4-4229-9732-dc4b300cd0ff class="margin-0">created_time</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2847d766-f106-499b-84b0-a4078b81ccb9 class="margin-0">variation_id</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c5c0bcb9-2a2e-4bf6-9f09-a7dd2cebb3a7 class="margin-0">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#addc5549-3a11-4e7b-8722-44e6ffc34e36 class="margin-0">sku</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0a5241bb-8e52-4cf9-ad4b-2f0ae2590207 class="margin-0">price</a></td><td class="no-break-word">numeric,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4240676a-c9de-4960-9706-b12da2cc4159 class="margin-0">image</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#671f265a-056c-434a-a7b4-403aaf71ba89 class="margin-0">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#38e4b79f-bf78-43bd-929b-e21979355d55 class="margin-0">props</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#12f619be-3657-4276-b602-534ab172380c class="margin-5">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#47ed37af-9200-42d0-90d7-79b69919dead class="margin-10">id</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f8f5f61f-b123-4dfc-840b-f9c467c3ba87 class="margin-10">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f4219359-7b12-42f4-b40d-e95fb4b65321 class="margin-10">attr_id</a></td><td class="no-break-word">integer64</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6ed54544-6fe9-4903-9be9-928564133292 class="margin-10">attr_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1a0edfeb-04cb-4001-985e-e4014edd832c class="margin-0">quantity</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9cc7ab15-6bc0-43b1-938e-d507058552cb class="margin-0">toMigrate</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2e0dcf41-b20a-404a-91fc-9b0c6585cfda class="margin-0">establishment_identifier</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="9950b4f8-54a7-48e0-9612-f77fc94596f8"></a>

###### 2.1.2.2.2.1 Field **\_id**

###### 2.1.2.2.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr><tr><td>Foreign collection</td><td><a href=#9e7d9462-9ccb-449b-a053-38685a5f26cd>unified_products</a></td></tr><tr><td>Foreign field</td><td><a href=#3db8b469-67f6-4984-be67-c8e18f1e40fe>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr></tbody></table>

### <a id="10897209-bd3e-4f55-8c72-e61d8878a941"></a>

###### 2.1.2.2.2.2 Field **inventory\_id**

###### 2.1.2.2.2.2.1 **inventory\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>inventory_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,objectId)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8f2d217a-7cc9-4fd5-95cf-df17f80876ba"></a>

###### 2.1.2.2.2.3 Field **product\_id**

###### 2.1.2.2.2.3.1 **product\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>product_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,objectId)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="31c3370b-67c4-4229-9732-dc4b300cd0ff"></a>

###### 2.1.2.2.2.4 Field **created\_time**

###### 2.1.2.2.2.4.1 **created\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1742853234</td></tr></tbody></table>

### <a id="2847d766-f106-499b-84b0-a4078b81ccb9"></a>

###### 2.1.2.2.2.5 Field **variation\_id**

###### 2.1.2.2.2.5.1 **variation\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>variation_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c5c0bcb9-2a2e-4bf6-9f09-a7dd2cebb3a7"></a>

###### 2.1.2.2.2.6 Field **name**

###### 2.1.2.2.2.6.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Blanco-PRO</td></tr></tbody></table>

### <a id="addc5549-3a11-4e7b-8722-44e6ffc34e36"></a>

###### 2.1.2.2.2.7 Field **sku**

###### 2.1.2.2.2.7.1 **sku** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>sku</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>FU-BL-PR</td></tr></tbody></table>

### <a id="0a5241bb-8e52-4cf9-ad4b-2f0ae2590207"></a>

###### 2.1.2.2.2.8 Field **price**

###### 2.1.2.2.2.8.1 **price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4240676a-c9de-4960-9706-b12da2cc4159"></a>

###### 2.1.2.2.2.9 Field **image**

###### 2.1.2.2.2.9.1 **image** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>image</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="671f265a-056c-434a-a7b4-403aaf71ba89"></a>

###### 2.1.2.2.2.10 Field **active**

###### 2.1.2.2.2.10.1 **active** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>active</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="38e4b79f-bf78-43bd-929b-e21979355d55"></a>

###### 2.1.2.2.2.11 Field **props**

###### 2.1.2.2.2.11.1 **props** Hierarchy

Parent field: **unified\_variations**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#12f619be-3657-4276-b602-534ab172380c class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.2.2.11.2 **props** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>props</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="12f619be-3657-4276-b602-534ab172380c"></a>

###### 2.1.2.2.2.12 Field **\[0\]**

###### 2.1.2.2.2.12.1 **\[0\]** Hierarchy

Parent field: **props**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#47ed37af-9200-42d0-90d7-79b69919dead class="margin-NaN">id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f8f5f61f-b123-4dfc-840b-f9c467c3ba87 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f4219359-7b12-42f4-b40d-e95fb4b65321 class="margin-NaN">attr_id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6ed54544-6fe9-4903-9be9-928564133292 class="margin-NaN">attr_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.2.2.12.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="47ed37af-9200-42d0-90d7-79b69919dead"></a>

###### 2.1.2.2.2.13 Field **id**

###### 2.1.2.2.2.13.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>950519954</td></tr></tbody></table>

### <a id="f8f5f61f-b123-4dfc-840b-f9c467c3ba87"></a>

###### 2.1.2.2.2.14 Field **name**

###### 2.1.2.2.2.14.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>DIADEMA GAMER PROFESIONAL</td></tr></tbody></table>

### <a id="f4219359-7b12-42f4-b40d-e95fb4b65321"></a>

###### 2.1.2.2.2.15 Field **attr\_id**

###### 2.1.2.2.2.15.1 **attr\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>attr_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer64</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>725095205051581</td></tr></tbody></table>

### <a id="6ed54544-6fe9-4903-9be9-928564133292"></a>

###### 2.1.2.2.2.16 Field **attr\_name**

###### 2.1.2.2.2.16.1 **attr\_name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>attr_name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Producto</td></tr></tbody></table>

### <a id="1a0edfeb-04cb-4001-985e-e4014edd832c"></a>

###### 2.1.2.2.2.17 Field **quantity**

###### 2.1.2.2.2.17.1 **quantity** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>quantity</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="9cc7ab15-6bc0-43b1-938e-d507058552cb"></a>

###### 2.1.2.2.2.18 Field **toMigrate**

###### 2.1.2.2.2.18.1 **toMigrate** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>toMigrate</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="2e0dcf41-b20a-404a-91fc-9b0c6585cfda"></a>

###### 2.1.2.2.2.19 Field **establishment\_identifier**

###### 2.1.2.2.2.19.1 **establishment\_identifier** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>establishment_identifier</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>rocketfy_customer_tecnostorecol_994880791</td></tr></tbody></table>

###### 2.1.2.2.3 **unified\_variations** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">establishment_identifier_-1</td><td class="table-column-property">product_id_-1</td><td class="table-column-property">inventory_id_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">establishment_identifier_-1</td><td class="table-column-indexes">product_id_-1</td><td class="table-column-indexes">inventory_id_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">undefined('ascending')</td><td class="table-column-indexes">undefined('descending')</td><td class="table-column-indexes">undefined('descending')</td><td class="table-column-indexes">undefined('descending')</td></tr><tr><td>Background indexing</td><td class="table-column-indexes"></td><td class="table-column-indexes">true</td><td class="table-column-indexes"></td><td class="table-column-indexes"></td></tr></tbody></table>

### <a id="d9546eb8-72ab-4118-ac98-345b9b52d0e6"></a>

##### 2.1.2.3 Collection **warehouse\_imports**

###### 2.1.2.3.1 **warehouse\_imports** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>warehouse_imports</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#6f94401a-8e31-4b31-9268-15061668a1b5><span class="name-container">rocketfy</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.3.2 **warehouse\_imports** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#2ed96282-51a6-484b-bb4a-6597fb701687 class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#871dd2cf-bb8d-4297-9db9-fcde06bbb2b9 class="margin-0">product_id</a></td><td class="no-break-word">string</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#82c224b3-df98-47be-9251-ce5f67a5b608 class="margin-0">dbname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#177fca9c-07e0-4ab1-9d6c-d4bc40b8635c class="margin-0">created_time</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="2ed96282-51a6-484b-bb4a-6597fb701687"></a>

###### 2.1.2.3.2.1 Field **\_id**

###### 2.1.2.3.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="871dd2cf-bb8d-4297-9db9-fcde06bbb2b9"></a>

###### 2.1.2.3.2.2 Field **product\_id**

###### 2.1.2.3.2.2.1 **product\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>product_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#0caea05c-4c87-43e4-9955-63f1a5327efe>wearehouse_products</a></td></tr><tr><td>Foreign field</td><td><a href=#29f0288a-ccf4-405c-949e-93f27f97f667>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr><tr><td>Sample</td><td>636c774023908a828794a26e</td></tr></tbody></table>

### <a id="82c224b3-df98-47be-9251-ce5f67a5b608"></a>

###### 2.1.2.3.2.3 Field **dbname**

###### 2.1.2.3.2.3.1 **dbname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dbname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>rocketfy_customer_nikystore_1645109750</td></tr></tbody></table>

### <a id="177fca9c-07e0-4ab1-9d6c-d4bc40b8635c"></a>

###### 2.1.2.3.2.4 Field **created\_time**

###### 2.1.2.3.2.4.1 **created\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1742928198</td></tr></tbody></table>

###### 2.1.2.3.3 **warehouse\_imports** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">product_id_1</td><td class="table-column-property">_id_</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">product_id_1</td><td class="table-column-indexes">_id_</td></tr><tr><td>Key</td><td class="table-column-indexes">undefined('ascending')</td><td class="table-column-indexes">undefined('ascending')</td></tr></tbody></table>

### <a id="0caea05c-4c87-43e4-9955-63f1a5327efe"></a>

##### 2.1.2.4 Collection **wearehouse\_products**

###### 2.1.2.4.1 **wearehouse\_products** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>wearehouse_products</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#6f94401a-8e31-4b31-9268-15061668a1b5><span class="name-container">rocketfy</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.4.2 **wearehouse\_products** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#29f0288a-ccf4-405c-949e-93f27f97f667 class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk, dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#67a4d225-964b-478f-b0c3-f87f4ba7802a class="margin-0">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#94657179-09d5-40ea-8fc5-23cdccc74e0c class="margin-0">type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#72748c5b-2330-40ac-a06e-c66b010995f1 class="margin-0">short_description</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a2438519-ceeb-4a24-a9fb-8e4218fcfe7b class="margin-0">description</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1cfdd2e6-9e26-4965-988d-d38df4383f8d class="margin-0">price</a></td><td class="no-break-word">numeric,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0db9b7da-2ac1-4060-a1d4-752498650d2f class="margin-0">sku</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9b11b3a9-c1b8-470c-a3eb-18c3cb18862d class="margin-0">slug</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3e00412e-5060-4d3d-a553-00116f47b000 class="margin-0">visible</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7b68cc97-65b5-4df3-8ad5-53fae58f788b class="margin-0">imagePrin</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cc9d60a0-2530-4f32-9103-11b2ab2bcffc class="margin-5">fieldname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#99a54046-898c-4080-a338-ff84b5c44e4b class="margin-5">originalname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5e204df7-7f5d-4308-8e3a-ac406a7c46d0 class="margin-5">encoding</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0b981829-3656-476d-9708-d04d70406b41 class="margin-5">mimetype</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#462c3021-803c-482b-970b-614da1fd9c6a class="margin-5">size</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4215aecc-48cb-4467-b38d-d4d4cc65df71 class="margin-5">bucket</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#754bac07-eab3-4ceb-a2f0-600d82ed3d52 class="margin-5">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f575b7c1-6d7c-4071-a70b-59301a159f10 class="margin-5">acl</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5f790dee-6ace-4e2c-af74-a0c241d7e237 class="margin-5">contentType</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#063b3ff6-5744-42ed-989f-12494926d5ed class="margin-5">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e64e7b9c-d36e-460e-bbe9-0b202da51a70 class="margin-5">storageClass</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#67576eb4-deaa-4051-95ea-685fb77942a8 class="margin-5">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a8eb4e32-859a-4f01-b296-52635a118edc class="margin-5">metadata</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e2c06639-08f7-49b1-a8a7-1fb6d7b76cf6 class="margin-10">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#494c65e1-a84a-4eee-a80d-ce1a72cf23e8 class="margin-10">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ccdf1832-f2a1-4ad2-9100-80c850d905bf class="margin-5">location</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#07470b71-c816-45c3-91dc-d607d1635563 class="margin-5">etag</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#76383a70-dfc9-4750-b99b-dd9513346155 class="margin-5">versionId</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1b48c72f-b256-4069-aa4f-945ff9fa8c53 class="margin-5">principal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ed385778-1b6f-40a7-b323-f265e418a095 class="margin-5">status</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#24579ec3-9eca-45c0-a4ec-90924edfabbe class="margin-5">url</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8858420c-9c8f-497b-9ba6-ee27ed9fb414 class="margin-5">contentEncoding</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#790921d3-9577-42a5-901b-8aa7cf6a3497 class="margin-5">file</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d07ab573-e159-4e3e-b50d-5b2734b54b8a class="margin-5">id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#200e7540-681b-412a-97ba-82f1ee1a8997 class="margin-5">name</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#11f0de5c-c6f9-480a-a935-7ff35a9751a4 class="margin-0">images</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#707c7c9c-8b32-4ce1-942c-1e55803e6332 class="margin-5">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cc20d610-c556-4c76-919a-0451108ae8fb class="margin-10">fieldname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2e9b6781-b412-40d3-9f08-f408b4248faa class="margin-10">originalname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8434cd88-0982-4a39-b689-52fc4b274836 class="margin-10">encoding</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1f211791-7557-4dd0-a34c-a9975c858aac class="margin-10">mimetype</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d18cb7cc-4fec-4641-a31d-fc69eb9e6a25 class="margin-10">size</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#52a7a188-a5ae-4591-b4c7-46e6ccdb2608 class="margin-10">bucket</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0ed37de6-e8b4-4c53-9605-d93d236dc27c class="margin-10">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9870061b-c105-4088-9e7a-680b84335174 class="margin-10">acl</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#df32f84b-fe4c-46f2-8731-c1245d1e326a class="margin-10">contentType</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#587c23fe-9c38-4e47-9a7a-80db24077f58 class="margin-10">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f98e8d9b-bf72-4588-b53d-3e3548d8e134 class="margin-10">storageClass</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#13624b82-b62b-4835-9a80-87d134927dcf class="margin-10">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#59566a7c-7fa3-4861-8f05-1f494b0deb29 class="margin-10">metadata</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7cf6f3e0-56aa-4c9a-a32f-4ee6227b54eb class="margin-15">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#41969e74-b22e-4868-b4d3-ad73b3c98720 class="margin-15">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dfbbd87f-45ea-4c69-b2b5-d58fbbd1336b class="margin-10">location</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#07f2a018-0bca-40e7-a7c6-730e20673bf0 class="margin-10">etag</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#41e2a047-a61f-4f4f-bf50-7c14241057ab class="margin-10">versionId</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#13764987-4119-48fb-9f17-fa71da40b2d2 class="margin-10">principal</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1de69ef3-d82b-4292-ae71-457ef7c54466 class="margin-10">status</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#be4e276d-98a5-4e53-bf89-4a3cea3755fb class="margin-10">url</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#af20d252-1802-4f33-a565-b191be7881e7 class="margin-10">contentEncoding</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#807c26ff-66a0-4065-8696-5f5624cd1658 class="margin-10">file</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f8c0f7cb-5d1f-43b0-8a5c-bed929d0dfea class="margin-10">id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#aee00cf8-2942-4dab-ac1d-a23e5aa5946c class="margin-10">name</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#04997a75-413a-4870-874a-5c9bc2ef9d9e class="margin-0">created_time</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d0208153-6d6e-4a93-8f2a-71ed3fa4cc3c class="margin-0">attributes</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#41e21b94-e02c-4540-9fac-27d8b301d766 class="margin-5">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#caf6598c-20e7-4827-8bbb-7929bc604845 class="margin-10">checked</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#062631b4-79a8-4f8b-a9f0-d21d679a0fe5 class="margin-10">createItem</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#861316e0-747d-447b-a23f-7457ba847a7c class="margin-10">id</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b1445f02-295a-40f6-9e7c-035a6b43984e class="margin-10">items</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#401a37db-2264-4779-988d-60a6203656a9 class="margin-15">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1248952c-fe7d-47db-b67f-07bb2b2a6247 class="margin-20">checked</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1c1d82f1-3d6e-48f9-83d7-9d94f64ff7dc class="margin-20">id</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2d196b74-b3fd-4e24-a197-b785aa7a2297 class="margin-20">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ba43246a-ff27-4b23-8ca6-2e619d81cfdf class="margin-10">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4f0bdda3-c399-4191-9995-6c146c78b6a0 class="margin-10">subname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9481ea44-2de0-4b57-a02a-ca50638085c7 class="margin-0">variations</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#36c9c6e9-d487-48b1-8287-94a020b214d9 class="margin-5">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dff3c863-f576-4ce3-ae60-c8f6e0ad2b2d class="margin-10">inventory_id</a></td><td class="no-break-word">string,objectId</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#95d0d39a-cb61-4a18-bc8d-97e98790bd10 class="margin-10">product_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ca7f119c-4b0c-4381-ac05-b0726b9b92b8 class="margin-10">created_time</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ba4f3cf7-e229-4a4a-a96d-17123bc9c416 class="margin-10">variation_id</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#eafb0186-1051-4443-9079-1a3711c72be0 class="margin-10">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1579c837-5e1d-4d33-8c6b-5b553899c223 class="margin-10">sku</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f69e951a-4faf-4656-8d83-1cfc327a9c6a class="margin-10">price</a></td><td class="no-break-word">numeric,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fdba763d-5146-42db-9bb6-0b04584b1782 class="margin-10">image</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4082af47-080b-4261-808c-8e10aa08609e class="margin-10">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0c5d4012-dfd1-4740-9bb4-414c3ee635f8 class="margin-10">props</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#eb21ce0d-3a0e-45eb-8854-6ed189944d6e class="margin-15">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#48c56190-fccd-47f3-81b8-4f43ade6e719 class="margin-20">id</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8ee2a0e1-ebe5-401b-a848-22c75a666b67 class="margin-20">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3a34c835-bc81-4cee-9550-31be9e37b987 class="margin-20">attr_id</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c1c38d99-7fd0-4176-92e4-a8cbd8a0e035 class="margin-20">attr_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d9610ecb-d47d-47fc-8011-65fba7e8ac4a class="margin-10">_id</a></td><td class="no-break-word">string,objectId</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cff77544-07b7-44bd-b434-47d81e5a90f2 class="margin-10">quantity</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8c371cc6-6267-4505-89d6-63690d17b61c class="margin-10">establishment_identifier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b832ed7e-09e7-47f6-85c5-417406a7a6e3 class="margin-10">id</a></td><td class="no-break-word">string,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a01934f8-9e39-42b5-997e-2ea5be2f843e class="margin-10">isValidForm</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#03af50d2-2619-4ae8-bf6f-41f787343684 class="margin-10">shopify_variant_id</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4198a7e9-c4e9-4985-9832-60a836aacfbc class="margin-0">dimensions</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#153d0f68-9207-4ae1-a929-e0d03c810f4c class="margin-5">width</a></td><td class="no-break-word">double</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#56d25285-4d3c-42c6-a3a6-0bea03154be8 class="margin-5">height</a></td><td class="no-break-word">double</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8f28afc2-3d58-47bd-8321-8331873748c4 class="margin-5">large</a></td><td class="no-break-word">double</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#53754a7e-ace2-4181-b918-d12c1222b52f class="margin-5">volume</a></td><td class="no-break-word">double</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c28da140-ea24-47ae-8f3c-3d2a17164393 class="margin-5">weight</a></td><td class="no-break-word">numeric,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e557c278-1f38-4e1c-a3d3-2f4392825737 class="margin-5">weight_in_unit</a></td><td class="no-break-word">double</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ab34e0b5-2c2b-4fc2-89f5-f41b3c157901 class="margin-5">weight_unit</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#de15d260-fdc7-4111-8989-ed978ea0cc9f class="margin-0">metadata</a></td><td class="no-break-word">array,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cc0c4c86-32ed-4823-919e-833be8de1c7c class="margin-5">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#138039d9-dbbc-4ee0-a161-22f6dfea3a6e class="margin-0">category_id</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cd48ea2c-5930-4da3-a57d-312d75162972 class="margin-5">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a34020f6-631a-4a01-be65-3ad8db8a1047 class="margin-5">name</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#376da31f-c510-4555-aefa-3524e3121085 class="margin-0">warehouse</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#068b30f9-a7a0-4622-bd0a-7bfdcadb1376 class="margin-5">shipping</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7f50dbfb-516e-4e7f-bf70-4699e2775607 class="margin-5">suggested_price</a></td><td class="no-break-word">double</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0b875cb7-bcc3-4b53-8daa-b3ec4e4caabf class="margin-5">warehouse_price</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#392086f8-7177-4919-ab8c-26b30583a975 class="margin-5">discount</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5baa84a1-57e3-4706-ab79-209ea7a58515 class="margin-5">id_warehouse_rkf</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#37d310d2-d657-45b2-a704-7490e3793d96 class="margin-5">data</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#66a2eb12-dd46-4049-b392-143bf5aaccef class="margin-10">db_seller</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fb3e16ff-28e1-422e-bdeb-bd35c5eebeb6 class="margin-10">only_my_stores</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a17e1a7d-dfad-4c74-a334-ca7116e9a093 class="margin-10">shop</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cb32a604-386e-4509-8296-2bb752cee0cc class="margin-15">name</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2da13e9a-1830-4a4f-8702-9ad5919d4a17 class="margin-15">email</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cb8a21bb-8888-41bc-89d0-ff07c42fe810 class="margin-15">cc_nit</a></td><td class="no-break-word">string,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cd5813da-4e1f-44ef-bf46-d3f348ff049f class="margin-15">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ff324031-f559-4c96-9cbf-fbf9e98c6f6e class="margin-15">composed_address</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ce8a4cf2-0aa8-4bef-a87d-e39ae88fe316 class="margin-20">street</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f90a9167-7dbe-4bf7-829d-e4048a5b79df class="margin-20">street_number_one</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dd646760-4995-4dda-b2d5-eb38328d5735 class="margin-20">street_number_two</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#76603c15-d572-40d9-8bd9-bf30e462b54e class="margin-15">cod_postal</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#76a6f72b-779c-473d-8bca-48c364669204 class="margin-15">country</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a02eab7a-ddbd-450f-b686-f214fd0dcc92 class="margin-15">city</a></td><td class="no-break-word">document,string,null</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d3760f6a-f6f8-4391-8a86-4e33c633d5f0 class="margin-20">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e1fe952b-f176-4ec4-8a4a-aaa772a8aa8f class="margin-25">_id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0ac94e9a-54d5-4912-b7a8-622a659b7dae class="margin-25">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8a88ea5e-a285-496e-9b0c-dc83ef1da5d2 class="margin-25">before_courrier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8f4acb12-a9c4-40f0-a12a-259afce52a90 class="margin-25">checked</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ae19f329-a7aa-4b57-997f-6084396f10b1 class="margin-25">city_code</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1fdf17bb-66a2-4f3c-a632-c9dac041feb3 class="margin-25">cod_depto</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#43c2e8a6-6406-47f4-800e-3a595333fe2a class="margin-25">country</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d279953c-35ce-4b03-b483-115bdeefca53 class="margin-30">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7313d16a-58a4-414e-8636-e075d60ab46f class="margin-30">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7c96330d-4281-4a42-a123-5a92d7ae2e5a class="margin-30">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ee0f2f87-ecd3-4380-ac78-09166d6b2e5b class="margin-25">courrier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#56888e8e-e7f5-4bf5-b243-679de6e3d8c0 class="margin-25">dane_code</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cec2bb55-ad49-4b45-b694-fb18156597cd class="margin-30">rocketfy</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b67690e1-eddf-4874-8516-aa7f7cc96dba class="margin-30">servientrega</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c3d41599-d117-4246-a6a2-40f6397fd8b0 class="margin-25">disabled</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9339521a-69e5-49b2-b6e8-a7de8c0e3050 class="margin-25">forTest</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#931dd7fc-0beb-4a22-b8d5-7a02800bace1 class="margin-25">postal_code</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7aa9de0f-1cd8-43e9-bfeb-5f1186b742df class="margin-25">shipping_zone</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4c36e4ae-a695-4974-880f-75fed6a7f49a class="margin-25">shop_error</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d2ac6498-67a9-4761-8b09-2f16d3b2b79e class="margin-25">state</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8ff4fb9a-334b-4791-a9da-a5cbf04fefd6 class="margin-30">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5af11d58-85f5-4782-ae48-7ffc0df978bf class="margin-30">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c9d2e4c1-d59a-4172-86af-94442e72c94f class="margin-30">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#19082597-3d34-4501-bfa7-38b93dc31613 class="margin-15">departament</a></td><td class="no-break-word">document,string,null</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b4ea8a1e-56e6-4f26-a7f1-b94e1a1409ff class="margin-20">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a81be04d-79cd-45be-94ab-26682312f9f7 class="margin-25">_id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#96f5654b-df8c-4c2e-8136-8f4d48ffe239 class="margin-25">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#010738bc-12a4-4d98-9334-fa85929a095c class="margin-25">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#14154ed1-7a73-45f4-acd3-3f252bfe64a8 class="margin-25">country</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3203b6b3-c6c1-4348-99b1-3e4fc91a7a27 class="margin-30">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#465a2a36-ecc8-4123-bea1-316532de8b28 class="margin-30">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a8e6f79e-c3b7-4cd5-9ae8-3ccfa8d573ba class="margin-30">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#26bfb226-c315-494d-9e6c-2744511b5c33 class="margin-25">disabled</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f43d764e-b745-4c25-ae8a-546e59c823a6 class="margin-15">slogan</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2ca4af40-07e2-47df-80a5-f697e51647fa class="margin-15">color_primary</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d6b0d42d-4096-48c6-b6dc-71c27bc7c0e8 class="margin-15">colors</a></td><td class="no-break-word">array,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3753b497-6d51-42b2-be23-92d9d22c6e71 class="margin-20">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#09558d09-cae0-4953-a1a4-3a4494a3030c class="margin-25">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3b728b9f-2d7b-4c62-a09b-ed80c6a22f78 class="margin-15">large_description</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ec652a65-5d8e-49b6-824d-1bad308deea1 class="margin-15">logo</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1efa5b3f-9e74-4211-92b5-268908523510 class="margin-20">fieldname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e39551b2-2e13-46af-9dd4-164455f4a16a class="margin-20">originalname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c28cac81-ddd5-43a5-9400-13bdf8673a0c class="margin-20">encoding</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8f0319a4-63ef-48bc-83da-29c11382cbb0 class="margin-20">mimetype</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a6ecdd77-01e8-4631-ae51-5c5a001c0122 class="margin-20">size</a></td><td class="no-break-word">numeric,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8b918670-80f6-4dc2-966b-30214b0725a2 class="margin-20">bucket</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e3f9a06b-adfa-4d49-82f7-60af95727a80 class="margin-20">key</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#10573aff-eaf5-45b5-bed2-5168e1c391ea class="margin-20">acl</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6889b61a-4a50-4e12-aef2-deb044ddc957 class="margin-20">contentType</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d11c913b-fe77-4c4e-bd85-a3b87ac4c9b7 class="margin-20">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bfd04098-651e-4439-9656-ffd0ff8eaf5e class="margin-20">storageClass</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#35e94ad9-7198-4a93-a7c1-67dc091d18ba class="margin-20">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ada8171d-4f17-42f3-893e-099d2dc6b408 class="margin-20">metadata</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#56af53f0-0b62-4d9f-90c4-5c3f37c6def2 class="margin-25">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cb89aaad-290e-425a-94e1-50c582feba59 class="margin-25">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#96417e62-92c7-4def-bb55-e75fcb07350a class="margin-20">location</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5407cc7e-beb2-4bd7-a130-b767c121385c class="margin-20">etag</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6b25c1ab-d950-4432-87c1-19d58a3de6e8 class="margin-20">versionId</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cc9e36a0-ed42-4d00-bf92-2ec8a3557110 class="margin-20">contentEncoding</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#374732ff-688e-4207-b57e-9b2e600fa118 class="margin-20">created_time</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ed266c9c-644d-49bf-b478-ecd7fdbc5f47 class="margin-15">banner</a></td><td class="no-break-word">document,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b7e25618-182d-496a-98e9-624fc445511c class="margin-20">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6dc205dc-5b8d-4b7c-9b4c-2735d9d25f2d class="margin-25">location</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#00b68081-332e-46d7-afd7-94c697cac71a class="margin-25">acl</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#85e9382e-3ad1-4ef6-b6e9-5d2fdee3d0ed class="margin-25">bucket</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8668d108-b364-45e2-bff7-d087d82cde54 class="margin-25">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#df2dc48b-bd5d-4615-8ab5-185c88a71d53 class="margin-25">contentEncoding</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#84ecf8d8-fdd3-4470-9e94-7736e000bc64 class="margin-25">contentType</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#241cf5cf-babc-49b1-9de6-ea3d025ad5fd class="margin-25">created_time</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ded23226-fb69-4f10-92de-61452576680f class="margin-25">encoding</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#777f2407-15ca-4d16-a806-14225cd2bf70 class="margin-25">etag</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c773c1ce-3698-48a7-afad-1d8722172c34 class="margin-25">fieldname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ed44f796-4f43-4544-a2c1-d3768d4540c1 class="margin-25">key</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9f5207cf-3dd0-4fa5-961e-978196183a2f class="margin-25">metadata</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7fbf6001-1fba-49fe-8c81-d991560c2f17 class="margin-30">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f1fa0ba4-a6ff-43d9-82b3-18d5605f7a93 class="margin-30">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#58cc97db-e73e-4b8c-9f0f-e0af713e8ef7 class="margin-25">mimetype</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#508884ca-a078-4874-b7bf-9e23b5b80017 class="margin-25">originalname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#83dae5b0-7973-45d3-b1bb-4abbd61033ae class="margin-25">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2c82de82-049c-4581-aefe-032b73447f9f class="margin-25">size</a></td><td class="no-break-word">numeric,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f9f44719-3a7a-48c4-b27c-5597b7cfc7bb class="margin-25">storageClass</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2e0ffd1b-e856-4ddb-9878-ff7a9ebc2cf1 class="margin-25">versionId</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2b658d3a-25aa-4140-b87b-22d4281fecdc class="margin-15">promises</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0a9a7fc4-aa96-473b-8d7e-a691dcaaf15b class="margin-15">social</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#577e2bdb-f27d-416f-8570-ba1310b9cbd6 class="margin-20">instagram</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#de4851fb-b60c-4706-b415-4eba7479b14d class="margin-20">messenger</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#34dba23d-f359-495f-adba-db960eb44192 class="margin-20">whatsapp</a></td><td class="no-break-word">numeric,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5237c8b2-d0c4-4a6d-b18e-7605db373935 class="margin-20">facebook</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b5cced4b-b372-42dd-a837-c2c8ab5e52e6 class="margin-15">horary</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7a7c3d43-266e-4812-892e-a857b9fc0015 class="margin-20">init_horary</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#022d2e49-3566-42fc-afa8-ceaf35decda9 class="margin-25">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bd834a22-0ad9-44c4-ac3f-21c3f792f297 class="margin-25">value</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#32f350a1-9b9c-4a82-9d86-c7c829e80a36 class="margin-20">final_horary</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b6aad4c5-ad28-45c0-a2eb-8c60f54769c8 class="margin-25">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5682f348-d69e-469b-8529-056121f01dce class="margin-25">value</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d07012e7-6097-4a26-a193-80b7f3acc375 class="margin-15">neighborhood</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#eae2c42d-c1a3-4fec-a106-034bb25bc62c class="margin-15">location</a></td><td class="no-break-word">document,null,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ffa247e1-cac3-4c5e-8019-711a4b043e37 class="margin-20">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e024dbd4-8155-4672-bcfc-057ee45871a9 class="margin-25">lat</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#88e053fb-f2ed-4925-beb2-15f85e9fcd8a class="margin-25">lng</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e3d7dd9d-6ec9-436f-9232-524a60161021 class="margin-15">tel</a></td><td class="no-break-word">numeric,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#49bd41a3-a3e4-4b2f-a591-138e4ca74dc5 class="margin-15">payments</a></td><td class="no-break-word">document,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b481c030-9227-411a-bb72-f6be0d09c148 class="margin-20">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5711aed3-e84b-4990-adef-92fd3266736c class="margin-25">pse</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#48840bf1-f05d-4c43-99bc-bfbd8f4d9c8c class="margin-25">card</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#eb9c8e3b-739c-4b75-ba33-f732b8fba573 class="margin-25">cod</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#73ed4084-a56b-4c61-87fe-38d1cbc9264b class="margin-25">bancolombia_collect</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a5badfdc-6b0f-420f-8c20-b73ec791f60a class="margin-25">bancolombia_qr</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f95d4e6a-49a2-4256-8a8e-326f1dbed987 class="margin-25">bancolombia_transfer</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4ba0dd38-0b32-439e-9de0-1e13dca98420 class="margin-25">nequi</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2ca7fb7d-789c-484c-85b9-9c4cff5f2055 class="margin-15">principal_address</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fff19708-f19e-4268-984e-f4efb922d5d8 class="margin-15">carry</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#664f931c-2fe7-46ae-bc20-20d21a9adf96 class="margin-15">geolocation</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4047ec66-06b0-4877-8fb7-f7ef689defc5 class="margin-20">lat</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7dad6b71-d872-4284-92a6-3bf4ebfab00c class="margin-20">lng</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ab2ae1fa-334f-4bb3-8f60-353b9ffbf0e2 class="margin-15">default</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#368ed2fd-0df8-4ce0-a1f5-bdf14f20dfb4 class="margin-15">gtag</a></td><td class="no-break-word">null,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#25529cf4-1e9d-49de-a16d-a128d56beaa5 class="margin-15">indicative</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8408f5f2-e892-488d-ab06-41e8194cc0e8 class="margin-15">pixel</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#47fa6237-2ab0-42c4-9a0c-690c12297ffc class="margin-10">rem</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ae995f7f-4690-4f1d-8c50-e65096e817ad class="margin-15">name</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#083681c9-f705-4754-9747-7f33575d2ef1 class="margin-15">last_name</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#181ce998-4e59-4054-b150-926265aeb8b6 class="margin-15">tel</a></td><td class="no-break-word">numeric,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#de4db032-096a-430d-9348-3949db3d0221 class="margin-5">statistics</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d07aa858-0ecb-452c-8329-3880e1d46f4e class="margin-10">sales</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#91bacde1-b8ba-4277-ac34-1292d224161e class="margin-10">imports</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#76982eaa-d18c-47dd-a243-c6efe67eb068 class="margin-5">father_id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d534c787-307d-4f46-b09e-2b7eaca551fa class="margin-5">shared_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#74fb6938-13c1-439a-8fd7-f3aa8c11f5ae class="margin-5">suggestions</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4afa0df0-896e-43ba-9945-7b33f77b2897 class="margin-0">warranty</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4b7773b2-3d77-4f03-bcdb-dedd3e7902ad class="margin-0">disabled_by_inactivity</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e02a5f63-6aac-4957-8613-6355ec2d4c89 class="margin-0">total_inventory</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c94bce45-3ff3-434f-ba8f-799d686d78a3 class="margin-0">category</a></td><td class="no-break-word">document,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e15e6ba6-5b5d-4186-8dda-e53a6febad96 class="margin-5">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5f3e625f-01f8-4918-ab39-b126e9258012 class="margin-10">_id</a></td><td class="no-break-word">string,objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#961ae830-0464-4e0c-ba9f-98964443e060 class="margin-10">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2a854d38-8abd-4958-a841-9af679b109a8 class="margin-10">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6a4c54d9-4f5c-41f4-9fc8-dab09627c672 class="margin-10">category_father</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#af3a0336-4795-4a67-b57b-28b1cd1eda9a class="margin-10">path_from_root</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#042e4681-94ad-41fc-afdc-bf1dc3de3026 class="margin-15">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#97de3524-a747-41c7-a339-2b888f041992 class="margin-20">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7bd25ae4-4f6c-4b55-ad9c-49c20d9a8053 class="margin-20">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#859c5cf2-8007-49c2-8fba-0a7a68c964f4 class="margin-10">children_categories</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#01254cd8-6f93-40fc-874f-953ff1c728ef class="margin-15">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a6a3ea19-c744-4704-90df-ff1365581ce7 class="margin-20">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#946fc241-01d7-4260-a7da-7276d452cc00 class="margin-20">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cc583a06-9b0a-4b28-ad26-737fc6a514f0 class="margin-10">settings</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1246458f-ff5c-47e0-bba6-ed52fcc463f9 class="margin-15">adult_content</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#23ec97a5-48fc-44c6-b19f-ffe64a6326e7 class="margin-15">fragile</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3e8418be-3707-411e-9b25-f47393f0d335 class="margin-15">currencies</a></td><td class="no-break-word">array</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f021a06e-2337-427d-aaad-7bb8599ba289 class="margin-20">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6ca30205-cbfa-4613-a6be-5eca2642cea9 class="margin-15">inmediate_payment</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5f2752a1-59c9-4279-8c05-c4cd1b7aa94f class="margin-15">items_review_allowed</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0f09a277-14ff-4422-a166-55a6fb1baf71 class="margin-15">listing_allowed</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bc4efc4c-a1c6-4942-8d13-af34f15bd54d class="margin-15">max_description_length</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#afbfba1c-136d-44bb-8519-8270210b735d class="margin-15">max_pictures_per_item</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c6f3ce21-e7d4-4229-8909-1cdb16558aff class="margin-15">max_pictures_per_item_var</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bd485a11-0755-441e-abf0-fde36133ec9b class="margin-15">max_sub_title_length</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#441aa472-3bfb-4477-a93c-d90de521be28 class="margin-15">max_title_length</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#db60fcac-26b4-4d59-abc4-6d8bca0f44bc class="margin-15">maximum_price</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2398b183-3bd2-45ab-b885-cc56b81d6733 class="margin-15">maximum_price_currency</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9940d20e-0f2e-4359-b26a-a1f3331e4fae class="margin-15">minimum_price</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#38614ed2-53fa-47d3-8c06-590511225f58 class="margin-15">minimum_price_currency</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5f7bec98-fc01-4c43-aacc-bec5b0ba4442 class="margin-15">sat_product_code_mexico</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d86a93b3-d0fc-4104-b5e4-016ae7cf6b59 class="margin-15">sat_product_description_mexico</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8495f827-3b2e-4731-a90e-13053806a487 class="margin-15">seller_contact</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8e70ca9d-2674-446a-b25f-28d427a175bc class="margin-15">status</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8128146f-807d-4490-b512-cec7382bc11b class="margin-10">country</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2ec8180a-efbd-443c-b516-d8a44b989cdf class="margin-10">date_created</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c19aea5e-3922-48dd-8361-3d52d94cac3b class="margin-10">permalink</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#403fdafd-7aae-4d35-8acb-739e4575237a class="margin-10">picture</a></td><td class="no-break-word">null,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5c14173d-c5d1-4037-bb6e-a8bdbd8c219f class="margin-0">country_ref</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#17eb216d-e21e-44ba-add8-d0ceaadd1ccf class="margin-5">_id</a></td><td class="no-break-word">objectId,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3619e6ac-a785-41a5-93ec-569240826f3c class="margin-5">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f21e27d1-e3f2-4ae4-bb41-6f75239ad5b3 class="margin-5">iso2</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d59b9c4b-bf17-4213-990e-f0bf5e7bf96a class="margin-5">iso3</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e8bd220f-59d2-4251-9bd7-7678993f6b82 class="margin-5">flag_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#07975898-638d-498a-80cd-84888d87fb12 class="margin-5">phone_code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#757464b8-643f-43f3-b296-63fb542b4e40 class="margin-0">featured</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f65461d3-42b2-4caa-94e2-3e8bbbda9288 class="margin-0">shared_metadata</a></td><td class="no-break-word">document,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0693bc10-2926-48ca-add4-96c5554bf350 class="margin-5">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d831edad-5fb6-488a-bbcc-50be26f95f40 class="margin-10">shared_with</a></td><td class="no-break-word">null,array</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#47fb169c-5f21-44b3-9be6-941ebd0e98a4 class="margin-15">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#38f5c5b9-42e8-436f-b8ca-63dfc2fed6ce class="margin-20">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9da97876-700e-4f5b-9772-697b127e4c11 class="margin-25">label</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#978d06c2-5ede-47eb-aac6-f3d0b272b2e9 class="margin-25">value</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d336bb50-52a3-4e65-b92b-c711e644377d class="margin-0">shop_out</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#33fecb1d-d431-48a5-bddc-fc5bc09d308e class="margin-0">vivible</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5c9f0e25-a29b-4627-8b6c-237402add3d1 class="margin-0">vusible</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#81d51b83-9544-48df-8d41-880fa1f22224 class="margin-0">warranty_description</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="29f0288a-ccf4-405c-949e-93f27f97f667"></a>

###### 2.1.2.4.2.1 Field **\_id**

###### 2.1.2.4.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="67a4d225-964b-478f-b0c3-f87f4ba7802a"></a>

###### 2.1.2.4.2.2 Field **name**

###### 2.1.2.4.2.2.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Joyero UBI-23001-1</td></tr></tbody></table>

### <a id="94657179-09d5-40ea-8fc5-23cdccc74e0c"></a>

###### 2.1.2.4.2.3 Field **type**

###### 2.1.2.4.2.3.1 **type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>variable</td></tr></tbody></table>

### <a id="72748c5b-2330-40ac-a06e-c66b010995f1"></a>

###### 2.1.2.4.2.4 Field **short\_description**

###### 2.1.2.4.2.4.1 **short\_description** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>short_description</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Joyeria fina, duradera e hipoalergénica, chapado con un porcentaje en oro.</td></tr></tbody></table>

### <a id="a2438519-ceeb-4a24-a9fb-8e4218fcfe7b"></a>

###### 2.1.2.4.2.5 Field **description**

###### 2.1.2.4.2.5.1 **description** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>description</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>&lt;p&gt;Descubra nuestra exclusiva l&amp;iacute;nea de joyer&amp;iacute;a de fantas&amp;iacute;a fina, cuidadosamente elaborada con materiales de primera calidad. Cada pieza es una obra maestra, con una base de cobre chapado en una exquisita mezcla de oro y rodio que le confiere un color deslumbrante y un brillo incomparable. La elecci&amp;oacute;n de estos materiales no solo garantiza una est&amp;eacute;tica impresionante, sino que tambi&amp;eacute;n hace que nuestras joyas sean hipoalerg&amp;eacute;nicas, brind&amp;aacute;ndote la m&amp;aacute;xima comodidad y estilo.&lt;/p&gt; &lt;p&gt;&amp;nbsp;&lt;/p&gt; &lt;p&gt;Los detalles maravillosos de nuestras piezas no se detuvieron aqu&amp;iacute;. Incorporamos circonio y microcirc&amp;oacute;n como materiales secundarios, asegurando un acabado impecable y un toque de elegancia adicional. La calidad es nuestra prioridad, y queremos que cada pieza no solo resalte tu belleza, sino que tambi&amp;eacute;n perdure a lo largo del tiempo.&lt;/p&gt; &lt;p&gt;&amp;nbsp;&lt;/p&gt; &lt;p&gt;Para garantizar la durabilidad de sus accesorios, es esencial brindarles el cuidado adecuado. Aqu&amp;iacute; tienes algunas pr&amp;aacute;cticas recomendadas:&lt;/p&gt; &lt;p&gt;&amp;nbsp;&lt;/p&gt; &lt;p&gt;1. &lt;strong&gt;Evite el contacto con productos qu&amp;iacute;micos: &lt;/strong&gt;Mant&amp;eacute;n tus joyas alejadas de jabones, lociones y otros productos qu&amp;iacute;micos que puedan afectar su brillo y calidad original.&lt;/p&gt; &lt;p&gt;&amp;nbsp;&lt;/p&gt; &lt;p&gt;2. &lt;strong&gt;Almac&amp;eacute;nalos por separado&lt;/strong&gt;: Guarde cada pieza de forma individual para evitar rayones y asegurar que mantengan su esplendor &amp;uacute;nico.&lt;/p&gt; &lt;p&gt;&amp;nbsp;&lt;/p&gt; &lt;p&gt;3. &lt;strong&gt;Evita ambientes adversos&lt;/strong&gt;: Por su durabilidad, nuestras joyas son resistentes, pero es aconsejable no exponerlas innecesariamente a lugares como la piscina, gimnasio, mar o ducha, donde podr&amp;iacute;an enfrentar condiciones que podr&amp;iacute;an afectar su estado a largo plazo.&lt;/p&gt; &lt;p&gt;&amp;nbsp;&lt;/p&gt; &lt;p&gt;Cada joya es una declaraci&amp;oacute;n de estilo y elegancia, y con el cuidado adecuado, podr&amp;aacute;s disfrutar de su belleza durante mucho tiempo. &amp;iexcl;Luce tu brillo &amp;uacute;nico con nuestra colecci&amp;oacute;n de fantas&amp;iacute;a fina!&lt;/p&gt;</td></tr></tbody></table>

### <a id="1cfdd2e6-9e26-4965-988d-d38df4383f8d"></a>

###### 2.1.2.4.2.6 Field **price**

###### 2.1.2.4.2.6.1 **price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="0db9b7da-2ac1-4060-a1d4-752498650d2f"></a>

###### 2.1.2.4.2.7 Field **sku**

###### 2.1.2.4.2.7.1 **sku** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>sku</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="9b11b3a9-c1b8-470c-a3eb-18c3cb18862d"></a>

###### 2.1.2.4.2.8 Field **slug**

###### 2.1.2.4.2.8.1 **slug** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>slug</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>joyero-ubi-23001-1</td></tr></tbody></table>

### <a id="3e00412e-5060-4d3d-a553-00116f47b000"></a>

###### 2.1.2.4.2.9 Field **visible**

###### 2.1.2.4.2.9.1 **visible** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>visible</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="7b68cc97-65b5-4df3-8ad5-53fae58f788b"></a>

###### 2.1.2.4.2.10 Field **imagePrin**

###### 2.1.2.4.2.10.1 **imagePrin** Hierarchy

Parent field: **wearehouse\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#cc9d60a0-2530-4f32-9103-11b2ab2bcffc class="margin-NaN">fieldname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#99a54046-898c-4080-a338-ff84b5c44e4b class="margin-NaN">originalname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5e204df7-7f5d-4308-8e3a-ac406a7c46d0 class="margin-NaN">encoding</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0b981829-3656-476d-9708-d04d70406b41 class="margin-NaN">mimetype</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#462c3021-803c-482b-970b-614da1fd9c6a class="margin-NaN">size</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4215aecc-48cb-4467-b38d-d4d4cc65df71 class="margin-NaN">bucket</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#754bac07-eab3-4ceb-a2f0-600d82ed3d52 class="margin-NaN">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f575b7c1-6d7c-4071-a70b-59301a159f10 class="margin-NaN">acl</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5f790dee-6ace-4e2c-af74-a0c241d7e237 class="margin-NaN">contentType</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#063b3ff6-5744-42ed-989f-12494926d5ed class="margin-NaN">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e64e7b9c-d36e-460e-bbe9-0b202da51a70 class="margin-NaN">storageClass</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#67576eb4-deaa-4051-95ea-685fb77942a8 class="margin-NaN">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a8eb4e32-859a-4f01-b296-52635a118edc class="margin-NaN">metadata</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ccdf1832-f2a1-4ad2-9100-80c850d905bf class="margin-NaN">location</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#07470b71-c816-45c3-91dc-d607d1635563 class="margin-NaN">etag</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#76383a70-dfc9-4750-b99b-dd9513346155 class="margin-NaN">versionId</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1b48c72f-b256-4069-aa4f-945ff9fa8c53 class="margin-NaN">principal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ed385778-1b6f-40a7-b323-f265e418a095 class="margin-NaN">status</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#24579ec3-9eca-45c0-a4ec-90924edfabbe class="margin-NaN">url</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8858420c-9c8f-497b-9ba6-ee27ed9fb414 class="margin-NaN">contentEncoding</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#790921d3-9577-42a5-901b-8aa7cf6a3497 class="margin-NaN">file</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d07ab573-e159-4e3e-b50d-5b2734b54b8a class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#200e7540-681b-412a-97ba-82f1ee1a8997 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.10.2 **imagePrin** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>imagePrin</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="cc9d60a0-2530-4f32-9103-11b2ab2bcffc"></a>

###### 2.1.2.4.2.11 Field **fieldname**

###### 2.1.2.4.2.11.1 **fieldname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="99a54046-898c-4080-a338-ff84b5c44e4b"></a>

###### 2.1.2.4.2.12 Field **originalname**

###### 2.1.2.4.2.12.1 **originalname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>originalname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1702239315sin-titulo-1702235413-pieza-a-pieza-1098051424.jpg</td></tr></tbody></table>

### <a id="5e204df7-7f5d-4308-8e3a-ac406a7c46d0"></a>

###### 2.1.2.4.2.13 Field **encoding**

###### 2.1.2.4.2.13.1 **encoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>encoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>7bit</td></tr></tbody></table>

### <a id="0b981829-3656-476d-9708-d04d70406b41"></a>

###### 2.1.2.4.2.14 Field **mimetype**

###### 2.1.2.4.2.14.1 **mimetype** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mimetype</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="462c3021-803c-482b-970b-614da1fd9c6a"></a>

###### 2.1.2.4.2.15 Field **size**

###### 2.1.2.4.2.15.1 **size** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>size</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>2835476</td></tr></tbody></table>

### <a id="4215aecc-48cb-4467-b38d-d4d4cc65df71"></a>

###### 2.1.2.4.2.16 Field **bucket**

###### 2.1.2.4.2.16.1 **bucket** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>bucket</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>shopping-rocketfy-uploads</td></tr></tbody></table>

### <a id="754bac07-eab3-4ceb-a2f0-600d82ed3d52"></a>

###### 2.1.2.4.2.17 Field **key**

###### 2.1.2.4.2.17.1 **key** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>key</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1702239315sin-titulo-1702235413-pieza-a-pieza-1098051424.jpg</td></tr></tbody></table>

### <a id="f575b7c1-6d7c-4071-a70b-59301a159f10"></a>

###### 2.1.2.4.2.18 Field **acl**

###### 2.1.2.4.2.18.1 **acl** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>acl</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>public-read</td></tr></tbody></table>

### <a id="5f790dee-6ace-4e2c-af74-a0c241d7e237"></a>

###### 2.1.2.4.2.19 Field **contentType**

###### 2.1.2.4.2.19.1 **contentType** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentType</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="063b3ff6-5744-42ed-989f-12494926d5ed"></a>

###### 2.1.2.4.2.20 Field **contentDisposition**

###### 2.1.2.4.2.20.1 **contentDisposition** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentDisposition</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="e64e7b9c-d36e-460e-bbe9-0b202da51a70"></a>

###### 2.1.2.4.2.21 Field **storageClass**

###### 2.1.2.4.2.21.1 **storageClass** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>storageClass</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>STANDARD</td></tr></tbody></table>

### <a id="67576eb4-deaa-4051-95ea-685fb77942a8"></a>

###### 2.1.2.4.2.22 Field **serverSideEncryption**

###### 2.1.2.4.2.22.1 **serverSideEncryption** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>serverSideEncryption</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a8eb4e32-859a-4f01-b296-52635a118edc"></a>

###### 2.1.2.4.2.23 Field **metadata**

###### 2.1.2.4.2.23.1 **metadata** Hierarchy

Parent field: **imagePrin**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#e2c06639-08f7-49b1-a8a7-1fb6d7b76cf6 class="margin-NaN">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#494c65e1-a84a-4eee-a80d-ce1a72cf23e8 class="margin-NaN">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.23.2 **metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="e2c06639-08f7-49b1-a8a7-1fb6d7b76cf6"></a>

###### 2.1.2.4.2.24 Field **fieldName**

###### 2.1.2.4.2.24.1 **fieldName** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldName</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="494c65e1-a84a-4eee-a80d-ce1a72cf23e8"></a>

###### 2.1.2.4.2.25 Field **Content-Type**

###### 2.1.2.4.2.25.1 **Content-Type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Content-Type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="ccdf1832-f2a1-4ad2-9100-80c850d905bf"></a>

###### 2.1.2.4.2.26 Field **location**

###### 2.1.2.4.2.26.1 **location** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>location</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://s3-uploads.rocketfy.co/1702239315sin-titulo-1702235413-pieza-a-pieza-1098051424.jpg</td></tr></tbody></table>

### <a id="07470b71-c816-45c3-91dc-d607d1635563"></a>

###### 2.1.2.4.2.27 Field **etag**

###### 2.1.2.4.2.27.1 **etag** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>etag</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>"4da7d4169d706df1fddb965318eaf66c"</td></tr></tbody></table>

### <a id="76383a70-dfc9-4750-b99b-dd9513346155"></a>

###### 2.1.2.4.2.28 Field **versionId**

###### 2.1.2.4.2.28.1 **versionId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>versionId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>b0F3LziDCQ1Jqoj12Pxqrleswz0uBEwr</td></tr></tbody></table>

### <a id="1b48c72f-b256-4069-aa4f-945ff9fa8c53"></a>

###### 2.1.2.4.2.29 Field **principal**

###### 2.1.2.4.2.29.1 **principal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>principal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="ed385778-1b6f-40a7-b323-f265e418a095"></a>

###### 2.1.2.4.2.30 Field **status**

###### 2.1.2.4.2.30.1 **status** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>status</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>old</td></tr></tbody></table>

### <a id="24579ec3-9eca-45c0-a4ec-90924edfabbe"></a>

###### 2.1.2.4.2.31 Field **url**

###### 2.1.2.4.2.31.1 **url** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>url</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://s3-uploads.rocketfy.co/1702239315sin-titulo-1702235413-pieza-a-pieza-1098051424.jpg</td></tr></tbody></table>

### <a id="8858420c-9c8f-497b-9ba6-ee27ed9fb414"></a>

###### 2.1.2.4.2.32 Field **contentEncoding**

###### 2.1.2.4.2.32.1 **contentEncoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentEncoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="790921d3-9577-42a5-901b-8aa7cf6a3497"></a>

###### 2.1.2.4.2.33 Field **file**

###### 2.1.2.4.2.33.1 **file** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>file</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="d07ab573-e159-4e3e-b50d-5b2734b54b8a"></a>

###### 2.1.2.4.2.34 Field **id**

###### 2.1.2.4.2.34.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>66b3d51028485d2d64477257</td></tr></tbody></table>

### <a id="200e7540-681b-412a-97ba-82f1ee1a8997"></a>

###### 2.1.2.4.2.35 Field **name**

###### 2.1.2.4.2.35.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>t-24-v-maki-espaciosyhogar-54142172.png</td></tr></tbody></table>

### <a id="11f0de5c-c6f9-480a-a935-7ff35a9751a4"></a>

###### 2.1.2.4.2.36 Field **images**

###### 2.1.2.4.2.36.1 **images** Hierarchy

Parent field: **wearehouse\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#707c7c9c-8b32-4ce1-942c-1e55803e6332 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.36.2 **images** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>images</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="707c7c9c-8b32-4ce1-942c-1e55803e6332"></a>

###### 2.1.2.4.2.37 Field **\[0\]**

###### 2.1.2.4.2.37.1 **\[0\]** Hierarchy

Parent field: **images**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#cc20d610-c556-4c76-919a-0451108ae8fb class="margin-NaN">fieldname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2e9b6781-b412-40d3-9f08-f408b4248faa class="margin-NaN">originalname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8434cd88-0982-4a39-b689-52fc4b274836 class="margin-NaN">encoding</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1f211791-7557-4dd0-a34c-a9975c858aac class="margin-NaN">mimetype</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d18cb7cc-4fec-4641-a31d-fc69eb9e6a25 class="margin-NaN">size</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#52a7a188-a5ae-4591-b4c7-46e6ccdb2608 class="margin-NaN">bucket</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0ed37de6-e8b4-4c53-9605-d93d236dc27c class="margin-NaN">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9870061b-c105-4088-9e7a-680b84335174 class="margin-NaN">acl</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#df32f84b-fe4c-46f2-8731-c1245d1e326a class="margin-NaN">contentType</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#587c23fe-9c38-4e47-9a7a-80db24077f58 class="margin-NaN">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f98e8d9b-bf72-4588-b53d-3e3548d8e134 class="margin-NaN">storageClass</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#13624b82-b62b-4835-9a80-87d134927dcf class="margin-NaN">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#59566a7c-7fa3-4861-8f05-1f494b0deb29 class="margin-NaN">metadata</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dfbbd87f-45ea-4c69-b2b5-d58fbbd1336b class="margin-NaN">location</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#07f2a018-0bca-40e7-a7c6-730e20673bf0 class="margin-NaN">etag</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#41e2a047-a61f-4f4f-bf50-7c14241057ab class="margin-NaN">versionId</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#13764987-4119-48fb-9f17-fa71da40b2d2 class="margin-NaN">principal</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1de69ef3-d82b-4292-ae71-457ef7c54466 class="margin-NaN">status</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#be4e276d-98a5-4e53-bf89-4a3cea3755fb class="margin-NaN">url</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#af20d252-1802-4f33-a565-b191be7881e7 class="margin-NaN">contentEncoding</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#807c26ff-66a0-4065-8696-5f5624cd1658 class="margin-NaN">file</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f8c0f7cb-5d1f-43b0-8a5c-bed929d0dfea class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#aee00cf8-2942-4dab-ac1d-a23e5aa5946c class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.37.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="cc20d610-c556-4c76-919a-0451108ae8fb"></a>

###### 2.1.2.4.2.38 Field **fieldname**

###### 2.1.2.4.2.38.1 **fieldname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="2e9b6781-b412-40d3-9f08-f408b4248faa"></a>

###### 2.1.2.4.2.39 Field **originalname**

###### 2.1.2.4.2.39.1 **originalname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>originalname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1723401187sin-titulo-1723399991-punto-boti-1679343550.jpg</td></tr></tbody></table>

### <a id="8434cd88-0982-4a39-b689-52fc4b274836"></a>

###### 2.1.2.4.2.40 Field **encoding**

###### 2.1.2.4.2.40.1 **encoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>encoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>7bit</td></tr></tbody></table>

### <a id="1f211791-7557-4dd0-a34c-a9975c858aac"></a>

###### 2.1.2.4.2.41 Field **mimetype**

###### 2.1.2.4.2.41.1 **mimetype** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mimetype</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="d18cb7cc-4fec-4641-a31d-fc69eb9e6a25"></a>

###### 2.1.2.4.2.42 Field **size**

###### 2.1.2.4.2.42.1 **size** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>size</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>164867</td></tr></tbody></table>

### <a id="52a7a188-a5ae-4591-b4c7-46e6ccdb2608"></a>

###### 2.1.2.4.2.43 Field **bucket**

###### 2.1.2.4.2.43.1 **bucket** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>bucket</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>shopping-rocketfy-uploads</td></tr></tbody></table>

### <a id="0ed37de6-e8b4-4c53-9605-d93d236dc27c"></a>

###### 2.1.2.4.2.44 Field **key**

###### 2.1.2.4.2.44.1 **key** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>key</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1723401187sin-titulo-1723399991-punto-boti-1679343550.jpg</td></tr></tbody></table>

### <a id="9870061b-c105-4088-9e7a-680b84335174"></a>

###### 2.1.2.4.2.45 Field **acl**

###### 2.1.2.4.2.45.1 **acl** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>acl</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>public-read</td></tr></tbody></table>

### <a id="df32f84b-fe4c-46f2-8731-c1245d1e326a"></a>

###### 2.1.2.4.2.46 Field **contentType**

###### 2.1.2.4.2.46.1 **contentType** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentType</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="587c23fe-9c38-4e47-9a7a-80db24077f58"></a>

###### 2.1.2.4.2.47 Field **contentDisposition**

###### 2.1.2.4.2.47.1 **contentDisposition** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentDisposition</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="f98e8d9b-bf72-4588-b53d-3e3548d8e134"></a>

###### 2.1.2.4.2.48 Field **storageClass**

###### 2.1.2.4.2.48.1 **storageClass** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>storageClass</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>STANDARD</td></tr></tbody></table>

### <a id="13624b82-b62b-4835-9a80-87d134927dcf"></a>

###### 2.1.2.4.2.49 Field **serverSideEncryption**

###### 2.1.2.4.2.49.1 **serverSideEncryption** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>serverSideEncryption</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="59566a7c-7fa3-4861-8f05-1f494b0deb29"></a>

###### 2.1.2.4.2.50 Field **metadata**

###### 2.1.2.4.2.50.1 **metadata** Hierarchy

Parent field: **\[0\]**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#7cf6f3e0-56aa-4c9a-a32f-4ee6227b54eb class="margin-NaN">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#41969e74-b22e-4868-b4d3-ad73b3c98720 class="margin-NaN">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.50.2 **metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="7cf6f3e0-56aa-4c9a-a32f-4ee6227b54eb"></a>

###### 2.1.2.4.2.51 Field **fieldName**

###### 2.1.2.4.2.51.1 **fieldName** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldName</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="41969e74-b22e-4868-b4d3-ad73b3c98720"></a>

###### 2.1.2.4.2.52 Field **Content-Type**

###### 2.1.2.4.2.52.1 **Content-Type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Content-Type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="dfbbd87f-45ea-4c69-b2b5-d58fbbd1336b"></a>

###### 2.1.2.4.2.53 Field **location**

###### 2.1.2.4.2.53.1 **location** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>location</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://s3-uploads.rocketfy.co/1723401187sin-titulo-1723399991-punto-boti-1679343550.jpg</td></tr></tbody></table>

### <a id="07f2a018-0bca-40e7-a7c6-730e20673bf0"></a>

###### 2.1.2.4.2.54 Field **etag**

###### 2.1.2.4.2.54.1 **etag** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>etag</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>"2fea26e2662833df6b7be31a4b7b48eb"</td></tr></tbody></table>

### <a id="41e2a047-a61f-4f4f-bf50-7c14241057ab"></a>

###### 2.1.2.4.2.55 Field **versionId**

###### 2.1.2.4.2.55.1 **versionId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>versionId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>TKw1pxW7jXeKFn7UpPmZGf3tL4izYrCK</td></tr></tbody></table>

### <a id="13764987-4119-48fb-9f17-fa71da40b2d2"></a>

###### 2.1.2.4.2.56 Field **principal**

###### 2.1.2.4.2.56.1 **principal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>principal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="1de69ef3-d82b-4292-ae71-457ef7c54466"></a>

###### 2.1.2.4.2.57 Field **status**

###### 2.1.2.4.2.57.1 **status** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>status</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>old</td></tr></tbody></table>

### <a id="be4e276d-98a5-4e53-bf89-4a3cea3755fb"></a>

###### 2.1.2.4.2.58 Field **url**

###### 2.1.2.4.2.58.1 **url** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>url</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://s3-uploads.rocketfy.co/1723401187sin-titulo-1723399991-punto-boti-1679343550.jpg</td></tr></tbody></table>

### <a id="af20d252-1802-4f33-a565-b191be7881e7"></a>

###### 2.1.2.4.2.59 Field **contentEncoding**

###### 2.1.2.4.2.59.1 **contentEncoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentEncoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="807c26ff-66a0-4065-8696-5f5624cd1658"></a>

###### 2.1.2.4.2.60 Field **file**

###### 2.1.2.4.2.60.1 **file** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>file</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="f8c0f7cb-5d1f-43b0-8a5c-bed929d0dfea"></a>

###### 2.1.2.4.2.61 Field **id**

###### 2.1.2.4.2.61.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="aee00cf8-2942-4dab-ac1d-a23e5aa5946c"></a>

###### 2.1.2.4.2.62 Field **name**

###### 2.1.2.4.2.62.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="04997a75-413a-4870-874a-5c9bc2ef9d9e"></a>

###### 2.1.2.4.2.63 Field **created\_time**

###### 2.1.2.4.2.63.1 **created\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1743198295</td></tr></tbody></table>

### <a id="d0208153-6d6e-4a93-8f2a-71ed3fa4cc3c"></a>

###### 2.1.2.4.2.64 Field **attributes**

###### 2.1.2.4.2.64.1 **attributes** Hierarchy

Parent field: **wearehouse\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#41e21b94-e02c-4540-9fac-27d8b301d766 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.64.2 **attributes** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>attributes</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="41e21b94-e02c-4540-9fac-27d8b301d766"></a>

###### 2.1.2.4.2.65 Field **\[0\]**

###### 2.1.2.4.2.65.1 **\[0\]** Hierarchy

Parent field: **attributes**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#caf6598c-20e7-4827-8bbb-7929bc604845 class="margin-NaN">checked</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#062631b4-79a8-4f8b-a9f0-d21d679a0fe5 class="margin-NaN">createItem</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#861316e0-747d-447b-a23f-7457ba847a7c class="margin-NaN">id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b1445f02-295a-40f6-9e7c-035a6b43984e class="margin-NaN">items</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ba43246a-ff27-4b23-8ca6-2e619d81cfdf class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4f0bdda3-c399-4191-9995-6c146c78b6a0 class="margin-NaN">subname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.65.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="caf6598c-20e7-4827-8bbb-7929bc604845"></a>

###### 2.1.2.4.2.66 Field **checked**

###### 2.1.2.4.2.66.1 **checked** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>checked</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="062631b4-79a8-4f8b-a9f0-d21d679a0fe5"></a>

###### 2.1.2.4.2.67 Field **createItem**

###### 2.1.2.4.2.67.1 **createItem** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>createItem</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="861316e0-747d-447b-a23f-7457ba847a7c"></a>

###### 2.1.2.4.2.68 Field **id**

###### 2.1.2.4.2.68.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1360710</td></tr></tbody></table>

### <a id="b1445f02-295a-40f6-9e7c-035a6b43984e"></a>

###### 2.1.2.4.2.69 Field **items**

###### 2.1.2.4.2.69.1 **items** Hierarchy

Parent field: **\[0\]**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#401a37db-2264-4779-988d-60a6203656a9 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.69.2 **items** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>items</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="401a37db-2264-4779-988d-60a6203656a9"></a>

###### 2.1.2.4.2.70 Field **\[0\]**

###### 2.1.2.4.2.70.1 **\[0\]** Hierarchy

Parent field: **items**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#1248952c-fe7d-47db-b67f-07bb2b2a6247 class="margin-NaN">checked</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1c1d82f1-3d6e-48f9-83d7-9d94f64ff7dc class="margin-NaN">id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2d196b74-b3fd-4e24-a197-b785aa7a2297 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.70.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="1248952c-fe7d-47db-b67f-07bb2b2a6247"></a>

###### 2.1.2.4.2.71 Field **checked**

###### 2.1.2.4.2.71.1 **checked** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>checked</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="1c1d82f1-3d6e-48f9-83d7-9d94f64ff7dc"></a>

###### 2.1.2.4.2.72 Field **id**

###### 2.1.2.4.2.72.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>9766693</td></tr></tbody></table>

### <a id="2d196b74-b3fd-4e24-a197-b785aa7a2297"></a>

###### 2.1.2.4.2.73 Field **name**

###### 2.1.2.4.2.73.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>MATCH</td></tr></tbody></table>

### <a id="ba43246a-ff27-4b23-8ca6-2e619d81cfdf"></a>

###### 2.1.2.4.2.74 Field **name**

###### 2.1.2.4.2.74.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>MATCH</td></tr></tbody></table>

### <a id="4f0bdda3-c399-4191-9995-6c146c78b6a0"></a>

###### 2.1.2.4.2.75 Field **subname**

###### 2.1.2.4.2.75.1 **subname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>subname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Agrega las variaciones de MATCH</td></tr></tbody></table>

### <a id="9481ea44-2de0-4b57-a02a-ca50638085c7"></a>

###### 2.1.2.4.2.76 Field **variations**

###### 2.1.2.4.2.76.1 **variations** Hierarchy

Parent field: **wearehouse\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#36c9c6e9-d487-48b1-8287-94a020b214d9 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.76.2 **variations** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>variations</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="36c9c6e9-d487-48b1-8287-94a020b214d9"></a>

###### 2.1.2.4.2.77 Field **\[0\]**

###### 2.1.2.4.2.77.1 **\[0\]** Hierarchy

Parent field: **variations**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#dff3c863-f576-4ce3-ae60-c8f6e0ad2b2d class="margin-NaN">inventory_id</a></td><td class="no-break-word">string,objectId</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#95d0d39a-cb61-4a18-bc8d-97e98790bd10 class="margin-NaN">product_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ca7f119c-4b0c-4381-ac05-b0726b9b92b8 class="margin-NaN">created_time</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ba4f3cf7-e229-4a4a-a96d-17123bc9c416 class="margin-NaN">variation_id</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#eafb0186-1051-4443-9079-1a3711c72be0 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1579c837-5e1d-4d33-8c6b-5b553899c223 class="margin-NaN">sku</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f69e951a-4faf-4656-8d83-1cfc327a9c6a class="margin-NaN">price</a></td><td class="no-break-word">numeric,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fdba763d-5146-42db-9bb6-0b04584b1782 class="margin-NaN">image</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4082af47-080b-4261-808c-8e10aa08609e class="margin-NaN">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0c5d4012-dfd1-4740-9bb4-414c3ee635f8 class="margin-NaN">props</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d9610ecb-d47d-47fc-8011-65fba7e8ac4a class="margin-NaN">_id</a></td><td class="no-break-word">string,objectId</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cff77544-07b7-44bd-b434-47d81e5a90f2 class="margin-NaN">quantity</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8c371cc6-6267-4505-89d6-63690d17b61c class="margin-NaN">establishment_identifier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b832ed7e-09e7-47f6-85c5-417406a7a6e3 class="margin-NaN">id</a></td><td class="no-break-word">string,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a01934f8-9e39-42b5-997e-2ea5be2f843e class="margin-NaN">isValidForm</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#03af50d2-2619-4ae8-bf6f-41f787343684 class="margin-NaN">shopify_variant_id</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.77.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="dff3c863-f576-4ce3-ae60-c8f6e0ad2b2d"></a>

###### 2.1.2.4.2.78 Field **inventory\_id**

###### 2.1.2.4.2.78.1 **inventory\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>inventory_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,objectId)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="95d0d39a-cb61-4a18-bc8d-97e98790bd10"></a>

###### 2.1.2.4.2.79 Field **product\_id**

###### 2.1.2.4.2.79.1 **product\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>product_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>66207d3bf200e414d620744b</td></tr></tbody></table>

### <a id="ca7f119c-4b0c-4381-ac05-b0726b9b92b8"></a>

###### 2.1.2.4.2.80 Field **created\_time**

###### 2.1.2.4.2.80.1 **created\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1713405244</td></tr></tbody></table>

### <a id="ba4f3cf7-e229-4a4a-a96d-17123bc9c416"></a>

###### 2.1.2.4.2.81 Field **variation\_id**

###### 2.1.2.4.2.81.1 **variation\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>variation_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="eafb0186-1051-4443-9079-1a3711c72be0"></a>

###### 2.1.2.4.2.82 Field **name**

###### 2.1.2.4.2.82.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>MATCH</td></tr></tbody></table>

### <a id="1579c837-5e1d-4d33-8c6b-5b553899c223"></a>

###### 2.1.2.4.2.83 Field **sku**

###### 2.1.2.4.2.83.1 **sku** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>sku</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>82587</td></tr></tbody></table>

### <a id="f69e951a-4faf-4656-8d83-1cfc327a9c6a"></a>

###### 2.1.2.4.2.84 Field **price**

###### 2.1.2.4.2.84.1 **price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="fdba763d-5146-42db-9bb6-0b04584b1782"></a>

###### 2.1.2.4.2.85 Field **image**

###### 2.1.2.4.2.85.1 **image** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>image</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4082af47-080b-4261-808c-8e10aa08609e"></a>

###### 2.1.2.4.2.86 Field **active**

###### 2.1.2.4.2.86.1 **active** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>active</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="0c5d4012-dfd1-4740-9bb4-414c3ee635f8"></a>

###### 2.1.2.4.2.87 Field **props**

###### 2.1.2.4.2.87.1 **props** Hierarchy

Parent field: **\[0\]**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#eb21ce0d-3a0e-45eb-8854-6ed189944d6e class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.87.2 **props** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>props</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="eb21ce0d-3a0e-45eb-8854-6ed189944d6e"></a>

###### 2.1.2.4.2.88 Field **\[0\]**

###### 2.1.2.4.2.88.1 **\[0\]** Hierarchy

Parent field: **props**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#48c56190-fccd-47f3-81b8-4f43ade6e719 class="margin-NaN">id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8ee2a0e1-ebe5-401b-a848-22c75a666b67 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3a34c835-bc81-4cee-9550-31be9e37b987 class="margin-NaN">attr_id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c1c38d99-7fd0-4176-92e4-a8cbd8a0e035 class="margin-NaN">attr_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.88.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="48c56190-fccd-47f3-81b8-4f43ade6e719"></a>

###### 2.1.2.4.2.89 Field **id**

###### 2.1.2.4.2.89.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>9766693</td></tr></tbody></table>

### <a id="8ee2a0e1-ebe5-401b-a848-22c75a666b67"></a>

###### 2.1.2.4.2.90 Field **name**

###### 2.1.2.4.2.90.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>MATCH</td></tr></tbody></table>

### <a id="3a34c835-bc81-4cee-9550-31be9e37b987"></a>

###### 2.1.2.4.2.91 Field **attr\_id**

###### 2.1.2.4.2.91.1 **attr\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>attr_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1360710</td></tr></tbody></table>

### <a id="c1c38d99-7fd0-4176-92e4-a8cbd8a0e035"></a>

###### 2.1.2.4.2.92 Field **attr\_name**

###### 2.1.2.4.2.92.1 **attr\_name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>attr_name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>MATCH</td></tr></tbody></table>

### <a id="d9610ecb-d47d-47fc-8011-65fba7e8ac4a"></a>

###### 2.1.2.4.2.93 Field **\_id**

###### 2.1.2.4.2.93.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,objectId)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="cff77544-07b7-44bd-b434-47d81e5a90f2"></a>

###### 2.1.2.4.2.94 Field **quantity**

###### 2.1.2.4.2.94.1 **quantity** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>quantity</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8c371cc6-6267-4505-89d6-63690d17b61c"></a>

###### 2.1.2.4.2.95 Field **establishment\_identifier**

###### 2.1.2.4.2.95.1 **establishment\_identifier** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>establishment_identifier</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="b832ed7e-09e7-47f6-85c5-417406a7a6e3"></a>

###### 2.1.2.4.2.96 Field **id**

###### 2.1.2.4.2.96.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a01934f8-9e39-42b5-997e-2ea5be2f843e"></a>

###### 2.1.2.4.2.97 Field **isValidForm**

###### 2.1.2.4.2.97.1 **isValidForm** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>isValidForm</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="03af50d2-2619-4ae8-bf6f-41f787343684"></a>

###### 2.1.2.4.2.98 Field **shopify\_variant\_id**

###### 2.1.2.4.2.98.1 **shopify\_variant\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shopify_variant_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4198a7e9-c4e9-4985-9832-60a836aacfbc"></a>

###### 2.1.2.4.2.99 Field **dimensions**

###### 2.1.2.4.2.99.1 **dimensions** Hierarchy

Parent field: **wearehouse\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#153d0f68-9207-4ae1-a929-e0d03c810f4c class="margin-NaN">width</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#56d25285-4d3c-42c6-a3a6-0bea03154be8 class="margin-NaN">height</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8f28afc2-3d58-47bd-8321-8331873748c4 class="margin-NaN">large</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#53754a7e-ace2-4181-b918-d12c1222b52f class="margin-NaN">volume</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c28da140-ea24-47ae-8f3c-3d2a17164393 class="margin-NaN">weight</a></td><td class="no-break-word">numeric,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e557c278-1f38-4e1c-a3d3-2f4392825737 class="margin-NaN">weight_in_unit</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ab34e0b5-2c2b-4fc2-89f5-f41b3c157901 class="margin-NaN">weight_unit</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.99.2 **dimensions** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dimensions</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="153d0f68-9207-4ae1-a929-e0d03c810f4c"></a>

###### 2.1.2.4.2.100 Field **width**

###### 2.1.2.4.2.100.1 **width** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>width</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>11.5</td></tr></tbody></table>

### <a id="56d25285-4d3c-42c6-a3a6-0bea03154be8"></a>

###### 2.1.2.4.2.101 Field **height**

###### 2.1.2.4.2.101.1 **height** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>height</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>7.1</td></tr></tbody></table>

### <a id="8f28afc2-3d58-47bd-8321-8331873748c4"></a>

###### 2.1.2.4.2.102 Field **large**

###### 2.1.2.4.2.102.1 **large** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>large</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>2.3</td></tr></tbody></table>

### <a id="53754a7e-ace2-4181-b918-d12c1222b52f"></a>

###### 2.1.2.4.2.103 Field **volume**

###### 2.1.2.4.2.103.1 **volume** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>volume</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1012.5</td></tr></tbody></table>

### <a id="c28da140-ea24-47ae-8f3c-3d2a17164393"></a>

###### 2.1.2.4.2.104 Field **weight**

###### 2.1.2.4.2.104.1 **weight** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>weight</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="e557c278-1f38-4e1c-a3d3-2f4392825737"></a>

###### 2.1.2.4.2.105 Field **weight\_in\_unit**

###### 2.1.2.4.2.105.1 **weight\_in\_unit** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>weight_in_unit</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0.5</td></tr></tbody></table>

### <a id="ab34e0b5-2c2b-4fc2-89f5-f41b3c157901"></a>

###### 2.1.2.4.2.106 Field **weight\_unit**

###### 2.1.2.4.2.106.1 **weight\_unit** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>weight_unit</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>kg</td></tr></tbody></table>

### <a id="de15d260-fdc7-4111-8989-ed978ea0cc9f"></a>

###### 2.1.2.4.2.107 Field **metadata**

###### 2.1.2.4.2.107.1 **metadata** Hierarchy

Parent field: **wearehouse\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#cc0c4c86-32ed-4823-919e-833be8de1c7c class="margin-NaN">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.107.2 **metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (array,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="cc0c4c86-32ed-4823-919e-833be8de1c7c"></a>

###### 2.1.2.4.2.108 Field **items**

###### 2.1.2.4.2.108.1 **items** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="138039d9-dbbc-4ee0-a161-22f6dfea3a6e"></a>

###### 2.1.2.4.2.109 Field **category\_id**

###### 2.1.2.4.2.109.1 **category\_id** Hierarchy

Parent field: **wearehouse\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#cd48ea2c-5930-4da3-a57d-312d75162972 class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a34020f6-631a-4a01-be65-3ad8db8a1047 class="margin-NaN">name</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.109.2 **category\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>category_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="cd48ea2c-5930-4da3-a57d-312d75162972"></a>

###### 2.1.2.4.2.110 Field **id**

###### 2.1.2.4.2.110.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>5f6bbe0d988fee49206329cc</td></tr></tbody></table>

### <a id="a34020f6-631a-4a01-be65-3ad8db8a1047"></a>

###### 2.1.2.4.2.111 Field **name**

###### 2.1.2.4.2.111.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="376da31f-c510-4555-aefa-3524e3121085"></a>

###### 2.1.2.4.2.112 Field **warehouse**

###### 2.1.2.4.2.112.1 **warehouse** Hierarchy

Parent field: **wearehouse\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#068b30f9-a7a0-4622-bd0a-7bfdcadb1376 class="margin-NaN">shipping</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7f50dbfb-516e-4e7f-bf70-4699e2775607 class="margin-NaN">suggested_price</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0b875cb7-bcc3-4b53-8daa-b3ec4e4caabf class="margin-NaN">warehouse_price</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#392086f8-7177-4919-ab8c-26b30583a975 class="margin-NaN">discount</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5baa84a1-57e3-4706-ab79-209ea7a58515 class="margin-NaN">id_warehouse_rkf</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#37d310d2-d657-45b2-a704-7490e3793d96 class="margin-NaN">data</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#de4db032-096a-430d-9348-3949db3d0221 class="margin-NaN">statistics</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#76982eaa-d18c-47dd-a243-c6efe67eb068 class="margin-NaN">father_id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d534c787-307d-4f46-b09e-2b7eaca551fa class="margin-NaN">shared_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#74fb6938-13c1-439a-8fd7-f3aa8c11f5ae class="margin-NaN">suggestions</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.112.2 **warehouse** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>warehouse</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="068b30f9-a7a0-4622-bd0a-7bfdcadb1376"></a>

###### 2.1.2.4.2.113 Field **shipping**

###### 2.1.2.4.2.113.1 **shipping** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shipping</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="7f50dbfb-516e-4e7f-bf70-4699e2775607"></a>

###### 2.1.2.4.2.114 Field **suggested\_price**

###### 2.1.2.4.2.114.1 **suggested\_price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>suggested_price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>131.3</td></tr></tbody></table>

### <a id="0b875cb7-bcc3-4b53-8daa-b3ec4e4caabf"></a>

###### 2.1.2.4.2.115 Field **warehouse\_price**

###### 2.1.2.4.2.115.1 **warehouse\_price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>warehouse_price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="392086f8-7177-4919-ab8c-26b30583a975"></a>

###### 2.1.2.4.2.116 Field **discount**

###### 2.1.2.4.2.116.1 **discount** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>discount</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5baa84a1-57e3-4706-ab79-209ea7a58515"></a>

###### 2.1.2.4.2.117 Field **id\_warehouse\_rkf**

###### 2.1.2.4.2.117.1 **id\_warehouse\_rkf** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id_warehouse_rkf</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>d5aaa6c2-e62b-49bc-8fa6-23c21aabcb57</td></tr></tbody></table>

### <a id="37d310d2-d657-45b2-a704-7490e3793d96"></a>

###### 2.1.2.4.2.118 Field **data**

###### 2.1.2.4.2.118.1 **data** Hierarchy

Parent field: **warehouse**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#66a2eb12-dd46-4049-b392-143bf5aaccef class="margin-NaN">db_seller</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fb3e16ff-28e1-422e-bdeb-bd35c5eebeb6 class="margin-NaN">only_my_stores</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a17e1a7d-dfad-4c74-a334-ca7116e9a093 class="margin-NaN">shop</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#47fa6237-2ab0-42c4-9a0c-690c12297ffc class="margin-NaN">rem</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.118.2 **data** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>data</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="66a2eb12-dd46-4049-b392-143bf5aaccef"></a>

###### 2.1.2.4.2.119 Field **db\_seller**

###### 2.1.2.4.2.119.1 **db\_seller** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>db_seller</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>piezaapieza_986789376</td></tr></tbody></table>

### <a id="fb3e16ff-28e1-422e-bdeb-bd35c5eebeb6"></a>

###### 2.1.2.4.2.120 Field **only\_my\_stores**

###### 2.1.2.4.2.120.1 **only\_my\_stores** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>only_my_stores</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="a17e1a7d-dfad-4c74-a334-ca7116e9a093"></a>

###### 2.1.2.4.2.121 Field **shop**

###### 2.1.2.4.2.121.1 **shop** Hierarchy

Parent field: **data**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#cb32a604-386e-4509-8296-2bb752cee0cc class="margin-NaN">name</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2da13e9a-1830-4a4f-8702-9ad5919d4a17 class="margin-NaN">email</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cb8a21bb-8888-41bc-89d0-ff07c42fe810 class="margin-NaN">cc_nit</a></td><td class="no-break-word">string,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cd5813da-4e1f-44ef-bf46-d3f348ff049f class="margin-NaN">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ff324031-f559-4c96-9cbf-fbf9e98c6f6e class="margin-NaN">composed_address</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#76603c15-d572-40d9-8bd9-bf30e462b54e class="margin-NaN">cod_postal</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#76a6f72b-779c-473d-8bca-48c364669204 class="margin-NaN">country</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a02eab7a-ddbd-450f-b686-f214fd0dcc92 class="margin-NaN">city</a></td><td class="no-break-word">document,string,null</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#19082597-3d34-4501-bfa7-38b93dc31613 class="margin-NaN">departament</a></td><td class="no-break-word">document,string,null</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f43d764e-b745-4c25-ae8a-546e59c823a6 class="margin-NaN">slogan</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2ca4af40-07e2-47df-80a5-f697e51647fa class="margin-NaN">color_primary</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d6b0d42d-4096-48c6-b6dc-71c27bc7c0e8 class="margin-NaN">colors</a></td><td class="no-break-word">array,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3b728b9f-2d7b-4c62-a09b-ed80c6a22f78 class="margin-NaN">large_description</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ec652a65-5d8e-49b6-824d-1bad308deea1 class="margin-NaN">logo</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ed266c9c-644d-49bf-b478-ecd7fdbc5f47 class="margin-NaN">banner</a></td><td class="no-break-word">document,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2b658d3a-25aa-4140-b87b-22d4281fecdc class="margin-NaN">promises</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0a9a7fc4-aa96-473b-8d7e-a691dcaaf15b class="margin-NaN">social</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b5cced4b-b372-42dd-a837-c2c8ab5e52e6 class="margin-NaN">horary</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d07012e7-6097-4a26-a193-80b7f3acc375 class="margin-NaN">neighborhood</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#eae2c42d-c1a3-4fec-a106-034bb25bc62c class="margin-NaN">location</a></td><td class="no-break-word">document,null,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e3d7dd9d-6ec9-436f-9232-524a60161021 class="margin-NaN">tel</a></td><td class="no-break-word">numeric,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#49bd41a3-a3e4-4b2f-a591-138e4ca74dc5 class="margin-NaN">payments</a></td><td class="no-break-word">document,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2ca7fb7d-789c-484c-85b9-9c4cff5f2055 class="margin-NaN">principal_address</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fff19708-f19e-4268-984e-f4efb922d5d8 class="margin-NaN">carry</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#664f931c-2fe7-46ae-bc20-20d21a9adf96 class="margin-NaN">geolocation</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ab2ae1fa-334f-4bb3-8f60-353b9ffbf0e2 class="margin-NaN">default</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#368ed2fd-0df8-4ce0-a1f5-bdf14f20dfb4 class="margin-NaN">gtag</a></td><td class="no-break-word">null,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#25529cf4-1e9d-49de-a16d-a128d56beaa5 class="margin-NaN">indicative</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8408f5f2-e892-488d-ab06-41e8194cc0e8 class="margin-NaN">pixel</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.121.2 **shop** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shop</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="cb32a604-386e-4509-8296-2bb752cee0cc"></a>

###### 2.1.2.4.2.122 Field **name**

###### 2.1.2.4.2.122.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="2da13e9a-1830-4a4f-8702-9ad5919d4a17"></a>

###### 2.1.2.4.2.123 Field **email**

###### 2.1.2.4.2.123.1 **email** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>email</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>rocketfybodega@gmail.com</td></tr></tbody></table>

### <a id="cb8a21bb-8888-41bc-89d0-ff07c42fe810"></a>

###### 2.1.2.4.2.124 Field **cc\_nit**

###### 2.1.2.4.2.124.1 **cc\_nit** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cc_nit</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="cd5813da-4e1f-44ef-bf46-d3f348ff049f"></a>

###### 2.1.2.4.2.125 Field **address**

###### 2.1.2.4.2.125.1 **address** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>address</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Calle 27 # 27b - 15</td></tr></tbody></table>

### <a id="ff324031-f559-4c96-9cbf-fbf9e98c6f6e"></a>

###### 2.1.2.4.2.126 Field **composed\_address**

###### 2.1.2.4.2.126.1 **composed\_address** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#ce8a4cf2-0aa8-4bef-a87d-e39ae88fe316 class="margin-NaN">street</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f90a9167-7dbe-4bf7-829d-e4048a5b79df class="margin-NaN">street_number_one</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dd646760-4995-4dda-b2d5-eb38328d5735 class="margin-NaN">street_number_two</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.126.2 **composed\_address** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>composed_address</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="ce8a4cf2-0aa8-4bef-a87d-e39ae88fe316"></a>

###### 2.1.2.4.2.127 Field **street**

###### 2.1.2.4.2.127.1 **street** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>street</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Calle 27</td></tr></tbody></table>

### <a id="f90a9167-7dbe-4bf7-829d-e4048a5b79df"></a>

###### 2.1.2.4.2.128 Field **street\_number\_one**

###### 2.1.2.4.2.128.1 **street\_number\_one** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>street_number_one</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>27b</td></tr></tbody></table>

### <a id="dd646760-4995-4dda-b2d5-eb38328d5735"></a>

###### 2.1.2.4.2.129 Field **street\_number\_two**

###### 2.1.2.4.2.129.1 **street\_number\_two** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>street_number_two</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>15</td></tr></tbody></table>

### <a id="76603c15-d572-40d9-8bd9-bf30e462b54e"></a>

###### 2.1.2.4.2.130 Field **cod\_postal**

###### 2.1.2.4.2.130.1 **cod\_postal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cod_postal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>050021</td></tr></tbody></table>

### <a id="76a6f72b-779c-473d-8bca-48c364669204"></a>

###### 2.1.2.4.2.131 Field **country**

###### 2.1.2.4.2.131.1 **country** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>COL</td></tr></tbody></table>

### <a id="a02eab7a-ddbd-450f-b686-f214fd0dcc92"></a>

###### 2.1.2.4.2.132 Field **city**

###### 2.1.2.4.2.132.1 **city** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#d3760f6a-f6f8-4391-8a86-4e33c633d5f0 class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.132.2 **city** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>city</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (document,string,null)</td></tr><tr><td></td><td>[object Object],[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="d3760f6a-f6f8-4391-8a86-4e33c633d5f0"></a>

###### 2.1.2.4.2.133 Field **properties**

###### 2.1.2.4.2.133.1 **properties** Hierarchy

Parent field: **city**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#e1fe952b-f176-4ec4-8a4a-aaa772a8aa8f class="margin-NaN">_id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0ac94e9a-54d5-4912-b7a8-622a659b7dae class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8a88ea5e-a285-496e-9b0c-dc83ef1da5d2 class="margin-NaN">before_courrier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8f4acb12-a9c4-40f0-a12a-259afce52a90 class="margin-NaN">checked</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ae19f329-a7aa-4b57-997f-6084396f10b1 class="margin-NaN">city_code</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1fdf17bb-66a2-4f3c-a632-c9dac041feb3 class="margin-NaN">cod_depto</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#43c2e8a6-6406-47f4-800e-3a595333fe2a class="margin-NaN">country</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ee0f2f87-ecd3-4380-ac78-09166d6b2e5b class="margin-NaN">courrier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#56888e8e-e7f5-4bf5-b243-679de6e3d8c0 class="margin-NaN">dane_code</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c3d41599-d117-4246-a6a2-40f6397fd8b0 class="margin-NaN">disabled</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9339521a-69e5-49b2-b6e8-a7de8c0e3050 class="margin-NaN">forTest</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#931dd7fc-0beb-4a22-b8d5-7a02800bace1 class="margin-NaN">postal_code</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7aa9de0f-1cd8-43e9-bfeb-5f1186b742df class="margin-NaN">shipping_zone</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4c36e4ae-a695-4974-880f-75fed6a7f49a class="margin-NaN">shop_error</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d2ac6498-67a9-4761-8b09-2f16d3b2b79e class="margin-NaN">state</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.133.2 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="e1fe952b-f176-4ec4-8a4a-aaa772a8aa8f"></a>

###### 2.1.2.4.2.134 Field **\_id**

###### 2.1.2.4.2.134.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="0ac94e9a-54d5-4912-b7a8-622a659b7dae"></a>

###### 2.1.2.4.2.135 Field **name**

###### 2.1.2.4.2.135.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8a88ea5e-a285-496e-9b0c-dc83ef1da5d2"></a>

###### 2.1.2.4.2.136 Field **before\_courrier**

###### 2.1.2.4.2.136.1 **before\_courrier** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>before_courrier</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8f4acb12-a9c4-40f0-a12a-259afce52a90"></a>

###### 2.1.2.4.2.137 Field **checked**

###### 2.1.2.4.2.137.1 **checked** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>checked</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ae19f329-a7aa-4b57-997f-6084396f10b1"></a>

###### 2.1.2.4.2.138 Field **city\_code**

###### 2.1.2.4.2.138.1 **city\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>city_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="1fdf17bb-66a2-4f3c-a632-c9dac041feb3"></a>

###### 2.1.2.4.2.139 Field **cod\_depto**

###### 2.1.2.4.2.139.1 **cod\_depto** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cod_depto</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="43c2e8a6-6406-47f4-800e-3a595333fe2a"></a>

###### 2.1.2.4.2.140 Field **country**

###### 2.1.2.4.2.140.1 **country** Hierarchy

Parent field: **properties**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#d279953c-35ce-4b03-b483-115bdeefca53 class="margin-NaN">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7313d16a-58a4-414e-8636-e075d60ab46f class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7c96330d-4281-4a42-a123-5a92d7ae2e5a class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.140.2 **country** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="d279953c-35ce-4b03-b483-115bdeefca53"></a>

###### 2.1.2.4.2.141 Field **code**

###### 2.1.2.4.2.141.1 **code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="7313d16a-58a4-414e-8636-e075d60ab46f"></a>

###### 2.1.2.4.2.142 Field **id**

###### 2.1.2.4.2.142.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="7c96330d-4281-4a42-a123-5a92d7ae2e5a"></a>

###### 2.1.2.4.2.143 Field **name**

###### 2.1.2.4.2.143.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ee0f2f87-ecd3-4380-ac78-09166d6b2e5b"></a>

###### 2.1.2.4.2.144 Field **courrier**

###### 2.1.2.4.2.144.1 **courrier** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>courrier</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="56888e8e-e7f5-4bf5-b243-679de6e3d8c0"></a>

###### 2.1.2.4.2.145 Field **dane\_code**

###### 2.1.2.4.2.145.1 **dane\_code** Hierarchy

Parent field: **properties**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#cec2bb55-ad49-4b45-b694-fb18156597cd class="margin-NaN">rocketfy</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b67690e1-eddf-4874-8516-aa7f7cc96dba class="margin-NaN">servientrega</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.145.2 **dane\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dane_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="cec2bb55-ad49-4b45-b694-fb18156597cd"></a>

###### 2.1.2.4.2.146 Field **rocketfy**

###### 2.1.2.4.2.146.1 **rocketfy** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>rocketfy</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="b67690e1-eddf-4874-8516-aa7f7cc96dba"></a>

###### 2.1.2.4.2.147 Field **servientrega**

###### 2.1.2.4.2.147.1 **servientrega** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>servientrega</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c3d41599-d117-4246-a6a2-40f6397fd8b0"></a>

###### 2.1.2.4.2.148 Field **disabled**

###### 2.1.2.4.2.148.1 **disabled** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>disabled</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="9339521a-69e5-49b2-b6e8-a7de8c0e3050"></a>

###### 2.1.2.4.2.149 Field **forTest**

###### 2.1.2.4.2.149.1 **forTest** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>forTest</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="931dd7fc-0beb-4a22-b8d5-7a02800bace1"></a>

###### 2.1.2.4.2.150 Field **postal\_code**

###### 2.1.2.4.2.150.1 **postal\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>postal_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="7aa9de0f-1cd8-43e9-bfeb-5f1186b742df"></a>

###### 2.1.2.4.2.151 Field **shipping\_zone**

###### 2.1.2.4.2.151.1 **shipping\_zone** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shipping_zone</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4c36e4ae-a695-4974-880f-75fed6a7f49a"></a>

###### 2.1.2.4.2.152 Field **shop\_error**

###### 2.1.2.4.2.152.1 **shop\_error** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shop_error</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="d2ac6498-67a9-4761-8b09-2f16d3b2b79e"></a>

###### 2.1.2.4.2.153 Field **state**

###### 2.1.2.4.2.153.1 **state** Hierarchy

Parent field: **properties**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#8ff4fb9a-334b-4791-a9da-a5cbf04fefd6 class="margin-NaN">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5af11d58-85f5-4782-ae48-7ffc0df978bf class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c9d2e4c1-d59a-4172-86af-94442e72c94f class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.153.2 **state** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>state</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="8ff4fb9a-334b-4791-a9da-a5cbf04fefd6"></a>

###### 2.1.2.4.2.154 Field **code**

###### 2.1.2.4.2.154.1 **code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5af11d58-85f5-4782-ae48-7ffc0df978bf"></a>

###### 2.1.2.4.2.155 Field **id**

###### 2.1.2.4.2.155.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c9d2e4c1-d59a-4172-86af-94442e72c94f"></a>

###### 2.1.2.4.2.156 Field **name**

###### 2.1.2.4.2.156.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="19082597-3d34-4501-bfa7-38b93dc31613"></a>

###### 2.1.2.4.2.157 Field **departament**

###### 2.1.2.4.2.157.1 **departament** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#b4ea8a1e-56e6-4f26-a7f1-b94e1a1409ff class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.157.2 **departament** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>departament</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (document,string,null)</td></tr><tr><td></td><td>[object Object],[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="b4ea8a1e-56e6-4f26-a7f1-b94e1a1409ff"></a>

###### 2.1.2.4.2.158 Field **properties**

###### 2.1.2.4.2.158.1 **properties** Hierarchy

Parent field: **departament**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#a81be04d-79cd-45be-94ab-26682312f9f7 class="margin-NaN">_id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#96f5654b-df8c-4c2e-8136-8f4d48ffe239 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#010738bc-12a4-4d98-9334-fa85929a095c class="margin-NaN">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#14154ed1-7a73-45f4-acd3-3f252bfe64a8 class="margin-NaN">country</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#26bfb226-c315-494d-9e6c-2744511b5c33 class="margin-NaN">disabled</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.158.2 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="a81be04d-79cd-45be-94ab-26682312f9f7"></a>

###### 2.1.2.4.2.159 Field **\_id**

###### 2.1.2.4.2.159.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="96f5654b-df8c-4c2e-8136-8f4d48ffe239"></a>

###### 2.1.2.4.2.160 Field **name**

###### 2.1.2.4.2.160.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="010738bc-12a4-4d98-9334-fa85929a095c"></a>

###### 2.1.2.4.2.161 Field **code**

###### 2.1.2.4.2.161.1 **code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="14154ed1-7a73-45f4-acd3-3f252bfe64a8"></a>

###### 2.1.2.4.2.162 Field **country**

###### 2.1.2.4.2.162.1 **country** Hierarchy

Parent field: **properties**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#3203b6b3-c6c1-4348-99b1-3e4fc91a7a27 class="margin-NaN">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#465a2a36-ecc8-4123-bea1-316532de8b28 class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a8e6f79e-c3b7-4cd5-9ae8-3ccfa8d573ba class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.162.2 **country** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="3203b6b3-c6c1-4348-99b1-3e4fc91a7a27"></a>

###### 2.1.2.4.2.163 Field **code**

###### 2.1.2.4.2.163.1 **code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="465a2a36-ecc8-4123-bea1-316532de8b28"></a>

###### 2.1.2.4.2.164 Field **id**

###### 2.1.2.4.2.164.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a8e6f79e-c3b7-4cd5-9ae8-3ccfa8d573ba"></a>

###### 2.1.2.4.2.165 Field **name**

###### 2.1.2.4.2.165.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="26bfb226-c315-494d-9e6c-2744511b5c33"></a>

###### 2.1.2.4.2.166 Field **disabled**

###### 2.1.2.4.2.166.1 **disabled** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>disabled</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="f43d764e-b745-4c25-ae8a-546e59c823a6"></a>

###### 2.1.2.4.2.167 Field **slogan**

###### 2.1.2.4.2.167.1 **slogan** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>slogan</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="2ca4af40-07e2-47df-80a5-f697e51647fa"></a>

###### 2.1.2.4.2.168 Field **color\_primary**

###### 2.1.2.4.2.168.1 **color\_primary** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>color_primary</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>#d54c43</td></tr></tbody></table>

### <a id="d6b0d42d-4096-48c6-b6dc-71c27bc7c0e8"></a>

###### 2.1.2.4.2.169 Field **colors**

###### 2.1.2.4.2.169.1 **colors** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#3753b497-6d51-42b2-be23-92d9d22c6e71 class="margin-NaN">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.169.2 **colors** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>colors</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (array,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="3753b497-6d51-42b2-be23-92d9d22c6e71"></a>

###### 2.1.2.4.2.170 Field **items**

###### 2.1.2.4.2.170.1 **items** Hierarchy

Parent field: **colors**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#09558d09-cae0-4953-a1a4-3a4494a3030c class="margin-NaN">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.170.2 **items** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="09558d09-cae0-4953-a1a4-3a4494a3030c"></a>

###### 2.1.2.4.2.171 Field **\[0\]**

###### 2.1.2.4.2.171.1 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr></tbody></table>

### <a id="3b728b9f-2d7b-4c62-a09b-ed80c6a22f78"></a>

###### 2.1.2.4.2.172 Field **large\_description**

###### 2.1.2.4.2.172.1 **large\_description** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>large_description</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ec652a65-5d8e-49b6-824d-1bad308deea1"></a>

###### 2.1.2.4.2.173 Field **logo**

###### 2.1.2.4.2.173.1 **logo** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#1efa5b3f-9e74-4211-92b5-268908523510 class="margin-NaN">fieldname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e39551b2-2e13-46af-9dd4-164455f4a16a class="margin-NaN">originalname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c28cac81-ddd5-43a5-9400-13bdf8673a0c class="margin-NaN">encoding</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8f0319a4-63ef-48bc-83da-29c11382cbb0 class="margin-NaN">mimetype</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a6ecdd77-01e8-4631-ae51-5c5a001c0122 class="margin-NaN">size</a></td><td class="no-break-word">numeric,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8b918670-80f6-4dc2-966b-30214b0725a2 class="margin-NaN">bucket</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e3f9a06b-adfa-4d49-82f7-60af95727a80 class="margin-NaN">key</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#10573aff-eaf5-45b5-bed2-5168e1c391ea class="margin-NaN">acl</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6889b61a-4a50-4e12-aef2-deb044ddc957 class="margin-NaN">contentType</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d11c913b-fe77-4c4e-bd85-a3b87ac4c9b7 class="margin-NaN">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bfd04098-651e-4439-9656-ffd0ff8eaf5e class="margin-NaN">storageClass</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#35e94ad9-7198-4a93-a7c1-67dc091d18ba class="margin-NaN">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ada8171d-4f17-42f3-893e-099d2dc6b408 class="margin-NaN">metadata</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#96417e62-92c7-4def-bb55-e75fcb07350a class="margin-NaN">location</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5407cc7e-beb2-4bd7-a130-b767c121385c class="margin-NaN">etag</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6b25c1ab-d950-4432-87c1-19d58a3de6e8 class="margin-NaN">versionId</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cc9e36a0-ed42-4d00-bf92-2ec8a3557110 class="margin-NaN">contentEncoding</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#374732ff-688e-4207-b57e-9b2e600fa118 class="margin-NaN">created_time</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.173.2 **logo** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>logo</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="1efa5b3f-9e74-4211-92b5-268908523510"></a>

###### 2.1.2.4.2.174 Field **fieldname**

###### 2.1.2.4.2.174.1 **fieldname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="e39551b2-2e13-46af-9dd4-164455f4a16a"></a>

###### 2.1.2.4.2.175 Field **originalname**

###### 2.1.2.4.2.175.1 **originalname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>originalname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>piezaapieza_986789376_piezapieza__3_-removebg-preview.png</td></tr></tbody></table>

### <a id="c28cac81-ddd5-43a5-9400-13bdf8673a0c"></a>

###### 2.1.2.4.2.176 Field **encoding**

###### 2.1.2.4.2.176.1 **encoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>encoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>7bit</td></tr></tbody></table>

### <a id="8f0319a4-63ef-48bc-83da-29c11382cbb0"></a>

###### 2.1.2.4.2.177 Field **mimetype**

###### 2.1.2.4.2.177.1 **mimetype** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mimetype</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/png</td></tr></tbody></table>

### <a id="a6ecdd77-01e8-4631-ae51-5c5a001c0122"></a>

###### 2.1.2.4.2.178 Field **size**

###### 2.1.2.4.2.178.1 **size** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>size</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8b918670-80f6-4dc2-966b-30214b0725a2"></a>

###### 2.1.2.4.2.179 Field **bucket**

###### 2.1.2.4.2.179.1 **bucket** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>bucket</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>shopping-rocketfy-uploads</td></tr></tbody></table>

### <a id="e3f9a06b-adfa-4d49-82f7-60af95727a80"></a>

###### 2.1.2.4.2.180 Field **key**

###### 2.1.2.4.2.180.1 **key** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>key</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>piezaapieza_986789376_piezapieza__3_-removebg-preview.png</td></tr></tbody></table>

### <a id="10573aff-eaf5-45b5-bed2-5168e1c391ea"></a>

###### 2.1.2.4.2.181 Field **acl**

###### 2.1.2.4.2.181.1 **acl** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>acl</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>public-read</td></tr></tbody></table>

### <a id="6889b61a-4a50-4e12-aef2-deb044ddc957"></a>

###### 2.1.2.4.2.182 Field **contentType**

###### 2.1.2.4.2.182.1 **contentType** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentType</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/png</td></tr></tbody></table>

### <a id="d11c913b-fe77-4c4e-bd85-a3b87ac4c9b7"></a>

###### 2.1.2.4.2.183 Field **contentDisposition**

###### 2.1.2.4.2.183.1 **contentDisposition** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentDisposition</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="bfd04098-651e-4439-9656-ffd0ff8eaf5e"></a>

###### 2.1.2.4.2.184 Field **storageClass**

###### 2.1.2.4.2.184.1 **storageClass** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>storageClass</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>STANDARD</td></tr></tbody></table>

### <a id="35e94ad9-7198-4a93-a7c1-67dc091d18ba"></a>

###### 2.1.2.4.2.185 Field **serverSideEncryption**

###### 2.1.2.4.2.185.1 **serverSideEncryption** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>serverSideEncryption</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ada8171d-4f17-42f3-893e-099d2dc6b408"></a>

###### 2.1.2.4.2.186 Field **metadata**

###### 2.1.2.4.2.186.1 **metadata** Hierarchy

Parent field: **logo**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#56af53f0-0b62-4d9f-90c4-5c3f37c6def2 class="margin-NaN">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cb89aaad-290e-425a-94e1-50c582feba59 class="margin-NaN">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.186.2 **metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="56af53f0-0b62-4d9f-90c4-5c3f37c6def2"></a>

###### 2.1.2.4.2.187 Field **fieldName**

###### 2.1.2.4.2.187.1 **fieldName** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldName</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="cb89aaad-290e-425a-94e1-50c582feba59"></a>

###### 2.1.2.4.2.188 Field **Content-Type**

###### 2.1.2.4.2.188.1 **Content-Type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Content-Type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/png</td></tr></tbody></table>

### <a id="96417e62-92c7-4def-bb55-e75fcb07350a"></a>

###### 2.1.2.4.2.189 Field **location**

###### 2.1.2.4.2.189.1 **location** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>location</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://s3-uploads.rocketfy.co/piezaapieza_986789376_piezapieza__3_-removebg-preview.png</td></tr></tbody></table>

### <a id="5407cc7e-beb2-4bd7-a130-b767c121385c"></a>

###### 2.1.2.4.2.190 Field **etag**

###### 2.1.2.4.2.190.1 **etag** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>etag</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>"8f6e2ce5f4320717320c036943e4edf1"</td></tr></tbody></table>

### <a id="6b25c1ab-d950-4432-87c1-19d58a3de6e8"></a>

###### 2.1.2.4.2.191 Field **versionId**

###### 2.1.2.4.2.191.1 **versionId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>versionId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>FtAQQPvtf6DUNZeXRlIETiB7BPtf2CCe</td></tr></tbody></table>

### <a id="cc9e36a0-ed42-4d00-bf92-2ec8a3557110"></a>

###### 2.1.2.4.2.192 Field **contentEncoding**

###### 2.1.2.4.2.192.1 **contentEncoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentEncoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="374732ff-688e-4207-b57e-9b2e600fa118"></a>

###### 2.1.2.4.2.193 Field **created\_time**

###### 2.1.2.4.2.193.1 **created\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ed266c9c-644d-49bf-b478-ecd7fdbc5f47"></a>

###### 2.1.2.4.2.194 Field **banner**

###### 2.1.2.4.2.194.1 **banner** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#b7e25618-182d-496a-98e9-624fc445511c class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.194.2 **banner** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>banner</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (document,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="b7e25618-182d-496a-98e9-624fc445511c"></a>

###### 2.1.2.4.2.195 Field **properties**

###### 2.1.2.4.2.195.1 **properties** Hierarchy

Parent field: **banner**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#6dc205dc-5b8d-4b7c-9b4c-2735d9d25f2d class="margin-NaN">location</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#00b68081-332e-46d7-afd7-94c697cac71a class="margin-NaN">acl</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#85e9382e-3ad1-4ef6-b6e9-5d2fdee3d0ed class="margin-NaN">bucket</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8668d108-b364-45e2-bff7-d087d82cde54 class="margin-NaN">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#df2dc48b-bd5d-4615-8ab5-185c88a71d53 class="margin-NaN">contentEncoding</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#84ecf8d8-fdd3-4470-9e94-7736e000bc64 class="margin-NaN">contentType</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#241cf5cf-babc-49b1-9de6-ea3d025ad5fd class="margin-NaN">created_time</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ded23226-fb69-4f10-92de-61452576680f class="margin-NaN">encoding</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#777f2407-15ca-4d16-a806-14225cd2bf70 class="margin-NaN">etag</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c773c1ce-3698-48a7-afad-1d8722172c34 class="margin-NaN">fieldname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ed44f796-4f43-4544-a2c1-d3768d4540c1 class="margin-NaN">key</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9f5207cf-3dd0-4fa5-961e-978196183a2f class="margin-NaN">metadata</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#58cc97db-e73e-4b8c-9f0f-e0af713e8ef7 class="margin-NaN">mimetype</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#508884ca-a078-4874-b7bf-9e23b5b80017 class="margin-NaN">originalname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#83dae5b0-7973-45d3-b1bb-4abbd61033ae class="margin-NaN">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2c82de82-049c-4581-aefe-032b73447f9f class="margin-NaN">size</a></td><td class="no-break-word">numeric,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f9f44719-3a7a-48c4-b27c-5597b7cfc7bb class="margin-NaN">storageClass</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2e0ffd1b-e856-4ddb-9878-ff7a9ebc2cf1 class="margin-NaN">versionId</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.195.2 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="6dc205dc-5b8d-4b7c-9b4c-2735d9d25f2d"></a>

###### 2.1.2.4.2.196 Field **location**

###### 2.1.2.4.2.196.1 **location** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>location</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="00b68081-332e-46d7-afd7-94c697cac71a"></a>

###### 2.1.2.4.2.197 Field **acl**

###### 2.1.2.4.2.197.1 **acl** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>acl</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="85e9382e-3ad1-4ef6-b6e9-5d2fdee3d0ed"></a>

###### 2.1.2.4.2.198 Field **bucket**

###### 2.1.2.4.2.198.1 **bucket** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>bucket</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8668d108-b364-45e2-bff7-d087d82cde54"></a>

###### 2.1.2.4.2.199 Field **contentDisposition**

###### 2.1.2.4.2.199.1 **contentDisposition** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentDisposition</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="df2dc48b-bd5d-4615-8ab5-185c88a71d53"></a>

###### 2.1.2.4.2.200 Field **contentEncoding**

###### 2.1.2.4.2.200.1 **contentEncoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentEncoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="84ecf8d8-fdd3-4470-9e94-7736e000bc64"></a>

###### 2.1.2.4.2.201 Field **contentType**

###### 2.1.2.4.2.201.1 **contentType** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentType</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="241cf5cf-babc-49b1-9de6-ea3d025ad5fd"></a>

###### 2.1.2.4.2.202 Field **created\_time**

###### 2.1.2.4.2.202.1 **created\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ded23226-fb69-4f10-92de-61452576680f"></a>

###### 2.1.2.4.2.203 Field **encoding**

###### 2.1.2.4.2.203.1 **encoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>encoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="777f2407-15ca-4d16-a806-14225cd2bf70"></a>

###### 2.1.2.4.2.204 Field **etag**

###### 2.1.2.4.2.204.1 **etag** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>etag</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c773c1ce-3698-48a7-afad-1d8722172c34"></a>

###### 2.1.2.4.2.205 Field **fieldname**

###### 2.1.2.4.2.205.1 **fieldname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ed44f796-4f43-4544-a2c1-d3768d4540c1"></a>

###### 2.1.2.4.2.206 Field **key**

###### 2.1.2.4.2.206.1 **key** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>key</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="9f5207cf-3dd0-4fa5-961e-978196183a2f"></a>

###### 2.1.2.4.2.207 Field **metadata**

###### 2.1.2.4.2.207.1 **metadata** Hierarchy

Parent field: **properties**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#7fbf6001-1fba-49fe-8c81-d991560c2f17 class="margin-NaN">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f1fa0ba4-a6ff-43d9-82b3-18d5605f7a93 class="margin-NaN">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.207.2 **metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="7fbf6001-1fba-49fe-8c81-d991560c2f17"></a>

###### 2.1.2.4.2.208 Field **Content-Type**

###### 2.1.2.4.2.208.1 **Content-Type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Content-Type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="f1fa0ba4-a6ff-43d9-82b3-18d5605f7a93"></a>

###### 2.1.2.4.2.209 Field **fieldName**

###### 2.1.2.4.2.209.1 **fieldName** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldName</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="58cc97db-e73e-4b8c-9f0f-e0af713e8ef7"></a>

###### 2.1.2.4.2.210 Field **mimetype**

###### 2.1.2.4.2.210.1 **mimetype** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mimetype</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="508884ca-a078-4874-b7bf-9e23b5b80017"></a>

###### 2.1.2.4.2.211 Field **originalname**

###### 2.1.2.4.2.211.1 **originalname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>originalname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="83dae5b0-7973-45d3-b1bb-4abbd61033ae"></a>

###### 2.1.2.4.2.212 Field **serverSideEncryption**

###### 2.1.2.4.2.212.1 **serverSideEncryption** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>serverSideEncryption</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="2c82de82-049c-4581-aefe-032b73447f9f"></a>

###### 2.1.2.4.2.213 Field **size**

###### 2.1.2.4.2.213.1 **size** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>size</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="f9f44719-3a7a-48c4-b27c-5597b7cfc7bb"></a>

###### 2.1.2.4.2.214 Field **storageClass**

###### 2.1.2.4.2.214.1 **storageClass** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>storageClass</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="2e0ffd1b-e856-4ddb-9878-ff7a9ebc2cf1"></a>

###### 2.1.2.4.2.215 Field **versionId**

###### 2.1.2.4.2.215.1 **versionId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>versionId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="2b658d3a-25aa-4140-b87b-22d4281fecdc"></a>

###### 2.1.2.4.2.216 Field **promises**

###### 2.1.2.4.2.216.1 **promises** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>promises</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="0a9a7fc4-aa96-473b-8d7e-a691dcaaf15b"></a>

###### 2.1.2.4.2.217 Field **social**

###### 2.1.2.4.2.217.1 **social** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#577e2bdb-f27d-416f-8570-ba1310b9cbd6 class="margin-NaN">instagram</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#de4851fb-b60c-4706-b415-4eba7479b14d class="margin-NaN">messenger</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#34dba23d-f359-495f-adba-db960eb44192 class="margin-NaN">whatsapp</a></td><td class="no-break-word">numeric,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5237c8b2-d0c4-4a6d-b18e-7605db373935 class="margin-NaN">facebook</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.217.2 **social** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>social</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="577e2bdb-f27d-416f-8570-ba1310b9cbd6"></a>

###### 2.1.2.4.2.218 Field **instagram**

###### 2.1.2.4.2.218.1 **instagram** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>instagram</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="de4851fb-b60c-4706-b415-4eba7479b14d"></a>

###### 2.1.2.4.2.219 Field **messenger**

###### 2.1.2.4.2.219.1 **messenger** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>messenger</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="34dba23d-f359-495f-adba-db960eb44192"></a>

###### 2.1.2.4.2.220 Field **whatsapp**

###### 2.1.2.4.2.220.1 **whatsapp** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>whatsapp</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5237c8b2-d0c4-4a6d-b18e-7605db373935"></a>

###### 2.1.2.4.2.221 Field **facebook**

###### 2.1.2.4.2.221.1 **facebook** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>facebook</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="b5cced4b-b372-42dd-a837-c2c8ab5e52e6"></a>

###### 2.1.2.4.2.222 Field **horary**

###### 2.1.2.4.2.222.1 **horary** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#7a7c3d43-266e-4812-892e-a857b9fc0015 class="margin-NaN">init_horary</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#32f350a1-9b9c-4a82-9d86-c7c829e80a36 class="margin-NaN">final_horary</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.222.2 **horary** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>horary</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="7a7c3d43-266e-4812-892e-a857b9fc0015"></a>

###### 2.1.2.4.2.223 Field **init\_horary**

###### 2.1.2.4.2.223.1 **init\_horary** Hierarchy

Parent field: **horary**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#022d2e49-3566-42fc-afa8-ceaf35decda9 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bd834a22-0ad9-44c4-ac3f-21c3f792f297 class="margin-NaN">value</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.223.2 **init\_horary** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>init_horary</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="022d2e49-3566-42fc-afa8-ceaf35decda9"></a>

###### 2.1.2.4.2.224 Field **name**

###### 2.1.2.4.2.224.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>8 a.m.</td></tr></tbody></table>

### <a id="bd834a22-0ad9-44c4-ac3f-21c3f792f297"></a>

###### 2.1.2.4.2.225 Field **value**

###### 2.1.2.4.2.225.1 **value** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>value</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>8</td></tr></tbody></table>

### <a id="32f350a1-9b9c-4a82-9d86-c7c829e80a36"></a>

###### 2.1.2.4.2.226 Field **final\_horary**

###### 2.1.2.4.2.226.1 **final\_horary** Hierarchy

Parent field: **horary**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#b6aad4c5-ad28-45c0-a2eb-8c60f54769c8 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5682f348-d69e-469b-8529-056121f01dce class="margin-NaN">value</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.226.2 **final\_horary** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>final_horary</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="b6aad4c5-ad28-45c0-a2eb-8c60f54769c8"></a>

###### 2.1.2.4.2.227 Field **name**

###### 2.1.2.4.2.227.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6 p.m.</td></tr></tbody></table>

### <a id="5682f348-d69e-469b-8529-056121f01dce"></a>

###### 2.1.2.4.2.228 Field **value**

###### 2.1.2.4.2.228.1 **value** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>value</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>18</td></tr></tbody></table>

### <a id="d07012e7-6097-4a26-a193-80b7f3acc375"></a>

###### 2.1.2.4.2.229 Field **neighborhood**

###### 2.1.2.4.2.229.1 **neighborhood** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>neighborhood</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>cumbres</td></tr></tbody></table>

### <a id="eae2c42d-c1a3-4fec-a106-034bb25bc62c"></a>

###### 2.1.2.4.2.230 Field **location**

###### 2.1.2.4.2.230.1 **location** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#ffa247e1-cac3-4c5e-8019-711a4b043e37 class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.230.2 **location** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>location</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (document,null,string)</td></tr><tr><td></td><td>[object Object],[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ffa247e1-cac3-4c5e-8019-711a4b043e37"></a>

###### 2.1.2.4.2.231 Field **properties**

###### 2.1.2.4.2.231.1 **properties** Hierarchy

Parent field: **location**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#e024dbd4-8155-4672-bcfc-057ee45871a9 class="margin-NaN">lat</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#88e053fb-f2ed-4925-beb2-15f85e9fcd8a class="margin-NaN">lng</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.231.2 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="e024dbd4-8155-4672-bcfc-057ee45871a9"></a>

###### 2.1.2.4.2.232 Field **lat**

###### 2.1.2.4.2.232.1 **lat** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>lat</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="88e053fb-f2ed-4925-beb2-15f85e9fcd8a"></a>

###### 2.1.2.4.2.233 Field **lng**

###### 2.1.2.4.2.233.1 **lng** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>lng</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="e3d7dd9d-6ec9-436f-9232-524a60161021"></a>

###### 2.1.2.4.2.234 Field **tel**

###### 2.1.2.4.2.234.1 **tel** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>tel</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="49bd41a3-a3e4-4b2f-a591-138e4ca74dc5"></a>

###### 2.1.2.4.2.235 Field **payments**

###### 2.1.2.4.2.235.1 **payments** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#b481c030-9227-411a-bb72-f6be0d09c148 class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.235.2 **payments** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>payments</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (document,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="b481c030-9227-411a-bb72-f6be0d09c148"></a>

###### 2.1.2.4.2.236 Field **properties**

###### 2.1.2.4.2.236.1 **properties** Hierarchy

Parent field: **payments**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#5711aed3-e84b-4990-adef-92fd3266736c class="margin-NaN">pse</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#48840bf1-f05d-4c43-99bc-bfbd8f4d9c8c class="margin-NaN">card</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#eb9c8e3b-739c-4b75-ba33-f732b8fba573 class="margin-NaN">cod</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#73ed4084-a56b-4c61-87fe-38d1cbc9264b class="margin-NaN">bancolombia_collect</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a5badfdc-6b0f-420f-8c20-b73ec791f60a class="margin-NaN">bancolombia_qr</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f95d4e6a-49a2-4256-8a8e-326f1dbed987 class="margin-NaN">bancolombia_transfer</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4ba0dd38-0b32-439e-9de0-1e13dca98420 class="margin-NaN">nequi</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.236.2 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="5711aed3-e84b-4990-adef-92fd3266736c"></a>

###### 2.1.2.4.2.237 Field **pse**

###### 2.1.2.4.2.237.1 **pse** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>pse</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="48840bf1-f05d-4c43-99bc-bfbd8f4d9c8c"></a>

###### 2.1.2.4.2.238 Field **card**

###### 2.1.2.4.2.238.1 **card** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>card</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="eb9c8e3b-739c-4b75-ba33-f732b8fba573"></a>

###### 2.1.2.4.2.239 Field **cod**

###### 2.1.2.4.2.239.1 **cod** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cod</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="73ed4084-a56b-4c61-87fe-38d1cbc9264b"></a>

###### 2.1.2.4.2.240 Field **bancolombia\_collect**

###### 2.1.2.4.2.240.1 **bancolombia\_collect** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>bancolombia_collect</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a5badfdc-6b0f-420f-8c20-b73ec791f60a"></a>

###### 2.1.2.4.2.241 Field **bancolombia\_qr**

###### 2.1.2.4.2.241.1 **bancolombia\_qr** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>bancolombia_qr</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="f95d4e6a-49a2-4256-8a8e-326f1dbed987"></a>

###### 2.1.2.4.2.242 Field **bancolombia\_transfer**

###### 2.1.2.4.2.242.1 **bancolombia\_transfer** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>bancolombia_transfer</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4ba0dd38-0b32-439e-9de0-1e13dca98420"></a>

###### 2.1.2.4.2.243 Field **nequi**

###### 2.1.2.4.2.243.1 **nequi** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>nequi</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="2ca7fb7d-789c-484c-85b9-9c4cff5f2055"></a>

###### 2.1.2.4.2.244 Field **principal\_address**

###### 2.1.2.4.2.244.1 **principal\_address** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>principal_address</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>64a9f75ab97bf8bfaf92854b</td></tr></tbody></table>

### <a id="fff19708-f19e-4268-984e-f4efb922d5d8"></a>

###### 2.1.2.4.2.245 Field **carry**

###### 2.1.2.4.2.245.1 **carry** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>carry</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="664f931c-2fe7-46ae-bc20-20d21a9adf96"></a>

###### 2.1.2.4.2.246 Field **geolocation**

###### 2.1.2.4.2.246.1 **geolocation** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#4047ec66-06b0-4877-8fb7-f7ef689defc5 class="margin-NaN">lat</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7dad6b71-d872-4284-92a6-3bf4ebfab00c class="margin-NaN">lng</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.246.2 **geolocation** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>geolocation</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="4047ec66-06b0-4877-8fb7-f7ef689defc5"></a>

###### 2.1.2.4.2.247 Field **lat**

###### 2.1.2.4.2.247.1 **lat** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>lat</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="7dad6b71-d872-4284-92a6-3bf4ebfab00c"></a>

###### 2.1.2.4.2.248 Field **lng**

###### 2.1.2.4.2.248.1 **lng** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>lng</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ab2ae1fa-334f-4bb3-8f60-353b9ffbf0e2"></a>

###### 2.1.2.4.2.249 Field **default**

###### 2.1.2.4.2.249.1 **default** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>default</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="368ed2fd-0df8-4ce0-a1f5-bdf14f20dfb4"></a>

###### 2.1.2.4.2.250 Field **gtag**

###### 2.1.2.4.2.250.1 **gtag** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>gtag</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="25529cf4-1e9d-49de-a16d-a128d56beaa5"></a>

###### 2.1.2.4.2.251 Field **indicative**

###### 2.1.2.4.2.251.1 **indicative** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>indicative</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>57</td></tr></tbody></table>

### <a id="8408f5f2-e892-488d-ab06-41e8194cc0e8"></a>

###### 2.1.2.4.2.252 Field **pixel**

###### 2.1.2.4.2.252.1 **pixel** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>pixel</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="47fa6237-2ab0-42c4-9a0c-690c12297ffc"></a>

###### 2.1.2.4.2.253 Field **rem**

###### 2.1.2.4.2.253.1 **rem** Hierarchy

Parent field: **data**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#ae995f7f-4690-4f1d-8c50-e65096e817ad class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#083681c9-f705-4754-9747-7f33575d2ef1 class="margin-NaN">last_name</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#181ce998-4e59-4054-b150-926265aeb8b6 class="margin-NaN">tel</a></td><td class="no-break-word">numeric,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.253.2 **rem** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>rem</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="ae995f7f-4690-4f1d-8c50-e65096e817ad"></a>

###### 2.1.2.4.2.254 Field **name**

###### 2.1.2.4.2.254.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Julian</td></tr></tbody></table>

### <a id="083681c9-f705-4754-9747-7f33575d2ef1"></a>

###### 2.1.2.4.2.255 Field **last\_name**

###### 2.1.2.4.2.255.1 **last\_name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>last_name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Ramirez Velez</td></tr></tbody></table>

### <a id="181ce998-4e59-4054-b150-926265aeb8b6"></a>

###### 2.1.2.4.2.256 Field **tel**

###### 2.1.2.4.2.256.1 **tel** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>tel</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="de4db032-096a-430d-9348-3949db3d0221"></a>

###### 2.1.2.4.2.257 Field **statistics**

###### 2.1.2.4.2.257.1 **statistics** Hierarchy

Parent field: **warehouse**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#d07aa858-0ecb-452c-8329-3880e1d46f4e class="margin-NaN">sales</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#91bacde1-b8ba-4277-ac34-1292d224161e class="margin-NaN">imports</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.257.2 **statistics** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>statistics</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="d07aa858-0ecb-452c-8329-3880e1d46f4e"></a>

###### 2.1.2.4.2.258 Field **sales**

###### 2.1.2.4.2.258.1 **sales** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>sales</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="91bacde1-b8ba-4277-ac34-1292d224161e"></a>

###### 2.1.2.4.2.259 Field **imports**

###### 2.1.2.4.2.259.1 **imports** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>imports</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>704</td></tr></tbody></table>

### <a id="76982eaa-d18c-47dd-a243-c6efe67eb068"></a>

###### 2.1.2.4.2.260 Field **father\_id**

###### 2.1.2.4.2.260.1 **father\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>father_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6575dda966023d9e107e420e</td></tr></tbody></table>

### <a id="d534c787-307d-4f46-b09e-2b7eaca551fa"></a>

###### 2.1.2.4.2.261 Field **shared\_id**

###### 2.1.2.4.2.261.1 **shared\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shared_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6575ddab66023d9e107e4264</td></tr></tbody></table>

### <a id="74fb6938-13c1-439a-8fd7-f3aa8c11f5ae"></a>

###### 2.1.2.4.2.262 Field **suggestions**

###### 2.1.2.4.2.262.1 **suggestions** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>suggestions</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4afa0df0-896e-43ba-9945-7b33f77b2897"></a>

###### 2.1.2.4.2.263 Field **warranty**

###### 2.1.2.4.2.263.1 **warranty** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>warranty</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4b7773b2-3d77-4f03-bcdb-dedd3e7902ad"></a>

###### 2.1.2.4.2.264 Field **disabled\_by\_inactivity**

###### 2.1.2.4.2.264.1 **disabled\_by\_inactivity** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>disabled_by_inactivity</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="e02a5f63-6aac-4957-8613-6355ec2d4c89"></a>

###### 2.1.2.4.2.265 Field **total\_inventory**

###### 2.1.2.4.2.265.1 **total\_inventory** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>total_inventory</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>900</td></tr></tbody></table>

### <a id="c94bce45-3ff3-434f-ba8f-799d686d78a3"></a>

###### 2.1.2.4.2.266 Field **category**

###### 2.1.2.4.2.266.1 **category** Hierarchy

Parent field: **wearehouse\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#e15e6ba6-5b5d-4186-8dda-e53a6febad96 class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.266.2 **category** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>category</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (document,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="e15e6ba6-5b5d-4186-8dda-e53a6febad96"></a>

###### 2.1.2.4.2.267 Field **properties**

###### 2.1.2.4.2.267.1 **properties** Hierarchy

Parent field: **category**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#5f3e625f-01f8-4918-ab39-b126e9258012 class="margin-NaN">_id</a></td><td class="no-break-word">string,objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#961ae830-0464-4e0c-ba9f-98964443e060 class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2a854d38-8abd-4958-a841-9af679b109a8 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6a4c54d9-4f5c-41f4-9fc8-dab09627c672 class="margin-NaN">category_father</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#af3a0336-4795-4a67-b57b-28b1cd1eda9a class="margin-NaN">path_from_root</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#859c5cf2-8007-49c2-8fba-0a7a68c964f4 class="margin-NaN">children_categories</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cc583a06-9b0a-4b28-ad26-737fc6a514f0 class="margin-NaN">settings</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8128146f-807d-4490-b512-cec7382bc11b class="margin-NaN">country</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2ec8180a-efbd-443c-b516-d8a44b989cdf class="margin-NaN">date_created</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c19aea5e-3922-48dd-8361-3d52d94cac3b class="margin-NaN">permalink</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#403fdafd-7aae-4d35-8acb-739e4575237a class="margin-NaN">picture</a></td><td class="no-break-word">null,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.267.2 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="5f3e625f-01f8-4918-ab39-b126e9258012"></a>

###### 2.1.2.4.2.268 Field **\_id**

###### 2.1.2.4.2.268.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,objectId)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="961ae830-0464-4e0c-ba9f-98964443e060"></a>

###### 2.1.2.4.2.269 Field **id**

###### 2.1.2.4.2.269.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="2a854d38-8abd-4958-a841-9af679b109a8"></a>

###### 2.1.2.4.2.270 Field **name**

###### 2.1.2.4.2.270.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="6a4c54d9-4f5c-41f4-9fc8-dab09627c672"></a>

###### 2.1.2.4.2.271 Field **category\_father**

###### 2.1.2.4.2.271.1 **category\_father** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>category_father</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="af3a0336-4795-4a67-b57b-28b1cd1eda9a"></a>

###### 2.1.2.4.2.272 Field **path\_from\_root**

###### 2.1.2.4.2.272.1 **path\_from\_root** Hierarchy

Parent field: **properties**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#042e4681-94ad-41fc-afdc-bf1dc3de3026 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.272.2 **path\_from\_root** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>path_from_root</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="042e4681-94ad-41fc-afdc-bf1dc3de3026"></a>

###### 2.1.2.4.2.273 Field **\[0\]**

###### 2.1.2.4.2.273.1 **\[0\]** Hierarchy

Parent field: **path\_from\_root**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#97de3524-a747-41c7-a339-2b888f041992 class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7bd25ae4-4f6c-4b55-ad9c-49c20d9a8053 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.273.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="97de3524-a747-41c7-a339-2b888f041992"></a>

###### 2.1.2.4.2.274 Field **id**

###### 2.1.2.4.2.274.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="7bd25ae4-4f6c-4b55-ad9c-49c20d9a8053"></a>

###### 2.1.2.4.2.275 Field **name**

###### 2.1.2.4.2.275.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="859c5cf2-8007-49c2-8fba-0a7a68c964f4"></a>

###### 2.1.2.4.2.276 Field **children\_categories**

###### 2.1.2.4.2.276.1 **children\_categories** Hierarchy

Parent field: **properties**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#01254cd8-6f93-40fc-874f-953ff1c728ef class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.276.2 **children\_categories** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>children_categories</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="01254cd8-6f93-40fc-874f-953ff1c728ef"></a>

###### 2.1.2.4.2.277 Field **\[0\]**

###### 2.1.2.4.2.277.1 **\[0\]** Hierarchy

Parent field: **children\_categories**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#a6a3ea19-c744-4704-90df-ff1365581ce7 class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#946fc241-01d7-4260-a7da-7276d452cc00 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.277.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="a6a3ea19-c744-4704-90df-ff1365581ce7"></a>

###### 2.1.2.4.2.278 Field **id**

###### 2.1.2.4.2.278.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="946fc241-01d7-4260-a7da-7276d452cc00"></a>

###### 2.1.2.4.2.279 Field **name**

###### 2.1.2.4.2.279.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="cc583a06-9b0a-4b28-ad26-737fc6a514f0"></a>

###### 2.1.2.4.2.280 Field **settings**

###### 2.1.2.4.2.280.1 **settings** Hierarchy

Parent field: **properties**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#1246458f-ff5c-47e0-bba6-ed52fcc463f9 class="margin-NaN">adult_content</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#23ec97a5-48fc-44c6-b19f-ffe64a6326e7 class="margin-NaN">fragile</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3e8418be-3707-411e-9b25-f47393f0d335 class="margin-NaN">currencies</a></td><td class="no-break-word">array</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6ca30205-cbfa-4613-a6be-5eca2642cea9 class="margin-NaN">inmediate_payment</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5f2752a1-59c9-4279-8c05-c4cd1b7aa94f class="margin-NaN">items_review_allowed</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0f09a277-14ff-4422-a166-55a6fb1baf71 class="margin-NaN">listing_allowed</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bc4efc4c-a1c6-4942-8d13-af34f15bd54d class="margin-NaN">max_description_length</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#afbfba1c-136d-44bb-8519-8270210b735d class="margin-NaN">max_pictures_per_item</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c6f3ce21-e7d4-4229-8909-1cdb16558aff class="margin-NaN">max_pictures_per_item_var</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bd485a11-0755-441e-abf0-fde36133ec9b class="margin-NaN">max_sub_title_length</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#441aa472-3bfb-4477-a93c-d90de521be28 class="margin-NaN">max_title_length</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#db60fcac-26b4-4d59-abc4-6d8bca0f44bc class="margin-NaN">maximum_price</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2398b183-3bd2-45ab-b885-cc56b81d6733 class="margin-NaN">maximum_price_currency</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9940d20e-0f2e-4359-b26a-a1f3331e4fae class="margin-NaN">minimum_price</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#38614ed2-53fa-47d3-8c06-590511225f58 class="margin-NaN">minimum_price_currency</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5f7bec98-fc01-4c43-aacc-bec5b0ba4442 class="margin-NaN">sat_product_code_mexico</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d86a93b3-d0fc-4104-b5e4-016ae7cf6b59 class="margin-NaN">sat_product_description_mexico</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8495f827-3b2e-4731-a90e-13053806a487 class="margin-NaN">seller_contact</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8e70ca9d-2674-446a-b25f-28d427a175bc class="margin-NaN">status</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.280.2 **settings** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>settings</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="1246458f-ff5c-47e0-bba6-ed52fcc463f9"></a>

###### 2.1.2.4.2.281 Field **adult\_content**

###### 2.1.2.4.2.281.1 **adult\_content** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>adult_content</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="23ec97a5-48fc-44c6-b19f-ffe64a6326e7"></a>

###### 2.1.2.4.2.282 Field **fragile**

###### 2.1.2.4.2.282.1 **fragile** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fragile</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="3e8418be-3707-411e-9b25-f47393f0d335"></a>

###### 2.1.2.4.2.283 Field **currencies**

###### 2.1.2.4.2.283.1 **currencies** Hierarchy

Parent field: **settings**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#f021a06e-2337-427d-aaad-7bb8599ba289 class="margin-NaN">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.283.2 **currencies** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>currencies</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="f021a06e-2337-427d-aaad-7bb8599ba289"></a>

###### 2.1.2.4.2.284 Field **\[0\]**

###### 2.1.2.4.2.284.1 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr></tbody></table>

### <a id="6ca30205-cbfa-4613-a6be-5eca2642cea9"></a>

###### 2.1.2.4.2.285 Field **inmediate\_payment**

###### 2.1.2.4.2.285.1 **inmediate\_payment** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>inmediate_payment</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5f2752a1-59c9-4279-8c05-c4cd1b7aa94f"></a>

###### 2.1.2.4.2.286 Field **items\_review\_allowed**

###### 2.1.2.4.2.286.1 **items\_review\_allowed** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>items_review_allowed</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="0f09a277-14ff-4422-a166-55a6fb1baf71"></a>

###### 2.1.2.4.2.287 Field **listing\_allowed**

###### 2.1.2.4.2.287.1 **listing\_allowed** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>listing_allowed</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="bc4efc4c-a1c6-4942-8d13-af34f15bd54d"></a>

###### 2.1.2.4.2.288 Field **max\_description\_length**

###### 2.1.2.4.2.288.1 **max\_description\_length** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>max_description_length</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="afbfba1c-136d-44bb-8519-8270210b735d"></a>

###### 2.1.2.4.2.289 Field **max\_pictures\_per\_item**

###### 2.1.2.4.2.289.1 **max\_pictures\_per\_item** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>max_pictures_per_item</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c6f3ce21-e7d4-4229-8909-1cdb16558aff"></a>

###### 2.1.2.4.2.290 Field **max\_pictures\_per\_item\_var**

###### 2.1.2.4.2.290.1 **max\_pictures\_per\_item\_var** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>max_pictures_per_item_var</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="bd485a11-0755-441e-abf0-fde36133ec9b"></a>

###### 2.1.2.4.2.291 Field **max\_sub\_title\_length**

###### 2.1.2.4.2.291.1 **max\_sub\_title\_length** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>max_sub_title_length</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="441aa472-3bfb-4477-a93c-d90de521be28"></a>

###### 2.1.2.4.2.292 Field **max\_title\_length**

###### 2.1.2.4.2.292.1 **max\_title\_length** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>max_title_length</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="db60fcac-26b4-4d59-abc4-6d8bca0f44bc"></a>

###### 2.1.2.4.2.293 Field **maximum\_price**

###### 2.1.2.4.2.293.1 **maximum\_price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>maximum_price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="2398b183-3bd2-45ab-b885-cc56b81d6733"></a>

###### 2.1.2.4.2.294 Field **maximum\_price\_currency**

###### 2.1.2.4.2.294.1 **maximum\_price\_currency** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>maximum_price_currency</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="9940d20e-0f2e-4359-b26a-a1f3331e4fae"></a>

###### 2.1.2.4.2.295 Field **minimum\_price**

###### 2.1.2.4.2.295.1 **minimum\_price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>minimum_price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="38614ed2-53fa-47d3-8c06-590511225f58"></a>

###### 2.1.2.4.2.296 Field **minimum\_price\_currency**

###### 2.1.2.4.2.296.1 **minimum\_price\_currency** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>minimum_price_currency</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5f7bec98-fc01-4c43-aacc-bec5b0ba4442"></a>

###### 2.1.2.4.2.297 Field **sat\_product\_code\_mexico**

###### 2.1.2.4.2.297.1 **sat\_product\_code\_mexico** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>sat_product_code_mexico</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="d86a93b3-d0fc-4104-b5e4-016ae7cf6b59"></a>

###### 2.1.2.4.2.298 Field **sat\_product\_description\_mexico**

###### 2.1.2.4.2.298.1 **sat\_product\_description\_mexico** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>sat_product_description_mexico</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8495f827-3b2e-4731-a90e-13053806a487"></a>

###### 2.1.2.4.2.299 Field **seller\_contact**

###### 2.1.2.4.2.299.1 **seller\_contact** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>seller_contact</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8e70ca9d-2674-446a-b25f-28d427a175bc"></a>

###### 2.1.2.4.2.300 Field **status**

###### 2.1.2.4.2.300.1 **status** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>status</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8128146f-807d-4490-b512-cec7382bc11b"></a>

###### 2.1.2.4.2.301 Field **country**

###### 2.1.2.4.2.301.1 **country** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="2ec8180a-efbd-443c-b516-d8a44b989cdf"></a>

###### 2.1.2.4.2.302 Field **date\_created**

###### 2.1.2.4.2.302.1 **date\_created** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>date_created</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c19aea5e-3922-48dd-8361-3d52d94cac3b"></a>

###### 2.1.2.4.2.303 Field **permalink**

###### 2.1.2.4.2.303.1 **permalink** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>permalink</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="403fdafd-7aae-4d35-8acb-739e4575237a"></a>

###### 2.1.2.4.2.304 Field **picture**

###### 2.1.2.4.2.304.1 **picture** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>picture</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5c14173d-c5d1-4037-bb6e-a8bdbd8c219f"></a>

###### 2.1.2.4.2.305 Field **country\_ref**

###### 2.1.2.4.2.305.1 **country\_ref** Hierarchy

Parent field: **wearehouse\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#17eb216d-e21e-44ba-add8-d0ceaadd1ccf class="margin-NaN">_id</a></td><td class="no-break-word">objectId,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3619e6ac-a785-41a5-93ec-569240826f3c class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f21e27d1-e3f2-4ae4-bb41-6f75239ad5b3 class="margin-NaN">iso2</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d59b9c4b-bf17-4213-990e-f0bf5e7bf96a class="margin-NaN">iso3</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e8bd220f-59d2-4251-9bd7-7678993f6b82 class="margin-NaN">flag_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#07975898-638d-498a-80cd-84888d87fb12 class="margin-NaN">phone_code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.305.2 **country\_ref** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country_ref</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="17eb216d-e21e-44ba-add8-d0ceaadd1ccf"></a>

###### 2.1.2.4.2.306 Field **\_id**

###### 2.1.2.4.2.306.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (objectId,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="3619e6ac-a785-41a5-93ec-569240826f3c"></a>

###### 2.1.2.4.2.307 Field **name**

###### 2.1.2.4.2.307.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Colombia</td></tr></tbody></table>

### <a id="f21e27d1-e3f2-4ae4-bb41-6f75239ad5b3"></a>

###### 2.1.2.4.2.308 Field **iso2**

###### 2.1.2.4.2.308.1 **iso2** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>iso2</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>CO</td></tr></tbody></table>

### <a id="d59b9c4b-bf17-4213-990e-f0bf5e7bf96a"></a>

###### 2.1.2.4.2.309 Field **iso3**

###### 2.1.2.4.2.309.1 **iso3** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>iso3</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>COL</td></tr></tbody></table>

### <a id="e8bd220f-59d2-4251-9bd7-7678993f6b82"></a>

###### 2.1.2.4.2.310 Field **flag\_url**

###### 2.1.2.4.2.310.1 **flag\_url** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>flag_url</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://www.geonames.org/flags/x/co.gif</td></tr></tbody></table>

### <a id="07975898-638d-498a-80cd-84888d87fb12"></a>

###### 2.1.2.4.2.311 Field **phone\_code**

###### 2.1.2.4.2.311.1 **phone\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>phone_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>57</td></tr></tbody></table>

### <a id="757464b8-643f-43f3-b296-63fb542b4e40"></a>

###### 2.1.2.4.2.312 Field **featured**

###### 2.1.2.4.2.312.1 **featured** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>featured</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="f65461d3-42b2-4caa-94e2-3e8bbbda9288"></a>

###### 2.1.2.4.2.313 Field **shared\_metadata**

###### 2.1.2.4.2.313.1 **shared\_metadata** Hierarchy

Parent field: **wearehouse\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#0693bc10-2926-48ca-add4-96c5554bf350 class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.313.2 **shared\_metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shared_metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (document,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="0693bc10-2926-48ca-add4-96c5554bf350"></a>

###### 2.1.2.4.2.314 Field **properties**

###### 2.1.2.4.2.314.1 **properties** Hierarchy

Parent field: **shared\_metadata**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#d831edad-5fb6-488a-bbcc-50be26f95f40 class="margin-NaN">shared_with</a></td><td class="no-break-word">null,array</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.314.2 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="d831edad-5fb6-488a-bbcc-50be26f95f40"></a>

###### 2.1.2.4.2.315 Field **shared\_with**

###### 2.1.2.4.2.315.1 **shared\_with** Hierarchy

Parent field: **properties**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#47fb169c-5f21-44b3-9be6-941ebd0e98a4 class="margin-NaN">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.315.2 **shared\_with** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shared_with</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,array)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="47fb169c-5f21-44b3-9be6-941ebd0e98a4"></a>

###### 2.1.2.4.2.316 Field **items**

###### 2.1.2.4.2.316.1 **items** Hierarchy

Parent field: **shared\_with**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#38f5c5b9-42e8-436f-b8ca-63dfc2fed6ce class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.316.2 **items** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="38f5c5b9-42e8-436f-b8ca-63dfc2fed6ce"></a>

###### 2.1.2.4.2.317 Field **\[0\]**

###### 2.1.2.4.2.317.1 **\[0\]** Hierarchy

Parent field: **items**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#9da97876-700e-4f5b-9772-697b127e4c11 class="margin-NaN">label</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#978d06c2-5ede-47eb-aac6-f3d0b272b2e9 class="margin-NaN">value</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.317.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="9da97876-700e-4f5b-9772-697b127e4c11"></a>

###### 2.1.2.4.2.318 Field **label**

###### 2.1.2.4.2.318.1 **label** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>label</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="978d06c2-5ede-47eb-aac6-f3d0b272b2e9"></a>

###### 2.1.2.4.2.319 Field **value**

###### 2.1.2.4.2.319.1 **value** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>value</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="d336bb50-52a3-4e65-b92b-c711e644377d"></a>

###### 2.1.2.4.2.320 Field **shop\_out**

###### 2.1.2.4.2.320.1 **shop\_out** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shop_out</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="33fecb1d-d431-48a5-bddc-fc5bc09d308e"></a>

###### 2.1.2.4.2.321 Field **vivible**

###### 2.1.2.4.2.321.1 **vivible** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>vivible</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="5c9f0e25-a29b-4627-8b6c-237402add3d1"></a>

###### 2.1.2.4.2.322 Field **vusible**

###### 2.1.2.4.2.322.1 **vusible** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>vusible</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="81d51b83-9544-48df-8d41-880fa1f22224"></a>

###### 2.1.2.4.2.323 Field **warranty\_description**

###### 2.1.2.4.2.323.1 **warranty\_description** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>warranty_description</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

###### 2.1.2.4.3 **wearehouse\_products** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">warehouse.statistics.imports_-1</td><td class="table-column-property">visible_1_warehouse.data.only_my_stores_1_warehouse.statistics.imports_-1</td><td class="table-column-property">variations.variation_id_1</td><td class="table-column-property">warehouse.data.db_seller_1</td><td class="table-column-property">shared_metadata_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">warehouse.statistics.imports_-1</td><td class="table-column-indexes">visible_1_warehouse.data.only_my_stores_1_warehouse.statistics.imports_-1</td><td class="table-column-indexes">variations.variation_id_1</td><td class="table-column-indexes">warehouse.data.db_seller_1</td><td class="table-column-indexes">shared_metadata_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">imports('descending')</td><td class="table-column-indexes">undefined('ascending'), only_my_stores('ascending'), imports('descending')</td><td class="table-column-indexes">variation_id('ascending')</td><td class="table-column-indexes">db_seller('ascending')</td><td class="table-column-indexes">undefined('descending')</td></tr></tbody></table>

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">shared_metadata.shared_with_-1</td><td class="table-column-property">_id_</td><td class="table-column-property">name_-1</td><td class="table-column-property">visible_-1_warehouse.data.only_my_stores_-1_category.path_from_root.id_-1</td><td class="table-column-property">category._id_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">shared_metadata.shared_with_-1</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">name_-1</td><td class="table-column-indexes">visible_-1_warehouse.data.only_my_stores_-1_category.path_from_root.id_-1</td><td class="table-column-indexes">category._id_-1</td></tr><tr><td>Key</td><td class="table-column-indexes"></td><td class="table-column-indexes">undefined('ascending')</td><td class="table-column-indexes">undefined('descending')</td><td class="table-column-indexes">undefined('descending'), only_my_stores('descending')</td><td class="table-column-indexes"></td></tr></tbody></table>

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">visible_-1_warehouse.data.only_my_stores_-1_shared_metadata.shared_with.value_-1</td><td class="table-column-property">visible_-1_warehouse.data.only_my_stores_-1_shared_metadata_-1_shared_metadata.shared_with_-1_shared_metadata.shared_with.value_-1</td><td class="table-column-property">country_ref.iso3_1</td><td class="table-column-property">warehouse.father_id_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">visible_-1_warehouse.data.only_my_stores_-1_shared_metadata.shared_with.value_-1</td><td class="table-column-indexes">visible_-1_warehouse.data.only_my_stores_-1_shared_metadata_-1_shared_metadata.shared_with_-1_shared_metadata.shared_with.value_-1</td><td class="table-column-indexes">country_ref.iso3_1</td><td class="table-column-indexes">warehouse.father_id_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">undefined('descending'), only_my_stores('descending')</td><td class="table-column-indexes">undefined('descending'), only_my_stores('descending'), undefined('descending')</td><td class="table-column-indexes">iso3('ascending')</td><td class="table-column-indexes">father_id('descending')</td></tr></tbody></table>

### <a id="ec559fb7-4dbc-4d80-912e-a1628c5130b4"></a>

##### 2.1.2.5 Collection **customers**

###### 2.1.2.5.1 **customers** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>customers</td></tr><tr><td>Technical name</td><td>Tiendas1</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Description</td><td><div class="docs-markdown"><p>En esta colección se almacenan todos los registros de las tiendas registradas en la plataforma. Cada tienda posee un campo único denominado dbname, el cual se encarga de vincular los datos de la tienda con el resto de los recursos relacionados (órdenes, productos, billetera, etc.) a través del campo establishment_identifier. De esta forma, se garantiza la consistencia y la trazabilidad de la información en todo el sistema.</p></div></td></tr><tr><td>Database</td><td><a href=#6f94401a-8e31-4b31-9268-15061668a1b5><span class="name-container">rocketfy</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.5.2 **customers** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#33c75581-9fb5-4487-9520-bd2807d98f16 class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#945af247-d1cd-4c8a-a17f-f78a089e09f0 class="margin-0">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1cdda6a4-13f0-4561-8d0c-8e1362952f0c class="margin-0">email</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ff1ac9f3-9860-4fdd-8d06-a9ee97e41c72 class="margin-0">phone</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ec545f50-b52c-4fc8-8f0c-e45cf2821b0b class="margin-0">metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8e2eee8f-8423-4ae9-b7f9-fbced594a464 class="margin-5">accept_time</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#19e151d2-da67-4f86-87de-658a15aa3c35 class="margin-5">hostname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8c7eff37-0ec3-4b52-b804-7e1e6015b5c2 class="margin-5">platform</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2d022b7c-5ef1-413e-95f3-c30b06b1d74c class="margin-5">networkInterfaces</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bfd4ad06-55b2-4d80-84fe-967739a922ee class="margin-10">Ethernet</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7c2752ee-5a66-4e89-b79b-fc90e369e61f class="margin-15">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#73d42ea6-3e7a-4d5c-b368-73e02e3f886b class="margin-20">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f653a6b6-dd75-49c0-9099-d95ef2b35d3a class="margin-20">netmask</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c9cd12d7-bb85-4326-beae-a8c3ec273edc class="margin-20">family</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#67eb8694-239b-4c10-bd9e-f86d6911ea15 class="margin-20">mac</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0ca1c6c3-f21f-411d-b73c-90ced6aaa3c9 class="margin-20">internal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5e4abeff-cb63-4f7b-b636-5b74bfacc3cd class="margin-20">cidr</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f94199f3-376d-4dd1-b836-41a4ac8044f6 class="margin-20">scopeid</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2f46c2a7-836c-4344-836c-ee185ba5d24d class="margin-10">Wi-Fi</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#874edb61-9142-4dd7-bd21-a4c42915b672 class="margin-15">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f981b30b-5a4c-4652-a010-82e5299d169c class="margin-20">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dc10c421-5451-4765-af43-87e3561d40d1 class="margin-20">netmask</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b8e6d40f-4071-4c2d-8683-2f2fe454042d class="margin-20">family</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#02176330-400c-4c81-91aa-a200c2f45053 class="margin-20">mac</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a8959a1c-0847-4360-88bf-6dacea970813 class="margin-20">internal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0e5fac72-8cf6-4a12-a1b5-8f29c0a113b5 class="margin-20">cidr</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0055072d-3686-4d9c-a550-544491524736 class="margin-20">scopeid</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0f266d97-f930-49ca-8fe4-83e34b26897b class="margin-10">Loopback&nbsp;Pseudo-Interface&nbsp;1</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7df5dd6f-6e6e-4ef4-8d67-3e44a28c5e07 class="margin-15">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a319e91a-aced-4c15-a0c2-9609ec50e81e class="margin-20">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7046af0e-2f87-462d-ab7a-fff9114c3cad class="margin-20">netmask</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a4bdc91e-81ee-4958-bb8e-a20e26cb7e37 class="margin-20">family</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8bd581e6-89a0-4e57-8206-019f3e5ec694 class="margin-20">mac</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6402156b-3964-4b1a-aa9c-dfb07c70586b class="margin-20">internal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0a250e92-bbab-4715-ad9b-3969dcd299b7 class="margin-20">cidr</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#30ccbedd-8879-47d7-8d71-6f8fa1d80d4b class="margin-20">scopeid</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8cc53076-f4d0-4736-88b6-1b3513ad62f0 class="margin-5">from</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ae56d219-435c-4424-b2dd-82747b7c94cb class="margin-0">pageId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7fa9b648-96f2-4145-b5c0-11a173cd0b0e class="margin-0">dbname</a></td><td class="no-break-word">string</td><td>true</td><td>dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0ea96ddc-c9be-4494-bfff-540a55723c04 class="margin-0">plan</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3c6f0b20-5f47-43c6-914a-434161a50cf9 class="margin-0">country</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f345e444-7955-4564-9d49-9b08ac38c77a class="margin-0">test</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#54a6d97f-ff02-4aba-9f0c-35490dd449c3 class="margin-0">actived</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0d9dd937-3454-4ca8-9aa9-f7d1fd784358 class="margin-0">exp</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d5fe7c4b-1bfa-4b85-8972-5c6fde74d367 class="margin-0">created_time</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9e8a4ab0-4243-446a-b5c3-fc4238639306 class="margin-0">created_date</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#91c4826a-ef5b-406d-8cee-5e0392af76c7 class="margin-5">dateFormat</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cd5cea5c-91ee-46de-a6ef-56e214bd0efb class="margin-5">hourFormat</a></td><td class="no-break-word">time</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1800b1fe-dec0-4c4f-a323-fd2f81c74467 class="margin-5">toDate</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c30f0611-6534-4cd1-be32-246ed5195239 class="margin-0">host_asterisk</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#01803ffb-8fec-40af-9447-bcf8a629ff3b class="margin-0">user_asterisk</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fcaeadba-6fee-4b4d-9760-bba6674c722e class="margin-0">pass_asterisk</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0de8637d-9cc9-4750-997f-502e5318e6a0 class="margin-0">visible</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#646c2174-4f2b-4c72-b0ad-703ca4e1b38d class="margin-0">slug</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4067dba8-364a-4119-b154-61bed239fb48 class="margin-0">sender</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3a783962-191e-4c6b-80b7-eaaa2e33ac94 class="margin-5">date</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1f3b6a1a-3f25-4bc9-97d0-76a4d31a1430 class="margin-5">shippings_count</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4c6d80c1-eb3a-4ba1-bc41-c5030f79dc15 class="margin-0">updated_date</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a18d20bb-0a47-4ac6-bc2a-7ec5238f2a1b class="margin-5">created_sender</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9a7aed9d-9833-4314-84d9-f7f5f4749b32 class="margin-0">cohortMigrated3</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8290f3b9-e51e-4231-811c-6a68d24c00ec class="margin-0">blocked_balance</a></td><td class="no-break-word">double</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c005368e-01ab-4bf7-8b26-ce8e34f65d17 class="margin-0">rocketfy_leads</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#87df5c04-95f7-4c08-a2ef-48e1a328af54 class="margin-0">rocketfy_shipping</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c5cf1b4e-6a08-4e5e-99d4-dbda1d60a511 class="margin-0">cohortsMigration</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3c0ae373-2462-49dc-87d1-1a38e4752836 class="margin-0">billing</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3da72d31-68ec-4096-818b-f05db98ba718 class="margin-5">document_type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#453d0386-312d-4e22-976d-5f0c8f3dfd9f class="margin-5">document</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6b58770d-a4b3-46af-b748-e26aa5cf36ad class="margin-5">document_evidence</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#665e407b-53b7-43eb-a437-906ea41786dd class="margin-10">fieldname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2309b267-1f49-47b9-abe8-364b827ad708 class="margin-10">originalname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bd6759dd-42cf-4aae-b3e7-062b795ec3ea class="margin-10">encoding</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#54d6f06a-60bf-468f-82e8-33c121f52a17 class="margin-10">mimetype</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#71d313b8-fc1b-48f5-9d72-ae53d9eebe84 class="margin-10">size</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#227be7d0-697c-48af-9561-648a51ecf49d class="margin-10">bucket</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ce4270f0-2431-4f52-9f66-d9c62231a10f class="margin-10">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#572907b5-7fbf-422e-851c-1e9238156197 class="margin-10">acl</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f693ca8c-a34d-44b2-89c9-03c5cc473f0c class="margin-10">contentType</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#30d1a614-a8d5-44bc-bb1f-faaed158aede class="margin-10">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6e875dc7-7a93-4047-89a3-64d444b06801 class="margin-10">storageClass</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#07d9622d-e308-4a3f-89be-aafcbb71f387 class="margin-10">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#af5da64e-7dcf-4151-90ed-7acdb31e1a64 class="margin-10">metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ed1139bb-69ea-436b-a67f-2c24ddbe90c5 class="margin-15">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f304a1e7-c02b-410c-bed9-8f6145e2924b class="margin-15">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e903e4ba-738b-4b95-a607-12a694262758 class="margin-10">location</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e3b324ee-b774-405d-b9b1-6d15b5c87ca4 class="margin-10">etag</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6a7ee6be-433e-44f5-92c6-886fc9d20699 class="margin-10">versionId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8867f5e3-d4f0-4eea-966d-a3380b5c7b81 class="margin-5">corporate_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ef8ab477-c20c-401f-9d14-1adbffc8d2da class="margin-0">warehouse</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#68f4b692-3852-4a8d-b7eb-3221074cacb4 class="margin-5">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2e2e29e6-0482-4812-a5c0-ceeb408129e0 class="margin-5">status</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d119f2db-c96d-477d-9850-407d389498ed class="margin-5">old_warehouses</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9c079815-1182-4c69-a0d7-cd7576ab3019 class="margin-5">products_counter</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dd4b482c-55e1-474a-98ff-717de3c7a2ef class="margin-5">has_shared_products</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3fdd6662-5018-423d-991d-fbd020d8815e class="margin-0">refferal_settings</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a395528c-7280-451e-9a62-3d2682f9f8c7 class="margin-5">goal</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e9ad3af3-8523-44e1-98f1-577a0c55ac2d class="margin-5">goal_type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5dd50c83-c73c-42e5-ab6b-69464aafec87 class="margin-5">reward</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f5bae340-8952-4f46-a6c6-4814525735af class="margin-5">custom_commission</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8f0d6400-f2cc-4dd3-bc21-5e83080d149c class="margin-10">rkf_charge_percent</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8238957f-162a-476c-a37e-4f595830fe0d class="margin-10">constant_fee</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d059d20f-cc25-4463-9df3-89ad5c3da7a2 class="margin-0">balance_advance</a></td><td class="no-break-word">double</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a7160e13-7e23-48ef-977f-d6aa9fbf19aa class="margin-0">publicAPI</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ac6723a7-04b8-4523-be28-feb4453f13c6 class="margin-5">domain</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dea56063-3af9-4bfc-ab10-f460b8f37df4 class="margin-0">woocommerce</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#97ce625e-d858-43b8-9ec8-5d7357489faf class="margin-5">app_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2137d19d-48c3-4db9-9e87-7d4c2d2ea2dc class="margin-5">scope</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#87bd613d-3652-4390-ba93-5cbb4e327412 class="margin-5">user_id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#03336fb4-4ae3-488e-9c38-d1c0d0be8387 class="margin-5">return_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#21facc74-ba63-4e50-85cb-c83dbc9fb284 class="margin-5">callback_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dda2a908-f4f8-416d-a3f8-2323347607d4 class="margin-5">query_string</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e8710c73-40f3-4210-a7de-95e76c277059 class="margin-5">domain</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b7b43eaf-1f75-4176-87d6-522ed4e5a328 class="margin-5">auth_wc_api</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a7f31b68-fc53-4e97-8caa-bcfdfe3d2eaa class="margin-0">custom_servientrega</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9b6185d5-54f5-49aa-8ff4-f860d37b0e87 class="margin-5">user</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#92c3ba66-f267-4d5e-aac5-d33690a8253e class="margin-5">pwd</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#93fed53d-042d-4782-9654-6a6e9a1ca205 class="margin-5">billing_code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6db75db3-2723-4e10-a0ab-23eee4dad051 class="margin-5">nom_cargue</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e073e7b0-6cf9-43a8-8b25-76d09e6b3551 class="margin-5">id_product</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a9d4e174-0ac7-4351-954f-9083672efa0e class="margin-5">init_weight</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0f7187be-b68c-4da4-9a05-318da564fc46 class="margin-0">required_billing_validation</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6a868f88-dab3-4ac3-b5e9-1c37209b4f8c class="margin-0">questions</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d126f54d-0ccd-4e0a-b1c3-0c65144860bb class="margin-5">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5efb8e7a-1ec9-440a-9752-08db16e92154 class="margin-10">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#afe20082-b2df-42e0-9ca9-775e3598d4e8 class="margin-10">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7be45c90-5210-44f8-929c-a33a9224aa8b class="margin-10">answer</a></td><td class="no-break-word">array,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a85c0c37-c365-4c14-8f7c-c5e8a7f120de class="margin-15">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5e887fc4-3416-4a3c-b076-fc90a34b6dcc class="margin-20">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9f4b4beb-08b9-4892-8727-58e6dc19db04 class="margin-0">migrate_quick_wd</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bb75abec-e6dc-4e2e-8385-5721ef4dbfbc class="margin-0">migrated_contapyme</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ce87f866-1181-4d13-bac6-1223b8b9b565 class="margin-0">gifts</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9d3de58c-cd02-4589-94f6-b06d7573747b class="margin-5">shippings</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#04058119-8dbb-4b75-95d2-f800a75e9cf1 class="margin-10">quantity</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3e0b8a6b-83b8-4ab9-b683-52b75476bccf class="margin-0">dropshipper</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dc739228-8da5-47c7-bdad-3be25da0fb30 class="margin-5">date_created</a></td><td class="no-break-word">integer64</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#72c8ecdd-197d-433a-a1fc-ec65c7470c14 class="margin-5">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#286a2943-5d99-4afc-82ce-69a27f07e40a class="margin-0">last_connection_date</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ca20987e-ca6f-4f10-a6da-117d23d91e78 class="margin-5">format</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#54938ef9-60d7-44af-a8f5-b3c680d1618b class="margin-5">unix</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ae862b3a-9c19-4d1e-b45d-5e452b10aad2 class="margin-0">ban</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6b971885-76b9-4eaf-8263-79cca3a2f8f1 class="margin-5">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3c0cf2df-2f13-4bbc-85af-3c5817eb1a47 class="margin-0">store_information</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0e1a57dc-5ddb-4922-a1ba-522e77af5d41 class="margin-5">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7ed61ee0-e1bd-4e57-8048-3168a5d45382 class="margin-5">logo</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2fbbbdfd-e994-4b51-9973-5035cce8562d class="margin-5">banner</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9cc332aa-ab42-4f43-873b-bec0a5c09936 class="margin-0">blocked</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#32f84f08-13b8-46f1-8c02-ea69b9432c80 class="margin-0">enable_fast_withdraw</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c51aba41-3551-4d37-90c6-fc60ef63997f class="margin-0">indicative</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cf930d30-6b47-4a5f-b4cc-fecd6f037a37 class="margin-0">country_ref</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#25e3787b-c16e-4d9a-b163-f8cebf01f636 class="margin-5">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cbac59c3-47dd-4fbc-ba67-728b7b91c4c9 class="margin-5">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3e7d9459-71c1-42db-ac3a-2752206815fb class="margin-5">iso2</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a739af0a-76a2-4b8f-893a-d3b830eb84de class="margin-5">iso3</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8f932e74-62fb-4ecd-a8d7-0ef8ae76ccf3 class="margin-5">flag_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#48166c67-25b5-4ef7-8237-4deda2715f78 class="margin-5">phone_code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e4acc6e2-9421-4857-98ef-e42405e0394b class="margin-0">currency_ref</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c0ba7694-8fdf-4003-98fa-f2de1c0b70ac class="margin-5">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9030cd19-134a-4e10-a3c5-8c2798e71a5b class="margin-5">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#88d2b346-e65a-4d23-9f43-9cdcfabce142 class="margin-5">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2ed79b90-50ba-4212-bf46-dcd84e60c046 class="margin-5">htmlSymbol</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3cfe29b4-2eda-42cf-9560-4786ce790673 class="margin-0">scoringWarehouseReputation</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e57f4172-d5bf-4b51-b16f-48fc3d2c398a class="margin-5">averageChatResponse</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a399d7a1-c18b-49f0-a2e6-a2643344a3bd class="margin-5">averageChatResponseScore</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#311e7f61-6036-40d0-8430-cdae5fbb7cd3 class="margin-5">averageGuideTime</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#783dddde-6ac8-4267-8552-e11551e9c3a1 class="margin-5">averageGuideTimeScore</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#056d21dd-4129-45e0-8ca0-436c7064189b class="margin-5">cancellationRate</a></td><td class="no-break-word">double</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#948610c7-848c-46ad-a28d-2ed8450bbff6 class="margin-5">cancellationRateScore</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e74777ec-92c6-406d-a8de-05bf5c75e75b class="margin-5">final_score</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3d1716a5-ab96-45bf-9dc4-7b17926766f0 class="margin-0">subscription</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0eaf622f-9636-4538-af61-065ba8917c83 class="margin-5">plan</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c3312a13-2184-4385-bd2c-a46ba85f2a40 class="margin-5">remainingShipments</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d66853ac-3a1b-446b-82f7-6fad8ab01c8d class="margin-5">expiresAt</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ac4ba03d-0e49-4572-8a31-089dc6e41361 class="margin-5">isActive</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#13cbd748-952c-484d-9cbb-92334765ab3c class="margin-5">paymentMethodId</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="33c75581-9fb5-4487-9520-bd2807d98f16"></a>

###### 2.1.2.5.2.1 Field **\_id**

###### 2.1.2.5.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="945af247-d1cd-4c8a-a17f-f78a089e09f0"></a>

###### 2.1.2.5.2.2 Field **name**

###### 2.1.2.5.2.2.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>test two drop</td></tr></tbody></table>

### <a id="1cdda6a4-13f0-4561-8d0c-8e1362952f0c"></a>

###### 2.1.2.5.2.3 Field **email**

###### 2.1.2.5.2.3.1 **email** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>email</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>testtwo@test.co</td></tr></tbody></table>

### <a id="ff1ac9f3-9860-4fdd-8d06-a9ee97e41c72"></a>

###### 2.1.2.5.2.4 Field **phone**

###### 2.1.2.5.2.4.1 **phone** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>phone</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ec545f50-b52c-4fc8-8f0c-e45cf2821b0b"></a>

###### 2.1.2.5.2.5 Field **metadata**

###### 2.1.2.5.2.5.1 **metadata** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#8e2eee8f-8423-4ae9-b7f9-fbced594a464 class="margin-NaN">accept_time</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#19e151d2-da67-4f86-87de-658a15aa3c35 class="margin-NaN">hostname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8c7eff37-0ec3-4b52-b804-7e1e6015b5c2 class="margin-NaN">platform</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2d022b7c-5ef1-413e-95f3-c30b06b1d74c class="margin-NaN">networkInterfaces</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8cc53076-f4d0-4736-88b6-1b3513ad62f0 class="margin-NaN">from</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.5.2 **metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="8e2eee8f-8423-4ae9-b7f9-fbced594a464"></a>

###### 2.1.2.5.2.6 Field **accept\_time**

###### 2.1.2.5.2.6.1 **accept\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>accept_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1603230393</td></tr></tbody></table>

### <a id="19e151d2-da67-4f86-87de-658a15aa3c35"></a>

###### 2.1.2.5.2.7 Field **hostname**

###### 2.1.2.5.2.7.1 **hostname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>hostname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>DESKTOP-SSC8H1H</td></tr></tbody></table>

### <a id="8c7eff37-0ec3-4b52-b804-7e1e6015b5c2"></a>

###### 2.1.2.5.2.8 Field **platform**

###### 2.1.2.5.2.8.1 **platform** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>platform</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>win32</td></tr></tbody></table>

### <a id="2d022b7c-5ef1-413e-95f3-c30b06b1d74c"></a>

###### 2.1.2.5.2.9 Field **networkInterfaces**

###### 2.1.2.5.2.9.1 **networkInterfaces** Hierarchy

Parent field: **metadata**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#bfd4ad06-55b2-4d80-84fe-967739a922ee class="margin-NaN">Ethernet</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2f46c2a7-836c-4344-836c-ee185ba5d24d class="margin-NaN">Wi-Fi</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0f266d97-f930-49ca-8fe4-83e34b26897b class="margin-NaN">Loopback&nbsp;Pseudo-Interface&nbsp;1</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.9.2 **networkInterfaces** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>networkInterfaces</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="bfd4ad06-55b2-4d80-84fe-967739a922ee"></a>

###### 2.1.2.5.2.10 Field **Ethernet**

###### 2.1.2.5.2.10.1 **Ethernet** Hierarchy

Parent field: **networkInterfaces**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#7c2752ee-5a66-4e89-b79b-fc90e369e61f class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.10.2 **Ethernet** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Ethernet</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="7c2752ee-5a66-4e89-b79b-fc90e369e61f"></a>

###### 2.1.2.5.2.11 Field **\[0\]**

###### 2.1.2.5.2.11.1 **\[0\]** Hierarchy

Parent field: **Ethernet**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#73d42ea6-3e7a-4d5c-b368-73e02e3f886b class="margin-NaN">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f653a6b6-dd75-49c0-9099-d95ef2b35d3a class="margin-NaN">netmask</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c9cd12d7-bb85-4326-beae-a8c3ec273edc class="margin-NaN">family</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#67eb8694-239b-4c10-bd9e-f86d6911ea15 class="margin-NaN">mac</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0ca1c6c3-f21f-411d-b73c-90ced6aaa3c9 class="margin-NaN">internal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5e4abeff-cb63-4f7b-b636-5b74bfacc3cd class="margin-NaN">cidr</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f94199f3-376d-4dd1-b836-41a4ac8044f6 class="margin-NaN">scopeid</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.11.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="73d42ea6-3e7a-4d5c-b368-73e02e3f886b"></a>

###### 2.1.2.5.2.12 Field **address**

###### 2.1.2.5.2.12.1 **address** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>address</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>172.27.233.245</td></tr></tbody></table>

### <a id="f653a6b6-dd75-49c0-9099-d95ef2b35d3a"></a>

###### 2.1.2.5.2.13 Field **netmask**

###### 2.1.2.5.2.13.1 **netmask** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>netmask</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>255.255.248.0</td></tr></tbody></table>

### <a id="c9cd12d7-bb85-4326-beae-a8c3ec273edc"></a>

###### 2.1.2.5.2.14 Field **family**

###### 2.1.2.5.2.14.1 **family** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>family</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>IPv4</td></tr></tbody></table>

### <a id="67eb8694-239b-4c10-bd9e-f86d6911ea15"></a>

###### 2.1.2.5.2.15 Field **mac**

###### 2.1.2.5.2.15.1 **mac** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mac</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>00:ff:dd:1f:32:99</td></tr></tbody></table>

### <a id="0ca1c6c3-f21f-411d-b73c-90ced6aaa3c9"></a>

###### 2.1.2.5.2.16 Field **internal**

###### 2.1.2.5.2.16.1 **internal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>internal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="5e4abeff-cb63-4f7b-b636-5b74bfacc3cd"></a>

###### 2.1.2.5.2.17 Field **cidr**

###### 2.1.2.5.2.17.1 **cidr** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cidr</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>172.27.233.245/21</td></tr></tbody></table>

### <a id="f94199f3-376d-4dd1-b836-41a4ac8044f6"></a>

###### 2.1.2.5.2.18 Field **scopeid**

###### 2.1.2.5.2.18.1 **scopeid** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>scopeid</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>16</td></tr></tbody></table>

### <a id="2f46c2a7-836c-4344-836c-ee185ba5d24d"></a>

###### 2.1.2.5.2.19 Field **Wi-Fi**

###### 2.1.2.5.2.19.1 **Wi-Fi** Hierarchy

Parent field: **networkInterfaces**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#874edb61-9142-4dd7-bd21-a4c42915b672 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.19.2 **Wi-Fi** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Wi-Fi</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="874edb61-9142-4dd7-bd21-a4c42915b672"></a>

###### 2.1.2.5.2.20 Field **\[0\]**

###### 2.1.2.5.2.20.1 **\[0\]** Hierarchy

Parent field: **Wi-Fi**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#f981b30b-5a4c-4652-a010-82e5299d169c class="margin-NaN">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dc10c421-5451-4765-af43-87e3561d40d1 class="margin-NaN">netmask</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b8e6d40f-4071-4c2d-8683-2f2fe454042d class="margin-NaN">family</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#02176330-400c-4c81-91aa-a200c2f45053 class="margin-NaN">mac</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a8959a1c-0847-4360-88bf-6dacea970813 class="margin-NaN">internal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0e5fac72-8cf6-4a12-a1b5-8f29c0a113b5 class="margin-NaN">cidr</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0055072d-3686-4d9c-a550-544491524736 class="margin-NaN">scopeid</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.20.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="f981b30b-5a4c-4652-a010-82e5299d169c"></a>

###### 2.1.2.5.2.21 Field **address**

###### 2.1.2.5.2.21.1 **address** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>address</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>192.168.1.43</td></tr></tbody></table>

### <a id="dc10c421-5451-4765-af43-87e3561d40d1"></a>

###### 2.1.2.5.2.22 Field **netmask**

###### 2.1.2.5.2.22.1 **netmask** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>netmask</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>255.255.255.0</td></tr></tbody></table>

### <a id="b8e6d40f-4071-4c2d-8683-2f2fe454042d"></a>

###### 2.1.2.5.2.23 Field **family**

###### 2.1.2.5.2.23.1 **family** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>family</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>IPv4</td></tr></tbody></table>

### <a id="02176330-400c-4c81-91aa-a200c2f45053"></a>

###### 2.1.2.5.2.24 Field **mac**

###### 2.1.2.5.2.24.1 **mac** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mac</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>a0:51:0b:15:8f:ec</td></tr></tbody></table>

### <a id="a8959a1c-0847-4360-88bf-6dacea970813"></a>

###### 2.1.2.5.2.25 Field **internal**

###### 2.1.2.5.2.25.1 **internal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>internal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="0e5fac72-8cf6-4a12-a1b5-8f29c0a113b5"></a>

###### 2.1.2.5.2.26 Field **cidr**

###### 2.1.2.5.2.26.1 **cidr** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cidr</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>192.168.1.43/24</td></tr></tbody></table>

### <a id="0055072d-3686-4d9c-a550-544491524736"></a>

###### 2.1.2.5.2.27 Field **scopeid**

###### 2.1.2.5.2.27.1 **scopeid** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>scopeid</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>10</td></tr></tbody></table>

### <a id="0f266d97-f930-49ca-8fe4-83e34b26897b"></a>

###### 2.1.2.5.2.28 Field **Loopback Pseudo-Interface 1**

###### 2.1.2.5.2.28.1 **Loopback Pseudo-Interface 1** Hierarchy

Parent field: **networkInterfaces**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#7df5dd6f-6e6e-4ef4-8d67-3e44a28c5e07 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.28.2 **Loopback Pseudo-Interface 1** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Loopback Pseudo-Interface 1</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="7df5dd6f-6e6e-4ef4-8d67-3e44a28c5e07"></a>

###### 2.1.2.5.2.29 Field **\[0\]**

###### 2.1.2.5.2.29.1 **\[0\]** Hierarchy

Parent field: **Loopback Pseudo-Interface 1**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#a319e91a-aced-4c15-a0c2-9609ec50e81e class="margin-NaN">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7046af0e-2f87-462d-ab7a-fff9114c3cad class="margin-NaN">netmask</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a4bdc91e-81ee-4958-bb8e-a20e26cb7e37 class="margin-NaN">family</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8bd581e6-89a0-4e57-8206-019f3e5ec694 class="margin-NaN">mac</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6402156b-3964-4b1a-aa9c-dfb07c70586b class="margin-NaN">internal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0a250e92-bbab-4715-ad9b-3969dcd299b7 class="margin-NaN">cidr</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#30ccbedd-8879-47d7-8d71-6f8fa1d80d4b class="margin-NaN">scopeid</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.29.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="a319e91a-aced-4c15-a0c2-9609ec50e81e"></a>

###### 2.1.2.5.2.30 Field **address**

###### 2.1.2.5.2.30.1 **address** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>address</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>127.0.0.1</td></tr></tbody></table>

### <a id="7046af0e-2f87-462d-ab7a-fff9114c3cad"></a>

###### 2.1.2.5.2.31 Field **netmask**

###### 2.1.2.5.2.31.1 **netmask** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>netmask</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>255.0.0.0</td></tr></tbody></table>

### <a id="a4bdc91e-81ee-4958-bb8e-a20e26cb7e37"></a>

###### 2.1.2.5.2.32 Field **family**

###### 2.1.2.5.2.32.1 **family** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>family</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>IPv4</td></tr></tbody></table>

### <a id="8bd581e6-89a0-4e57-8206-019f3e5ec694"></a>

###### 2.1.2.5.2.33 Field **mac**

###### 2.1.2.5.2.33.1 **mac** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mac</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>00:00:00:00:00:00</td></tr></tbody></table>

### <a id="6402156b-3964-4b1a-aa9c-dfb07c70586b"></a>

###### 2.1.2.5.2.34 Field **internal**

###### 2.1.2.5.2.34.1 **internal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>internal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="0a250e92-bbab-4715-ad9b-3969dcd299b7"></a>

###### 2.1.2.5.2.35 Field **cidr**

###### 2.1.2.5.2.35.1 **cidr** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cidr</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>127.0.0.1/8</td></tr></tbody></table>

### <a id="30ccbedd-8879-47d7-8d71-6f8fa1d80d4b"></a>

###### 2.1.2.5.2.36 Field **scopeid**

###### 2.1.2.5.2.36.1 **scopeid** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>scopeid</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="8cc53076-f4d0-4736-88b6-1b3513ad62f0"></a>

###### 2.1.2.5.2.37 Field **from**

###### 2.1.2.5.2.37.1 **from** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>from</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>organico</td></tr></tbody></table>

### <a id="ae56d219-435c-4424-b2dd-82747b7c94cb"></a>

###### 2.1.2.5.2.38 Field **pageId**

###### 2.1.2.5.2.38.1 **pageId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>pageId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>247456575848438</td></tr></tbody></table>

### <a id="7fa9b648-96f2-4145-b5c0-11a173cd0b0e"></a>

###### 2.1.2.5.2.39 Field **dbname**

###### 2.1.2.5.2.39.1 **dbname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dbname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>testtwodrop_804079258</td></tr></tbody></table>

### <a id="0ea96ddc-c9be-4494-bfff-540a55723c04"></a>

###### 2.1.2.5.2.40 Field **plan**

###### 2.1.2.5.2.40.1 **plan** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>plan</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>pro</td></tr></tbody></table>

### <a id="3c6f0b20-5f47-43c6-914a-434161a50cf9"></a>

###### 2.1.2.5.2.41 Field **country**

###### 2.1.2.5.2.41.1 **country** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>COL</td></tr></tbody></table>

### <a id="f345e444-7955-4564-9d49-9b08ac38c77a"></a>

###### 2.1.2.5.2.42 Field **test**

###### 2.1.2.5.2.42.1 **test** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>test</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="54a6d97f-ff02-4aba-9f0c-35490dd449c3"></a>

###### 2.1.2.5.2.43 Field **actived**

###### 2.1.2.5.2.43.1 **actived** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>actived</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="0d9dd937-3454-4ca8-9aa9-f7d1fd784358"></a>

###### 2.1.2.5.2.44 Field **exp**

###### 2.1.2.5.2.44.1 **exp** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>exp</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1604526393</td></tr></tbody></table>

### <a id="d5fe7c4b-1bfa-4b85-8972-5c6fde74d367"></a>

###### 2.1.2.5.2.45 Field **created\_time**

###### 2.1.2.5.2.45.1 **created\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1603230393</td></tr></tbody></table>

### <a id="9e8a4ab0-4243-446a-b5c3-fc4238639306"></a>

###### 2.1.2.5.2.46 Field **created\_date**

###### 2.1.2.5.2.46.1 **created\_date** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#91c4826a-ef5b-406d-8cee-5e0392af76c7 class="margin-NaN">dateFormat</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cd5cea5c-91ee-46de-a6ef-56e214bd0efb class="margin-NaN">hourFormat</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1800b1fe-dec0-4c4f-a323-fd2f81c74467 class="margin-NaN">toDate</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.46.2 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="91c4826a-ef5b-406d-8cee-5e0392af76c7"></a>

###### 2.1.2.5.2.47 Field **dateFormat**

###### 2.1.2.5.2.47.1 **dateFormat** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dateFormat</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>ISODate("2020-10-20")</td></tr></tbody></table>

### <a id="cd5cea5c-91ee-46de-a6ef-56e214bd0efb"></a>

###### 2.1.2.5.2.48 Field **hourFormat**

###### 2.1.2.5.2.48.1 **hourFormat** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>hourFormat</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Format</td><td>time</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>16:46:33</td></tr></tbody></table>

### <a id="1800b1fe-dec0-4c4f-a323-fd2f81c74467"></a>

###### 2.1.2.5.2.49 Field **toDate**

###### 2.1.2.5.2.49.1 **toDate** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>toDate</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>ISODate("2020-10-20T16:46:33-05:00")</td></tr></tbody></table>

### <a id="c30f0611-6534-4cd1-be32-246ed5195239"></a>

###### 2.1.2.5.2.50 Field **host\_asterisk**

###### 2.1.2.5.2.50.1 **host\_asterisk** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>host_asterisk</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="01803ffb-8fec-40af-9447-bcf8a629ff3b"></a>

###### 2.1.2.5.2.51 Field **user\_asterisk**

###### 2.1.2.5.2.51.1 **user\_asterisk** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>user_asterisk</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="fcaeadba-6fee-4b4d-9760-bba6674c722e"></a>

###### 2.1.2.5.2.52 Field **pass\_asterisk**

###### 2.1.2.5.2.52.1 **pass\_asterisk** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>pass_asterisk</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="0de8637d-9cc9-4750-997f-502e5318e6a0"></a>

###### 2.1.2.5.2.53 Field **visible**

###### 2.1.2.5.2.53.1 **visible** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>visible</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="646c2174-4f2b-4c72-b0ad-703ca4e1b38d"></a>

###### 2.1.2.5.2.54 Field **slug**

###### 2.1.2.5.2.54.1 **slug** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>slug</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>testtwodrop2</td></tr></tbody></table>

### <a id="4067dba8-364a-4119-b154-61bed239fb48"></a>

###### 2.1.2.5.2.55 Field **sender**

###### 2.1.2.5.2.55.1 **sender** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#3a783962-191e-4c6b-80b7-eaaa2e33ac94 class="margin-NaN">date</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1f3b6a1a-3f25-4bc9-97d0-76a4d31a1430 class="margin-NaN">shippings_count</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.55.2 **sender** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>sender</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="3a783962-191e-4c6b-80b7-eaaa2e33ac94"></a>

###### 2.1.2.5.2.56 Field **date**

###### 2.1.2.5.2.56.1 **date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1605713844</td></tr></tbody></table>

### <a id="1f3b6a1a-3f25-4bc9-97d0-76a4d31a1430"></a>

###### 2.1.2.5.2.57 Field **shippings\_count**

###### 2.1.2.5.2.57.1 **shippings\_count** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shippings_count</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>370</td></tr></tbody></table>

### <a id="4c6d80c1-eb3a-4ba1-bc41-c5030f79dc15"></a>

###### 2.1.2.5.2.58 Field **updated\_date**

###### 2.1.2.5.2.58.1 **updated\_date** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#a18d20bb-0a47-4ac6-bc2a-7ec5238f2a1b class="margin-NaN">created_sender</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.58.2 **updated\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>updated_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="a18d20bb-0a47-4ac6-bc2a-7ec5238f2a1b"></a>

###### 2.1.2.5.2.59 Field **created\_sender**

###### 2.1.2.5.2.59.1 **created\_sender** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_sender</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1605713844</td></tr></tbody></table>

### <a id="9a7aed9d-9833-4314-84d9-f7f5f4749b32"></a>

###### 2.1.2.5.2.60 Field **cohortMigrated3**

###### 2.1.2.5.2.60.1 **cohortMigrated3** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cohortMigrated3</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="8290f3b9-e51e-4231-811c-6a68d24c00ec"></a>

###### 2.1.2.5.2.61 Field **blocked\_balance**

###### 2.1.2.5.2.61.1 **blocked\_balance** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>blocked_balance</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>4772129.24744489</td></tr></tbody></table>

### <a id="c005368e-01ab-4bf7-8b26-ce8e34f65d17"></a>

###### 2.1.2.5.2.62 Field **rocketfy\_leads**

###### 2.1.2.5.2.62.1 **rocketfy\_leads** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>rocketfy_leads</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="87df5c04-95f7-4c08-a2ef-48e1a328af54"></a>

###### 2.1.2.5.2.63 Field **rocketfy\_shipping**

###### 2.1.2.5.2.63.1 **rocketfy\_shipping** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>rocketfy_shipping</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c5cf1b4e-6a08-4e5e-99d4-dbda1d60a511"></a>

###### 2.1.2.5.2.64 Field **cohortsMigration**

###### 2.1.2.5.2.64.1 **cohortsMigration** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cohortsMigration</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="3c0ae373-2462-49dc-87d1-1a38e4752836"></a>

###### 2.1.2.5.2.65 Field **billing**

###### 2.1.2.5.2.65.1 **billing** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#3da72d31-68ec-4096-818b-f05db98ba718 class="margin-NaN">document_type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#453d0386-312d-4e22-976d-5f0c8f3dfd9f class="margin-NaN">document</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6b58770d-a4b3-46af-b748-e26aa5cf36ad class="margin-NaN">document_evidence</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8867f5e3-d4f0-4eea-966d-a3380b5c7b81 class="margin-NaN">corporate_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.65.2 **billing** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>billing</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="3da72d31-68ec-4096-818b-f05db98ba718"></a>

###### 2.1.2.5.2.66 Field **document\_type**

###### 2.1.2.5.2.66.1 **document\_type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>document_type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>CC</td></tr></tbody></table>

### <a id="453d0386-312d-4e22-976d-5f0c8f3dfd9f"></a>

###### 2.1.2.5.2.67 Field **document**

###### 2.1.2.5.2.67.1 **document** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>document</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1036676072</td></tr></tbody></table>

### <a id="6b58770d-a4b3-46af-b748-e26aa5cf36ad"></a>

###### 2.1.2.5.2.68 Field **document\_evidence**

###### 2.1.2.5.2.68.1 **document\_evidence** Hierarchy

Parent field: **billing**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#665e407b-53b7-43eb-a437-906ea41786dd class="margin-NaN">fieldname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2309b267-1f49-47b9-abe8-364b827ad708 class="margin-NaN">originalname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bd6759dd-42cf-4aae-b3e7-062b795ec3ea class="margin-NaN">encoding</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#54d6f06a-60bf-468f-82e8-33c121f52a17 class="margin-NaN">mimetype</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#71d313b8-fc1b-48f5-9d72-ae53d9eebe84 class="margin-NaN">size</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#227be7d0-697c-48af-9561-648a51ecf49d class="margin-NaN">bucket</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ce4270f0-2431-4f52-9f66-d9c62231a10f class="margin-NaN">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#572907b5-7fbf-422e-851c-1e9238156197 class="margin-NaN">acl</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f693ca8c-a34d-44b2-89c9-03c5cc473f0c class="margin-NaN">contentType</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#30d1a614-a8d5-44bc-bb1f-faaed158aede class="margin-NaN">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6e875dc7-7a93-4047-89a3-64d444b06801 class="margin-NaN">storageClass</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#07d9622d-e308-4a3f-89be-aafcbb71f387 class="margin-NaN">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#af5da64e-7dcf-4151-90ed-7acdb31e1a64 class="margin-NaN">metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e903e4ba-738b-4b95-a607-12a694262758 class="margin-NaN">location</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e3b324ee-b774-405d-b9b1-6d15b5c87ca4 class="margin-NaN">etag</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6a7ee6be-433e-44f5-92c6-886fc9d20699 class="margin-NaN">versionId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.68.2 **document\_evidence** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>document_evidence</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="665e407b-53b7-43eb-a437-906ea41786dd"></a>

###### 2.1.2.5.2.69 Field **fieldname**

###### 2.1.2.5.2.69.1 **fieldname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="2309b267-1f49-47b9-abe8-364b827ad708"></a>

###### 2.1.2.5.2.70 Field **originalname**

###### 2.1.2.5.2.70.1 **originalname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>originalname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>WhatsApp Image 2021-05-13 at 2.11.05 PM.jpeg</td></tr></tbody></table>

### <a id="bd6759dd-42cf-4aae-b3e7-062b795ec3ea"></a>

###### 2.1.2.5.2.71 Field **encoding**

###### 2.1.2.5.2.71.1 **encoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>encoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>7bit</td></tr></tbody></table>

### <a id="54d6f06a-60bf-468f-82e8-33c121f52a17"></a>

###### 2.1.2.5.2.72 Field **mimetype**

###### 2.1.2.5.2.72.1 **mimetype** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mimetype</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="71d313b8-fc1b-48f5-9d72-ae53d9eebe84"></a>

###### 2.1.2.5.2.73 Field **size**

###### 2.1.2.5.2.73.1 **size** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>size</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>54187</td></tr></tbody></table>

### <a id="227be7d0-697c-48af-9561-648a51ecf49d"></a>

###### 2.1.2.5.2.74 Field **bucket**

###### 2.1.2.5.2.74.1 **bucket** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>bucket</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>shopping-rocketfy-uploads</td></tr></tbody></table>

### <a id="ce4270f0-2431-4f52-9f66-d9c62231a10f"></a>

###### 2.1.2.5.2.75 Field **key**

###### 2.1.2.5.2.75.1 **key** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>key</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>WhatsApp Image 2021-05-13 at 2.11.05 PM.jpeg</td></tr></tbody></table>

### <a id="572907b5-7fbf-422e-851c-1e9238156197"></a>

###### 2.1.2.5.2.76 Field **acl**

###### 2.1.2.5.2.76.1 **acl** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>acl</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>public-read</td></tr></tbody></table>

### <a id="f693ca8c-a34d-44b2-89c9-03c5cc473f0c"></a>

###### 2.1.2.5.2.77 Field **contentType**

###### 2.1.2.5.2.77.1 **contentType** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentType</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="30d1a614-a8d5-44bc-bb1f-faaed158aede"></a>

###### 2.1.2.5.2.78 Field **contentDisposition**

###### 2.1.2.5.2.78.1 **contentDisposition** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentDisposition</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="6e875dc7-7a93-4047-89a3-64d444b06801"></a>

###### 2.1.2.5.2.79 Field **storageClass**

###### 2.1.2.5.2.79.1 **storageClass** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>storageClass</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>STANDARD</td></tr></tbody></table>

### <a id="07d9622d-e308-4a3f-89be-aafcbb71f387"></a>

###### 2.1.2.5.2.80 Field **serverSideEncryption**

###### 2.1.2.5.2.80.1 **serverSideEncryption** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>serverSideEncryption</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="af5da64e-7dcf-4151-90ed-7acdb31e1a64"></a>

###### 2.1.2.5.2.81 Field **metadata**

###### 2.1.2.5.2.81.1 **metadata** Hierarchy

Parent field: **document\_evidence**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#ed1139bb-69ea-436b-a67f-2c24ddbe90c5 class="margin-NaN">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f304a1e7-c02b-410c-bed9-8f6145e2924b class="margin-NaN">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.81.2 **metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="ed1139bb-69ea-436b-a67f-2c24ddbe90c5"></a>

###### 2.1.2.5.2.82 Field **fieldName**

###### 2.1.2.5.2.82.1 **fieldName** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldName</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="f304a1e7-c02b-410c-bed9-8f6145e2924b"></a>

###### 2.1.2.5.2.83 Field **Content-Type**

###### 2.1.2.5.2.83.1 **Content-Type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Content-Type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="e903e4ba-738b-4b95-a607-12a694262758"></a>

###### 2.1.2.5.2.84 Field **location**

###### 2.1.2.5.2.84.1 **location** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>location</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://shopping-rocketfy-uploads.s3.amazonaws.com/WhatsApp%20Image%202021-05-13%20at%202.11.05%20PM.jpeg</td></tr></tbody></table>

### <a id="e3b324ee-b774-405d-b9b1-6d15b5c87ca4"></a>

###### 2.1.2.5.2.85 Field **etag**

###### 2.1.2.5.2.85.1 **etag** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>etag</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>"27ab062edb3d65c172f6f4f5517545a5"</td></tr></tbody></table>

### <a id="6a7ee6be-433e-44f5-92c6-886fc9d20699"></a>

###### 2.1.2.5.2.86 Field **versionId**

###### 2.1.2.5.2.86.1 **versionId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>versionId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>ww6gGdpZn1oU1KnEFHxtyYzRJK7ITsPv</td></tr></tbody></table>

### <a id="8867f5e3-d4f0-4eea-966d-a3380b5c7b81"></a>

###### 2.1.2.5.2.87 Field **corporate\_name**

###### 2.1.2.5.2.87.1 **corporate\_name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>corporate_name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>JUAN PABLO GUTIERREZ VARGAS</td></tr></tbody></table>

### <a id="ef8ab477-c20c-401f-9d14-1adbffc8d2da"></a>

###### 2.1.2.5.2.88 Field **warehouse**

###### 2.1.2.5.2.88.1 **warehouse** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#68f4b692-3852-4a8d-b7eb-3221074cacb4 class="margin-NaN">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2e2e29e6-0482-4812-a5c0-ceeb408129e0 class="margin-NaN">status</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d119f2db-c96d-477d-9850-407d389498ed class="margin-NaN">old_warehouses</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9c079815-1182-4c69-a0d7-cd7576ab3019 class="margin-NaN">products_counter</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dd4b482c-55e1-474a-98ff-717de3c7a2ef class="margin-NaN">has_shared_products</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.88.2 **warehouse** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>warehouse</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="68f4b692-3852-4a8d-b7eb-3221074cacb4"></a>

###### 2.1.2.5.2.89 Field **active**

###### 2.1.2.5.2.89.1 **active** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>active</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="2e2e29e6-0482-4812-a5c0-ceeb408129e0"></a>

###### 2.1.2.5.2.90 Field **status**

###### 2.1.2.5.2.90.1 **status** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>status</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>rejected</td></tr></tbody></table>

### <a id="d119f2db-c96d-477d-9850-407d389498ed"></a>

###### 2.1.2.5.2.91 Field **old\_warehouses**

###### 2.1.2.5.2.91.1 **old\_warehouses** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>old_warehouses</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="9c079815-1182-4c69-a0d7-cd7576ab3019"></a>

###### 2.1.2.5.2.92 Field **products\_counter**

###### 2.1.2.5.2.92.1 **products\_counter** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>products_counter</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="dd4b482c-55e1-474a-98ff-717de3c7a2ef"></a>

###### 2.1.2.5.2.93 Field **has\_shared\_products**

###### 2.1.2.5.2.93.1 **has\_shared\_products** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>has_shared_products</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="3fdd6662-5018-423d-991d-fbd020d8815e"></a>

###### 2.1.2.5.2.94 Field **refferal\_settings**

###### 2.1.2.5.2.94.1 **refferal\_settings** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#a395528c-7280-451e-9a62-3d2682f9f8c7 class="margin-NaN">goal</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e9ad3af3-8523-44e1-98f1-577a0c55ac2d class="margin-NaN">goal_type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5dd50c83-c73c-42e5-ab6b-69464aafec87 class="margin-NaN">reward</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f5bae340-8952-4f46-a6c6-4814525735af class="margin-NaN">custom_commission</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.94.2 **refferal\_settings** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>refferal_settings</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="a395528c-7280-451e-9a62-3d2682f9f8c7"></a>

###### 2.1.2.5.2.95 Field **goal**

###### 2.1.2.5.2.95.1 **goal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>goal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>100</td></tr></tbody></table>

### <a id="e9ad3af3-8523-44e1-98f1-577a0c55ac2d"></a>

###### 2.1.2.5.2.96 Field **goal\_type**

###### 2.1.2.5.2.96.1 **goal\_type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>goal_type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>orders</td></tr></tbody></table>

### <a id="5dd50c83-c73c-42e5-ab6b-69464aafec87"></a>

###### 2.1.2.5.2.97 Field **reward**

###### 2.1.2.5.2.97.1 **reward** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>reward</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>500</td></tr></tbody></table>

### <a id="f5bae340-8952-4f46-a6c6-4814525735af"></a>

###### 2.1.2.5.2.98 Field **custom\_commission**

###### 2.1.2.5.2.98.1 **custom\_commission** Hierarchy

Parent field: **refferal\_settings**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#8f0d6400-f2cc-4dd3-bc21-5e83080d149c class="margin-NaN">rkf_charge_percent</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8238957f-162a-476c-a37e-4f595830fe0d class="margin-NaN">constant_fee</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.98.2 **custom\_commission** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>custom_commission</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="8f0d6400-f2cc-4dd3-bc21-5e83080d149c"></a>

###### 2.1.2.5.2.99 Field **rkf\_charge\_percent**

###### 2.1.2.5.2.99.1 **rkf\_charge\_percent** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>rkf_charge_percent</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="8238957f-162a-476c-a37e-4f595830fe0d"></a>

###### 2.1.2.5.2.100 Field **constant\_fee**

###### 2.1.2.5.2.100.1 **constant\_fee** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>constant_fee</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="d059d20f-cc25-4463-9df3-89ad5c3da7a2"></a>

###### 2.1.2.5.2.101 Field **balance\_advance**

###### 2.1.2.5.2.101.1 **balance\_advance** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>balance_advance</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a7160e13-7e23-48ef-977f-d6aa9fbf19aa"></a>

###### 2.1.2.5.2.102 Field **publicAPI**

###### 2.1.2.5.2.102.1 **publicAPI** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#ac6723a7-04b8-4523-be28-feb4453f13c6 class="margin-NaN">domain</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.102.2 **publicAPI** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>publicAPI</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="ac6723a7-04b8-4523-be28-feb4453f13c6"></a>

###### 2.1.2.5.2.103 Field **domain**

###### 2.1.2.5.2.103.1 **domain** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>domain</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://test.co</td></tr></tbody></table>

### <a id="dea56063-3af9-4bfc-ab10-f460b8f37df4"></a>

###### 2.1.2.5.2.104 Field **woocommerce**

###### 2.1.2.5.2.104.1 **woocommerce** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#97ce625e-d858-43b8-9ec8-5d7357489faf class="margin-NaN">app_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2137d19d-48c3-4db9-9e87-7d4c2d2ea2dc class="margin-NaN">scope</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#87bd613d-3652-4390-ba93-5cbb4e327412 class="margin-NaN">user_id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#03336fb4-4ae3-488e-9c38-d1c0d0be8387 class="margin-NaN">return_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#21facc74-ba63-4e50-85cb-c83dbc9fb284 class="margin-NaN">callback_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dda2a908-f4f8-416d-a3f8-2323347607d4 class="margin-NaN">query_string</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e8710c73-40f3-4210-a7de-95e76c277059 class="margin-NaN">domain</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b7b43eaf-1f75-4176-87d6-522ed4e5a328 class="margin-NaN">auth_wc_api</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.104.2 **woocommerce** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>woocommerce</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="97ce625e-d858-43b8-9ec8-5d7357489faf"></a>

###### 2.1.2.5.2.105 Field **app\_name**

###### 2.1.2.5.2.105.1 **app\_name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>app_name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Rocketfy</td></tr></tbody></table>

### <a id="2137d19d-48c3-4db9-9e87-7d4c2d2ea2dc"></a>

###### 2.1.2.5.2.106 Field **scope**

###### 2.1.2.5.2.106.1 **scope** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>scope</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>read_write</td></tr></tbody></table>

### <a id="87bd613d-3652-4390-ba93-5cbb4e327412"></a>

###### 2.1.2.5.2.107 Field **user\_id**

###### 2.1.2.5.2.107.1 **user\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>user_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>5f8f5ab9d4240339c4281f5f</td></tr></tbody></table>

### <a id="03336fb4-4ae3-488e-9c38-d1c0d0be8387"></a>

###### 2.1.2.5.2.108 Field **return\_url**

###### 2.1.2.5.2.108.1 **return\_url** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>return_url</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://app.rocketfy.co/orders/pending</td></tr></tbody></table>

### <a id="21facc74-ba63-4e50-85cb-c83dbc9fb284"></a>

###### 2.1.2.5.2.109 Field **callback\_url**

###### 2.1.2.5.2.109.1 **callback\_url** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>callback_url</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://rest.rocketfy.co/api/wc/hookauthwoocommerce</td></tr></tbody></table>

### <a id="dda2a908-f4f8-416d-a3f8-2323347607d4"></a>

###### 2.1.2.5.2.110 Field **query\_string**

###### 2.1.2.5.2.110.1 **query\_string** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>query_string</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://renechardon.com/wc-auth/v1/authorize?app_name=Rocketfy&amp;scope=read_write&amp;user_id=5f8f5ab9d4240339c4281f5f&amp;return_url=https%3A%2F%2Fapp.rocketfy.co%2Forders%2Fpending&amp;callback_url=https%3A%2F%2Frest.rocketfy.co%2Fapi%2Fwc%2Fhookauthwoocommerce</td></tr></tbody></table>

### <a id="e8710c73-40f3-4210-a7de-95e76c277059"></a>

###### 2.1.2.5.2.111 Field **domain**

###### 2.1.2.5.2.111.1 **domain** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>domain</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://renechardon.com</td></tr></tbody></table>

### <a id="b7b43eaf-1f75-4176-87d6-522ed4e5a328"></a>

###### 2.1.2.5.2.112 Field **auth\_wc\_api**

###### 2.1.2.5.2.112.1 **auth\_wc\_api** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>auth_wc_api</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="a7f31b68-fc53-4e97-8caa-bcfdfe3d2eaa"></a>

###### 2.1.2.5.2.113 Field **custom\_servientrega**

###### 2.1.2.5.2.113.1 **custom\_servientrega** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#9b6185d5-54f5-49aa-8ff4-f860d37b0e87 class="margin-NaN">user</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#92c3ba66-f267-4d5e-aac5-d33690a8253e class="margin-NaN">pwd</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#93fed53d-042d-4782-9654-6a6e9a1ca205 class="margin-NaN">billing_code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6db75db3-2723-4e10-a0ab-23eee4dad051 class="margin-NaN">nom_cargue</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e073e7b0-6cf9-43a8-8b25-76d09e6b3551 class="margin-NaN">id_product</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a9d4e174-0ac7-4351-954f-9083672efa0e class="margin-NaN">init_weight</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.113.2 **custom\_servientrega** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>custom_servientrega</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="9b6185d5-54f5-49aa-8ff4-f860d37b0e87"></a>

###### 2.1.2.5.2.114 Field **user**

###### 2.1.2.5.2.114.1 **user** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>user</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>901195703</td></tr></tbody></table>

### <a id="92c3ba66-f267-4d5e-aac5-d33690a8253e"></a>

###### 2.1.2.5.2.115 Field **pwd**

###### 2.1.2.5.2.115.1 **pwd** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>pwd</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>BpSUh12jBIipnUY/8yu2pQ==</td></tr></tbody></table>

### <a id="93fed53d-042d-4782-9654-6a6e9a1ca205"></a>

###### 2.1.2.5.2.116 Field **billing\_code**

###### 2.1.2.5.2.116.1 **billing\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>billing_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>SER123726</td></tr></tbody></table>

### <a id="6db75db3-2723-4e10-a0ab-23eee4dad051"></a>

###### 2.1.2.5.2.117 Field **nom\_cargue**

###### 2.1.2.5.2.117.1 **nom\_cargue** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>nom_cargue</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Industrial</td></tr></tbody></table>

### <a id="e073e7b0-6cf9-43a8-8b25-76d09e6b3551"></a>

###### 2.1.2.5.2.118 Field **id\_product**

###### 2.1.2.5.2.118.1 **id\_product** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id_product</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6</td></tr></tbody></table>

### <a id="a9d4e174-0ac7-4351-954f-9083672efa0e"></a>

###### 2.1.2.5.2.119 Field **init\_weight**

###### 2.1.2.5.2.119.1 **init\_weight** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>init_weight</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>2000</td></tr></tbody></table>

### <a id="0f7187be-b68c-4da4-9a05-318da564fc46"></a>

###### 2.1.2.5.2.120 Field **required\_billing\_validation**

###### 2.1.2.5.2.120.1 **required\_billing\_validation** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>required_billing_validation</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="6a868f88-dab3-4ac3-b5e9-1c37209b4f8c"></a>

###### 2.1.2.5.2.121 Field **questions**

###### 2.1.2.5.2.121.1 **questions** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#d126f54d-0ccd-4e0a-b1c3-0c65144860bb class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.121.2 **questions** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>questions</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="d126f54d-0ccd-4e0a-b1c3-0c65144860bb"></a>

###### 2.1.2.5.2.122 Field **\[0\]**

###### 2.1.2.5.2.122.1 **\[0\]** Hierarchy

Parent field: **questions**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#5efb8e7a-1ec9-440a-9752-08db16e92154 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#afe20082-b2df-42e0-9ca9-775e3598d4e8 class="margin-NaN">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7be45c90-5210-44f8-929c-a33a9224aa8b class="margin-NaN">answer</a></td><td class="no-break-word">array,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.122.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="5efb8e7a-1ec9-440a-9752-08db16e92154"></a>

###### 2.1.2.5.2.123 Field **name**

###### 2.1.2.5.2.123.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>¿En qué necesita ayuda?</td></tr></tbody></table>

### <a id="afe20082-b2df-42e0-9ca9-775e3598d4e8"></a>

###### 2.1.2.5.2.124 Field **key**

###### 2.1.2.5.2.124.1 **key** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>key</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>need_help</td></tr></tbody></table>

### <a id="7be45c90-5210-44f8-929c-a33a9224aa8b"></a>

###### 2.1.2.5.2.125 Field **answer**

###### 2.1.2.5.2.125.1 **answer** Hierarchy

Parent field: **\[0\]**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#a85c0c37-c365-4c14-8f7c-c5e8a7f120de class="margin-NaN">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.125.2 **answer** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>answer</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (array,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a85c0c37-c365-4c14-8f7c-c5e8a7f120de"></a>

###### 2.1.2.5.2.126 Field **items**

###### 2.1.2.5.2.126.1 **items** Hierarchy

Parent field: **answer**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#5e887fc4-3416-4a3c-b076-fc90a34b6dcc class="margin-NaN">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.126.2 **items** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="5e887fc4-3416-4a3c-b076-fc90a34b6dcc"></a>

###### 2.1.2.5.2.127 Field **\[0\]**

###### 2.1.2.5.2.127.1 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr></tbody></table>

### <a id="9f4b4beb-08b9-4892-8727-58e6dc19db04"></a>

###### 2.1.2.5.2.128 Field **migrate\_quick\_wd**

###### 2.1.2.5.2.128.1 **migrate\_quick\_wd** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>migrate_quick_wd</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="bb75abec-e6dc-4e2e-8385-5721ef4dbfbc"></a>

###### 2.1.2.5.2.129 Field **migrated\_contapyme**

###### 2.1.2.5.2.129.1 **migrated\_contapyme** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>migrated_contapyme</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="ce87f866-1181-4d13-bac6-1223b8b9b565"></a>

###### 2.1.2.5.2.130 Field **gifts**

###### 2.1.2.5.2.130.1 **gifts** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#9d3de58c-cd02-4589-94f6-b06d7573747b class="margin-NaN">shippings</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.130.2 **gifts** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>gifts</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="9d3de58c-cd02-4589-94f6-b06d7573747b"></a>

###### 2.1.2.5.2.131 Field **shippings**

###### 2.1.2.5.2.131.1 **shippings** Hierarchy

Parent field: **gifts**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#04058119-8dbb-4b75-95d2-f800a75e9cf1 class="margin-NaN">quantity</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.131.2 **shippings** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shippings</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="04058119-8dbb-4b75-95d2-f800a75e9cf1"></a>

###### 2.1.2.5.2.132 Field **quantity**

###### 2.1.2.5.2.132.1 **quantity** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>quantity</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="3e0b8a6b-83b8-4ab9-b683-52b75476bccf"></a>

###### 2.1.2.5.2.133 Field **dropshipper**

###### 2.1.2.5.2.133.1 **dropshipper** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#dc739228-8da5-47c7-bdad-3be25da0fb30 class="margin-NaN">date_created</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#72c8ecdd-197d-433a-a1fc-ec65c7470c14 class="margin-NaN">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.133.2 **dropshipper** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dropshipper</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="dc739228-8da5-47c7-bdad-3be25da0fb30"></a>

###### 2.1.2.5.2.134 Field **date\_created**

###### 2.1.2.5.2.134.1 **date\_created** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>date_created</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer64</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1632411667000</td></tr></tbody></table>

### <a id="72c8ecdd-197d-433a-a1fc-ec65c7470c14"></a>

###### 2.1.2.5.2.135 Field **active**

###### 2.1.2.5.2.135.1 **active** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>active</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="286a2943-5d99-4afc-82ce-69a27f07e40a"></a>

###### 2.1.2.5.2.136 Field **last\_connection\_date**

###### 2.1.2.5.2.136.1 **last\_connection\_date** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#ca20987e-ca6f-4f10-a6da-117d23d91e78 class="margin-NaN">format</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#54938ef9-60d7-44af-a8f5-b3c680d1618b class="margin-NaN">unix</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.136.2 **last\_connection\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>last_connection_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="ca20987e-ca6f-4f10-a6da-117d23d91e78"></a>

###### 2.1.2.5.2.137 Field **format**

###### 2.1.2.5.2.137.1 **format** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>format</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>31/03/2025 20:43</td></tr></tbody></table>

### <a id="54938ef9-60d7-44af-a8f5-b3c680d1618b"></a>

###### 2.1.2.5.2.138 Field **unix**

###### 2.1.2.5.2.138.1 **unix** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>unix</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1743453783</td></tr></tbody></table>

### <a id="ae862b3a-9c19-4d1e-b45d-5e452b10aad2"></a>

###### 2.1.2.5.2.139 Field **ban**

###### 2.1.2.5.2.139.1 **ban** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#6b971885-76b9-4eaf-8263-79cca3a2f8f1 class="margin-NaN">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.139.2 **ban** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>ban</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="6b971885-76b9-4eaf-8263-79cca3a2f8f1"></a>

###### 2.1.2.5.2.140 Field **\[0\]**

###### 2.1.2.5.2.140.1 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Sample</td><td>shippings</td></tr></tbody></table>

### <a id="3c0cf2df-2f13-4bbc-85af-3c5817eb1a47"></a>

###### 2.1.2.5.2.141 Field **store\_information**

###### 2.1.2.5.2.141.1 **store\_information** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#0e1a57dc-5ddb-4922-a1ba-522e77af5d41 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7ed61ee0-e1bd-4e57-8048-3168a5d45382 class="margin-NaN">logo</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2fbbbdfd-e994-4b51-9973-5035cce8562d class="margin-NaN">banner</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.141.2 **store\_information** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>store_information</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="0e1a57dc-5ddb-4922-a1ba-522e77af5d41"></a>

###### 2.1.2.5.2.142 Field **name**

###### 2.1.2.5.2.142.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>test two drop 2</td></tr></tbody></table>

### <a id="7ed61ee0-e1bd-4e57-8048-3168a5d45382"></a>

###### 2.1.2.5.2.143 Field **logo**

###### 2.1.2.5.2.143.1 **logo** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>logo</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://shopping-rocketfy-uploads.s3.amazonaws.com/testtwodrop_804079258_121642999_10221463163479893_6069666320517077970_n44.jpg</td></tr></tbody></table>

### <a id="2fbbbdfd-e994-4b51-9973-5035cce8562d"></a>

###### 2.1.2.5.2.144 Field **banner**

###### 2.1.2.5.2.144.1 **banner** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>banner</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://shopping-rocketfy-uploads.s3.amazonaws.com/testtwodrop_804079258_image%20%281%29.png</td></tr></tbody></table>

### <a id="9cc332aa-ab42-4f43-873b-bec0a5c09936"></a>

###### 2.1.2.5.2.145 Field **blocked**

###### 2.1.2.5.2.145.1 **blocked** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>blocked</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="32f84f08-13b8-46f1-8c02-ea69b9432c80"></a>

###### 2.1.2.5.2.146 Field **enable\_fast\_withdraw**

###### 2.1.2.5.2.146.1 **enable\_fast\_withdraw** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>enable_fast_withdraw</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="c51aba41-3551-4d37-90c6-fc60ef63997f"></a>

###### 2.1.2.5.2.147 Field **indicative**

###### 2.1.2.5.2.147.1 **indicative** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>indicative</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>57</td></tr></tbody></table>

### <a id="cf930d30-6b47-4a5f-b4cc-fecd6f037a37"></a>

###### 2.1.2.5.2.148 Field **country\_ref**

###### 2.1.2.5.2.148.1 **country\_ref** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#25e3787b-c16e-4d9a-b163-f8cebf01f636 class="margin-NaN">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cbac59c3-47dd-4fbc-ba67-728b7b91c4c9 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3e7d9459-71c1-42db-ac3a-2752206815fb class="margin-NaN">iso2</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a739af0a-76a2-4b8f-893a-d3b830eb84de class="margin-NaN">iso3</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8f932e74-62fb-4ecd-a8d7-0ef8ae76ccf3 class="margin-NaN">flag_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#48166c67-25b5-4ef7-8237-4deda2715f78 class="margin-NaN">phone_code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.148.2 **country\_ref** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country_ref</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="25e3787b-c16e-4d9a-b163-f8cebf01f636"></a>

###### 2.1.2.5.2.149 Field **\_id**

###### 2.1.2.5.2.149.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="cbac59c3-47dd-4fbc-ba67-728b7b91c4c9"></a>

###### 2.1.2.5.2.150 Field **name**

###### 2.1.2.5.2.150.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Colombia</td></tr></tbody></table>

### <a id="3e7d9459-71c1-42db-ac3a-2752206815fb"></a>

###### 2.1.2.5.2.151 Field **iso2**

###### 2.1.2.5.2.151.1 **iso2** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>iso2</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>CO</td></tr></tbody></table>

### <a id="a739af0a-76a2-4b8f-893a-d3b830eb84de"></a>

###### 2.1.2.5.2.152 Field **iso3**

###### 2.1.2.5.2.152.1 **iso3** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>iso3</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>COL</td></tr></tbody></table>

### <a id="8f932e74-62fb-4ecd-a8d7-0ef8ae76ccf3"></a>

###### 2.1.2.5.2.153 Field **flag\_url**

###### 2.1.2.5.2.153.1 **flag\_url** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>flag_url</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://www.geonames.org/flags/x/co.gif</td></tr></tbody></table>

### <a id="48166c67-25b5-4ef7-8237-4deda2715f78"></a>

###### 2.1.2.5.2.154 Field **phone\_code**

###### 2.1.2.5.2.154.1 **phone\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>phone_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>57</td></tr></tbody></table>

### <a id="e4acc6e2-9421-4857-98ef-e42405e0394b"></a>

###### 2.1.2.5.2.155 Field **currency\_ref**

###### 2.1.2.5.2.155.1 **currency\_ref** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#c0ba7694-8fdf-4003-98fa-f2de1c0b70ac class="margin-NaN">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9030cd19-134a-4e10-a3c5-8c2798e71a5b class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#88d2b346-e65a-4d23-9f43-9cdcfabce142 class="margin-NaN">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2ed79b90-50ba-4212-bf46-dcd84e60c046 class="margin-NaN">htmlSymbol</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.155.2 **currency\_ref** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>currency_ref</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="c0ba7694-8fdf-4003-98fa-f2de1c0b70ac"></a>

###### 2.1.2.5.2.156 Field **\_id**

###### 2.1.2.5.2.156.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="9030cd19-134a-4e10-a3c5-8c2798e71a5b"></a>

###### 2.1.2.5.2.157 Field **name**

###### 2.1.2.5.2.157.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Peso Colombiano</td></tr></tbody></table>

### <a id="88d2b346-e65a-4d23-9f43-9cdcfabce142"></a>

###### 2.1.2.5.2.158 Field **code**

###### 2.1.2.5.2.158.1 **code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>COP</td></tr></tbody></table>

### <a id="2ed79b90-50ba-4212-bf46-dcd84e60c046"></a>

###### 2.1.2.5.2.159 Field **htmlSymbol**

###### 2.1.2.5.2.159.1 **htmlSymbol** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>htmlSymbol</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>&amp;#36;</td></tr></tbody></table>

### <a id="3cfe29b4-2eda-42cf-9560-4786ce790673"></a>

###### 2.1.2.5.2.160 Field **scoringWarehouseReputation**

###### 2.1.2.5.2.160.1 **scoringWarehouseReputation** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#e57f4172-d5bf-4b51-b16f-48fc3d2c398a class="margin-NaN">averageChatResponse</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a399d7a1-c18b-49f0-a2e6-a2643344a3bd class="margin-NaN">averageChatResponseScore</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#311e7f61-6036-40d0-8430-cdae5fbb7cd3 class="margin-NaN">averageGuideTime</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#783dddde-6ac8-4267-8552-e11551e9c3a1 class="margin-NaN">averageGuideTimeScore</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#056d21dd-4129-45e0-8ca0-436c7064189b class="margin-NaN">cancellationRate</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#948610c7-848c-46ad-a28d-2ed8450bbff6 class="margin-NaN">cancellationRateScore</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e74777ec-92c6-406d-a8de-05bf5c75e75b class="margin-NaN">final_score</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.160.2 **scoringWarehouseReputation** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>scoringWarehouseReputation</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="e57f4172-d5bf-4b51-b16f-48fc3d2c398a"></a>

###### 2.1.2.5.2.161 Field **averageChatResponse**

###### 2.1.2.5.2.161.1 **averageChatResponse** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>averageChatResponse</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="a399d7a1-c18b-49f0-a2e6-a2643344a3bd"></a>

###### 2.1.2.5.2.162 Field **averageChatResponseScore**

###### 2.1.2.5.2.162.1 **averageChatResponseScore** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>averageChatResponseScore</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="311e7f61-6036-40d0-8430-cdae5fbb7cd3"></a>

###### 2.1.2.5.2.163 Field **averageGuideTime**

###### 2.1.2.5.2.163.1 **averageGuideTime** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>averageGuideTime</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="783dddde-6ac8-4267-8552-e11551e9c3a1"></a>

###### 2.1.2.5.2.164 Field **averageGuideTimeScore**

###### 2.1.2.5.2.164.1 **averageGuideTimeScore** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>averageGuideTimeScore</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="056d21dd-4129-45e0-8ca0-436c7064189b"></a>

###### 2.1.2.5.2.165 Field **cancellationRate**

###### 2.1.2.5.2.165.1 **cancellationRate** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cancellationRate</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>11.11</td></tr></tbody></table>

### <a id="948610c7-848c-46ad-a28d-2ed8450bbff6"></a>

###### 2.1.2.5.2.166 Field **cancellationRateScore**

###### 2.1.2.5.2.166.1 **cancellationRateScore** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cancellationRateScore</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>3</td></tr></tbody></table>

### <a id="e74777ec-92c6-406d-a8de-05bf5c75e75b"></a>

###### 2.1.2.5.2.167 Field **final\_score**

###### 2.1.2.5.2.167.1 **final\_score** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>final_score</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1</td></tr></tbody></table>

### <a id="3d1716a5-ab96-45bf-9dc4-7b17926766f0"></a>

###### 2.1.2.5.2.168 Field **subscription**

###### 2.1.2.5.2.168.1 **subscription** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#0eaf622f-9636-4538-af61-065ba8917c83 class="margin-NaN">plan</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c3312a13-2184-4385-bd2c-a46ba85f2a40 class="margin-NaN">remainingShipments</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d66853ac-3a1b-446b-82f7-6fad8ab01c8d class="margin-NaN">expiresAt</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ac4ba03d-0e49-4572-8a31-089dc6e41361 class="margin-NaN">isActive</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#13cbd748-952c-484d-9cbb-92334765ab3c class="margin-NaN">paymentMethodId</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.168.2 **subscription** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>subscription</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="0eaf622f-9636-4538-af61-065ba8917c83"></a>

###### 2.1.2.5.2.169 Field **plan**

###### 2.1.2.5.2.169.1 **plan** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>plan</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>free</td></tr></tbody></table>

### <a id="c3312a13-2184-4385-bd2c-a46ba85f2a40"></a>

###### 2.1.2.5.2.170 Field **remainingShipments**

###### 2.1.2.5.2.170.1 **remainingShipments** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>remainingShipments</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>15</td></tr></tbody></table>

### <a id="d66853ac-3a1b-446b-82f7-6fad8ab01c8d"></a>

###### 2.1.2.5.2.171 Field **expiresAt**

###### 2.1.2.5.2.171.1 **expiresAt** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>expiresAt</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ac4ba03d-0e49-4572-8a31-089dc6e41361"></a>

###### 2.1.2.5.2.172 Field **isActive**

###### 2.1.2.5.2.172.1 **isActive** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>isActive</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="13cbd748-952c-484d-9cbb-92334765ab3c"></a>

###### 2.1.2.5.2.173 Field **paymentMethodId**

###### 2.1.2.5.2.173.1 **paymentMethodId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>paymentMethodId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

###### 2.1.2.5.3 **customers** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">dbname_1</td><td class="table-column-property">wallet_-1</td><td class="table-column-property">billing_-1</td><td class="table-column-property">slug_-1</td><td class="table-column-property">warehouse.has_shared_products_-1_last_connection_date.unix_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">dbname_1</td><td class="table-column-indexes">wallet_-1</td><td class="table-column-indexes">billing_-1</td><td class="table-column-indexes">slug_-1</td><td class="table-column-indexes">warehouse.has_shared_products_-1_last_connection_date.unix_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">dbname('ascending')</td><td class="table-column-indexes"></td><td class="table-column-indexes">billing('descending')</td><td class="table-column-indexes">slug('descending')</td><td class="table-column-indexes">has_shared_products('descending'), unix('descending')</td></tr></tbody></table>

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">domain_-1</td><td class="table-column-property">_id_</td><td class="table-column-property">email_-1</td><td class="table-column-property">country_ref.iso3_-1</td><td class="table-column-property">warehouse.has_shared_products_1_warehouse.only_my_stores_1_last_connection_date.unix_1_scoring.horas_despacho_1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">domain_-1</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">email_-1</td><td class="table-column-indexes">country_ref.iso3_-1</td><td class="table-column-indexes">warehouse.has_shared_products_1_warehouse.only_my_stores_1_last_connection_date.unix_1_scoring.horas_despacho_1</td></tr><tr><td>Key</td><td class="table-column-indexes"></td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">email('descending')</td><td class="table-column-indexes">iso3('descending')</td><td class="table-column-indexes">has_shared_products('ascending'), unix('ascending')</td></tr></tbody></table>

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">warehouse.verified_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">warehouse.verified_-1</td></tr></tbody></table>

### <a id="9e7d9462-9ccb-449b-a053-38685a5f26cd"></a>

##### 2.1.2.6 Collection **unified\_products**

###### 2.1.2.6.1 **unified\_products** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>unified_products</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#6f94401a-8e31-4b31-9268-15061668a1b5><span class="name-container">rocketfy</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.6.2 **unified\_products** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#c2e733ac-c363-4663-b0da-e9a912d3b521 class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7fe1d3f5-2828-4c9e-978a-a54d10f6d4ae class="margin-0">establishment_identifier</a></td><td class="no-break-word">string</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bd963db3-9434-4930-ab98-d1b7d7b3915b class="margin-0">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f7c9dc3d-a5ef-4b19-b3b2-24f2b892b9d4 class="margin-0">type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c47e2221-02b8-422f-b72c-13eeb5125f13 class="margin-0">short_description</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f3220f80-caa1-46ae-9392-710d66971b79 class="margin-0">description</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dd82c179-795a-4065-8945-b2a1b9993b2d class="margin-0">price</a></td><td class="no-break-word">numeric,string,null</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ad1dd102-57fd-4f44-b8db-0f87aa267f85 class="margin-0">sku</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#15988e8a-0439-4291-8228-0f66872f5d7d class="margin-0">slug</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#572823dd-2ba4-4614-beb7-b2c272524c53 class="margin-0">visible</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ab7a6f64-7b25-41f1-b691-3c19020c2f41 class="margin-0">imagePrin</a></td><td class="no-break-word">document,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f5723ce9-8f40-49f7-92ea-3a12d9e738f8 class="margin-5">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0d01b890-d401-4135-aba4-21da0aa215ce class="margin-10">fieldname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0c34ef4b-a2d6-4a32-acd7-087e3be93b1c class="margin-10">originalname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#22967070-8f87-479f-a068-548e39667939 class="margin-10">encoding</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#46d61eb9-36a8-41ba-95d3-f0939a98615d class="margin-10">mimetype</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fd06f01b-0582-4ce2-84be-75755c234341 class="margin-10">size</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1c7af080-4a50-463e-a82b-94ffa2fa0bcd class="margin-10">bucket</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a2e480e2-f9cb-45a8-9868-103f4ba5ba49 class="margin-10">key</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#de0ca1e9-c5cf-494c-a8d0-6260f4d8c427 class="margin-10">acl</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#78e2282a-3a7d-47ae-8590-18c34f1e4c41 class="margin-10">contentType</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c29be43b-5e54-4720-8fdc-b6092c4aeff6 class="margin-10">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#631e71e5-6a40-4421-a400-0abb94b5c904 class="margin-10">contentEncoding</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#453c36d8-3832-48b4-860b-c8e38cab5a83 class="margin-10">storageClass</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#032d95a5-805f-4f24-8c59-ff690858ff17 class="margin-10">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#74dfae74-ef96-45b7-924a-3d832f87f3ee class="margin-10">metadata</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#38a59508-a6e6-4ff9-a026-5c96c89b5417 class="margin-15">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fbafb570-bba1-4a36-ada5-606318f6ef43 class="margin-15">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8a8ac9e1-364d-495b-80b8-0b253d663a8a class="margin-10">location</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4816e825-4ec2-4d22-8797-8b3e0e7ae8cd class="margin-10">etag</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e0862985-60e0-476b-88b8-8a348b703796 class="margin-10">versionId</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1582e5a2-525f-4843-8cab-4a32010e6d4f class="margin-10">principal</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#71057d69-c002-4459-a700-c6fc8d35755c class="margin-10">status</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#840867ac-7462-4a2c-aab1-e5c3108e4bc1 class="margin-10">url</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#56db0781-c00f-4564-b69f-2176419d1046 class="margin-0">images</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3b5aed89-50c3-430c-809b-6368497374d5 class="margin-5">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c686f935-2740-4d8b-9fc2-46b8585af7f0 class="margin-10">fieldname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c738dd4c-4e43-47a4-9003-1abae7350014 class="margin-10">originalname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#101b5017-8330-4ea6-94b0-5b9b50862bc2 class="margin-10">encoding</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5cc3b613-86a7-4444-b852-691ddeaf8b93 class="margin-10">mimetype</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#54535582-370b-4546-b7c0-6933a4faeb52 class="margin-10">size</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5620c2eb-2333-4260-b2ac-83bdc218458b class="margin-10">bucket</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e1cc1a56-56b0-4440-9084-0141e18cf0d3 class="margin-10">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#289944cd-6f27-4022-bc80-0c165f72a44b class="margin-10">acl</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#887e2027-7bd3-4275-acfb-18af7c01a3ed class="margin-10">contentType</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#153fbd33-b5a8-42f7-af71-01e559837999 class="margin-10">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0bf0e4c2-e11c-4327-a8e2-e54b2a2fa0ff class="margin-10">contentEncoding</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#aaf9958a-ff86-48f6-9a8f-46e7e13a6c42 class="margin-10">storageClass</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#555fe820-63d0-4dcb-936b-9f430e7858d7 class="margin-10">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3a2cc99a-80c9-4b13-ab36-d5505468163a class="margin-10">metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#31f03e24-0737-4cf1-a088-81c52c78f850 class="margin-15">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ba81aa85-1fcc-4d97-a4e2-7e64493ad105 class="margin-15">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0709ef35-5346-4a2c-993a-cdab6632d44a class="margin-10">location</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#886283ea-66e7-44cb-8a09-a13062813cd1 class="margin-10">etag</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e841836f-60dc-42ef-a06a-975c300041ad class="margin-10">versionId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ae066e94-2e30-44dc-a0fe-a19ee72f26b3 class="margin-10">principal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6fe99682-df35-485a-a2ac-8c5ca5c8866f class="margin-10">status</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a93c0437-1a40-4f52-9e6e-f2866e425e39 class="margin-10">url</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#42b2bf3a-f812-48a1-a913-7880d714045a class="margin-0">created_time</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2ea922c1-1214-4d52-82e3-666ab2d6cc81 class="margin-0">attributes</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#179632ee-411d-4d24-94d7-1c61e20d24cc class="margin-5">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#08f2224d-59b3-4c45-8170-ced5917c06ee class="margin-10">checked</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4ea6e8f1-151c-47cf-a30a-d2fea8e2acfa class="margin-10">id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1b9e8856-58e6-4174-965d-418b418523ff class="margin-10">items</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#04f74a6f-3076-4545-b746-49dbbae97aa5 class="margin-15">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e832363c-24b8-4436-bf84-e9c56bff258f class="margin-20">checked</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cbef175b-2641-4eab-881c-dba19174ba3c class="margin-20">id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1eaed199-b89d-4d80-b123-6164f8860846 class="margin-20">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8e3b1294-82f7-4ad7-89f1-2706ebdfc6e8 class="margin-10">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a555f9d3-8d93-4684-9f6d-d8d7d9169917 class="margin-10">subname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#52bfa870-b5a9-44cd-97c9-95f82ac920f8 class="margin-0">variations</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c59a1fab-d614-4876-900f-97173b597049 class="margin-5">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4865ea6b-5409-4d44-8708-ab6f4965806e class="margin-10">establishment_identifier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f8acffc8-769b-4713-ae33-d525e050fb49 class="margin-10">inventory_id</a></td><td class="no-break-word">string,objectId</td><td>true</td><td>dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#398a2f96-3430-4213-b233-a4520be52909 class="margin-10">product_id</a></td><td class="no-break-word">string,objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c89b7285-1934-4f50-8fcd-ad9318016a79 class="margin-10">created_time</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6f9afe6c-0b35-483d-aff9-d45623c0a24d class="margin-10">variation_id</a></td><td class="no-break-word">string,null,array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#abebda3a-28d1-4414-b1f8-14175dd45cb5 class="margin-15">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0ed9d24d-ce31-4bd4-9cbe-76b722380f62 class="margin-20">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e101a458-2558-4ba3-82f3-58807a7c2102 class="margin-25">attr_id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#088b14b8-9b02-4120-9e1b-90a77a40ea17 class="margin-25">attr_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f3feba5c-581f-4286-922f-cc92da29af11 class="margin-25">id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0f0066fe-54f7-479f-9594-2447634e210a class="margin-25">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#14d330b0-6fb5-4bbc-9001-92519038780a class="margin-10">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#42ad854e-4022-4853-a8fd-020047e41c60 class="margin-10">sku</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0f7b9cf8-d23d-426d-87bb-dcd235a5f967 class="margin-10">price</a></td><td class="no-break-word">numeric,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ead153dc-8aa9-4937-b239-b8da3764a414 class="margin-10">image</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c37a7bcd-bc64-4344-a9df-a8ebb8b9f4b3 class="margin-10">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cbd508ea-c129-4c8e-a9af-0c813cf17c64 class="margin-10">props</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5960bdb5-fe5f-4d90-ab4b-6d4bfdf979e2 class="margin-15">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bf958466-3b5a-44ce-84ce-0dbc55be690f class="margin-20">id</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#db2a854a-aba7-4148-a633-82791de76b2d class="margin-20">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#50f7c782-7862-4a3d-95cd-3348d75a69ec class="margin-20">attr_id</a></td><td class="no-break-word">integer64</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b4d058a1-97f0-4788-9c47-2a1674010be5 class="margin-20">attr_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#50425cca-d753-4c4e-b00f-35e77a329f3d class="margin-10">quantity</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3db8b469-67f6-4984-be67-c8e18f1e40fe class="margin-10">_id</a></td><td class="no-break-word">string,objectId</td><td>true</td><td>dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c1076876-cd9b-46ab-b508-0de2dd46ce3a class="margin-10">cost</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ca122f41-8063-4d21-ba30-5a29659b99f6 class="margin-10">dropshipper_price</a></td><td class="no-break-word">numeric,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#95518af7-8089-452d-a1c1-9c8962405c90 class="margin-10">id</a></td><td class="no-break-word">string,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d9d2f444-64ce-4172-8a92-5bfa4be2f835 class="margin-10">isValidForm</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8c0e102d-d3b9-4de4-a3a9-11d4acb853db class="margin-10">profit</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#59fa553a-1dab-4d86-8ecd-b80d69984bd1 class="margin-10">shopify_variant_id</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#79b1be1a-9713-4a68-858f-5bdef15837fd class="margin-10">warehouse_price</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e14e4034-60da-44c8-988f-b6b61cc82274 class="margin-10">woo_variant_id</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7243c27a-250b-425b-ae09-72302109974b class="margin-0">dimensions</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4a888b99-dc04-4630-820b-9f86901e2924 class="margin-5">width</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#673990aa-44ab-488a-b096-fad4fabb3923 class="margin-5">height</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#50a7f458-fa57-45fd-b2e7-282cf4c0cbf6 class="margin-5">large</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#02498d75-d2e6-4fd1-a53a-57abc98a38f1 class="margin-5">weight</a></td><td class="no-break-word">double</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#13b29a06-b616-437e-9fb1-d380df8721a1 class="margin-5">weight_unit</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8cd8373a-c742-450c-af35-2ef1e566306c class="margin-5">weight_in_unit</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d55107f9-4c71-45f7-8631-22cad9d61e09 class="margin-5">volume</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#261c6bf7-55dd-41c9-a945-08becb5a4768 class="margin-0">metadata</a></td><td class="no-break-word">array,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#94bf96ba-09ef-4497-ba1a-dc249771d8f0 class="margin-5">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3d3f46c8-19a3-4bb2-9833-c494566aec4c class="margin-0">free_shipping</a></td><td class="no-break-word">boolean,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#06ad3d4b-16e2-49ee-8ecf-b87e30d988f8 class="margin-0">category_id</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#55c6af7a-5289-4d30-8e88-b4071c8785ac class="margin-5">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#122cb18d-7b57-4023-9d51-948ed46f9e7f class="margin-5">name</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#aed38f15-3584-4d7c-8a6e-c9dc6f28cfa7 class="margin-0">category</a></td><td class="no-break-word">document,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#57cdd698-979f-4852-a8bc-4135c9c893ba class="margin-5">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c91f4b13-769c-41c8-bbbb-7d4490f9d989 class="margin-10">_id</a></td><td class="no-break-word">objectId,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#79a276ac-88f1-493c-a182-f5869d769e0e class="margin-10">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1e4b5c1e-6f2f-434d-8e8f-0da97a8fee49 class="margin-10">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#04469280-4a2d-4e5a-9c8b-d9afee432c3d class="margin-10">category_father</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8e0ffb1c-0a91-484f-b0d5-2c754ac0f593 class="margin-10">path_from_root</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#432b6d58-e2fb-43ff-9a46-3ef52843bdac class="margin-15">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2de57d55-9f3e-456a-b82d-e0bbffcfaed3 class="margin-20">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d2660199-c7fa-464b-96cd-aca76cfd5543 class="margin-20">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#62322fb0-913f-4187-a17b-4d2ef2fd6900 class="margin-10">children_categories</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6b2cffb5-952c-49a5-9236-8028a2d508c9 class="margin-15">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1734d25f-a2bf-4449-9366-623d0f69ac33 class="margin-20">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#82cbdf12-378a-4332-92d5-ef605d7c8e9b class="margin-20">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5cbe5b44-18fc-4318-8897-a9ec2f73d1cf class="margin-10">settings</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c6ef5842-8ac4-48df-9c7d-81ad11b99dfd class="margin-15">adult_content</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dfd0b5b8-018c-49d1-add6-b0829a4ca80b class="margin-15">fragile</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c4c5f436-97cb-4f58-96ca-d1993adabe48 class="margin-15">status</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#59280c2e-b823-423b-a282-989fa1714895 class="margin-15">currencies</a></td><td class="no-break-word">array</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#08e14ce9-3367-42fa-ae97-4b321cea86c5 class="margin-20">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0c02c5a2-a8b8-42f4-aa04-f34c67b078c9 class="margin-15">inmediate_payment</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cf7d8e94-1c9f-4235-a148-10ddc4a1dea2 class="margin-15">items_review_allowed</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e761427f-4b52-45be-b232-2ed00a9c6ae7 class="margin-15">listing_allowed</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2fe6d910-e7ae-4969-803c-e80cd9ed9b4a class="margin-15">max_description_length</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c64ce533-cbaf-4ca1-90d5-139cb244e123 class="margin-15">max_pictures_per_item</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7c346327-bd82-410d-bc58-0a782291f701 class="margin-15">max_pictures_per_item_var</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5841fc12-ba0f-44e2-a3be-65163143da9e class="margin-15">max_sub_title_length</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bd8b7d40-e35c-4e40-a3e3-19e5c2b2ad8a class="margin-15">max_title_length</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7858c557-11f9-4dd8-9e5e-cd78ab1a017c class="margin-15">maximum_price</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dec9ef3a-0cdf-47f1-98a9-ea5be11546ef class="margin-15">maximum_price_currency</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#54d7e874-ece5-4f35-8d40-ed558fa97cb0 class="margin-15">minimum_price</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5f0a6210-dde0-4c7d-a2d1-f814a91741fe class="margin-15">minimum_price_currency</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a827e458-921a-4afb-b448-be3c5d73915e class="margin-15">sat_product_code_mexico</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#59e812a3-ff28-46b2-ba3f-0a13a2c72c12 class="margin-15">sat_product_description_mexico</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#599d0478-2466-444e-a153-e8f44fec14b5 class="margin-15">seller_contact</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5d55bd13-8be2-414a-aa4f-7373586044d2 class="margin-10">country</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e05be836-4250-4593-a414-ca2a17cda55e class="margin-10">date_created</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#615881a6-c7d6-405f-bb94-d275b5609a7f class="margin-10">permalink</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0e889ec9-4927-4c39-b707-e58e25a8e955 class="margin-10">picture</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c75e6333-afa2-4c68-8438-0e6763a7942c class="margin-0">warranty</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9bee1cfe-0b40-44dc-8b5a-e5bd377e0551 class="margin-0">warranty_description</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ad4d5f9a-09fd-46c4-95f8-24eda3d77d0d class="margin-0">country_ref</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fd2fe4a1-6806-45e2-aa00-add083b683b2 class="margin-5">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f384f56f-30e5-406b-89f3-60ccd30e53d5 class="margin-5">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5b74f234-d47e-4aef-8d97-eae19adf0143 class="margin-5">iso2</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#48ff6ffc-d5f1-4ef3-acf9-a7554ad1bb49 class="margin-5">iso3</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ac51ee37-90a9-47e2-853c-c1cfdf8716bb class="margin-5">flag_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#501e81e4-6013-4d5d-91be-f5382f70520e class="margin-5">phone_code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cc4b35b6-8f54-43ed-a4a4-fac9ec5e1af3 class="margin-0">shared</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#24696a36-7a61-4cef-bf7d-43dd68caf232 class="margin-0">disabled</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a2bb589d-72b9-486c-81ce-46cab7afac87 class="margin-0">disabled_by_inactivity</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6cc02d56-0a5c-47e1-8678-6a3ebc71ed97 class="margin-0">dropshipper</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ed046033-2ebc-4716-94a7-05161132e010 class="margin-5">data</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d511caa6-7a72-48aa-9f60-5bd926221a62 class="margin-10">db_importer</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#31ea1152-0af5-47d3-ac25-64e767c3b923 class="margin-10">shop</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d386ded4-5918-4156-b663-c09d38b8ea6e class="margin-15">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#53db87e4-1b13-4d1d-a7f5-bee112a930d2 class="margin-15">carry</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#42707f3f-f30a-432e-83a1-4ffe1e6dac4d class="margin-15">cc_nit</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#57bde019-33ba-49c3-a0f4-d3f332bda31d class="margin-15">city</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ac8ac35b-8e21-45d5-b31f-354d8fc194ba class="margin-20">_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#be7e564c-a031-4e8f-9fb9-ffcd252c83e8 class="margin-20">before_courrier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8be037db-2863-403e-9556-4df1d59c7e66 class="margin-20">checked</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bc159314-81ae-4e54-ba0d-c8561f540c1a class="margin-20">city_code</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0b705d40-a8d0-40c0-bbd1-b91bd8b1021f class="margin-20">cod_depto</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e234c789-3272-423c-b8af-2471cd674241 class="margin-20">country</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3a80fa46-e603-4ce5-9e07-4b28876e84a6 class="margin-25">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ec61a93e-eac0-47a3-b3d3-8633098378bb class="margin-25">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d3398ba5-31c1-467b-81de-7833b478bf45 class="margin-25">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e145bb01-2f7b-4600-a3e8-febb7e1932cb class="margin-20">courrier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#109f30e6-6db0-4f70-b04f-b49f2135e0ac class="margin-20">dane_code</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7d725b85-a38c-4ffa-87b2-71edd7626db2 class="margin-25">rocketfy</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#59acfc1c-58f1-4bfb-99db-124595c59a33 class="margin-25">servientrega</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8018c9ec-be4c-4513-ab84-e8289bc1ae20 class="margin-20">disabled</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f732cc36-9392-44c7-87d7-49a4901a2ceb class="margin-20">forTest</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#da6d497a-b825-40f8-b01e-5192f94c74f1 class="margin-20">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7566ba06-5df9-4ac0-83d2-4af15b1433d3 class="margin-20">postal_code</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5684cd81-4be5-4d93-9981-192e4ac50dd4 class="margin-20">shipping_zone</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2989c74b-8893-4e26-bfd7-18cb235bc5cd class="margin-20">shop_error</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c594be0d-1559-4dc5-8014-0608af88b916 class="margin-20">state</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#65d27686-c1a7-4293-803c-bcf5f91eff89 class="margin-25">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#45fd203a-2362-4983-ad2e-e00a5366ad1e class="margin-25">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#46c250e3-3071-4ad6-8e2b-53331aa96f72 class="margin-25">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2bcdec1a-b328-46e8-a92b-4313e6aae9c2 class="margin-15">cod_postal</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f902f797-78a6-4ac0-9d6d-a52714cd667e class="margin-15">color_primary</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#24e86e8a-18d9-46b4-a1e7-3ec2720b3669 class="margin-15">colors</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#abdc360f-ab50-4a6a-9704-74fadb316583 class="margin-20">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c431ab09-6d31-4e86-8591-fe9f80f47376 class="margin-15">composed_address</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cc382011-090f-4b5f-aef1-efb8d34f9d8e class="margin-20">street</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7f7eefc7-df9f-43b8-92c8-3259b1ebd62c class="margin-20">street_number_one</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#84d49e59-0005-42de-b99d-1c00286d1d58 class="margin-20">street_number_two</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1270cf9c-273c-4b2e-b7f1-f3a4c9f941dc class="margin-15">country</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#021a2d22-e241-4272-b12f-b52b3a3dda19 class="margin-15">default</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b4fa7d4b-101c-4a79-8b96-9bb0f0f29d6f class="margin-15">departament</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5f4bb39d-24a9-42c3-9d6b-e0a0d613d180 class="margin-20">_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3c92b036-0857-43f2-8614-9aa53e451fac class="margin-20">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#787a542c-2165-4ae1-ab6e-e2ed80432422 class="margin-20">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ec25ddb8-f978-4042-ba18-a8463127ba57 class="margin-15">email</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f9dcb654-2ce8-4eb0-a2fc-59061c84b473 class="margin-15">geolocation</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1949d2aa-32aa-426c-a71a-e533c464b4fd class="margin-20">lat</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f39f9f4f-2e64-47c8-b2ad-0e9635032675 class="margin-20">lng</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6bedeab5-eb49-4d7f-82ee-22b705c3da8b class="margin-15">gtag</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1f1786a6-0de8-4b38-9a5c-1d692e79f850 class="margin-15">indicative</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8b8bcc68-b8a7-4902-a833-ee8ef2ede116 class="margin-15">large_description</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a5fd1468-2377-46ad-941d-d210a1a2a3e1 class="margin-15">location</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a1df519e-c6f4-4eba-aec9-f3c2940d4e6e class="margin-15">logo</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b3c0819e-6f40-417b-b5c7-e3a2fe8c41b2 class="margin-20">acl</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#04effb38-cf40-45c7-bf6c-107c189d4d9e class="margin-20">bucket</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2af742fa-448e-4ceb-9385-1488deb95e7b class="margin-20">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ef2089e0-46b1-49f6-b9d8-ae5eb53b8e87 class="margin-20">contentType</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#80d77e22-e039-4a97-984b-c1f2351e3f25 class="margin-20">created_time</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#52776beb-8dbd-4c68-ab5e-132924ab7595 class="margin-20">encoding</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0bd9dded-efe2-4263-bc79-49bb5db42ba1 class="margin-20">etag</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#87ed7b42-0652-40b6-8baa-1e240b1c851b class="margin-20">fieldname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#64441011-5f81-4522-97f8-1f0c4b1114db class="margin-20">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8b15faed-b0be-4ce2-9e18-65b4f2d3ecee class="margin-20">location</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8f8c28d7-ed1c-4ab5-a2ce-d7455d2e7bf4 class="margin-20">metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#118d626c-9743-46cf-9fbf-b1d5f5773484 class="margin-25">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#144191bf-86f7-4dad-9b11-59a5c624d91c class="margin-25">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#12cc603f-b035-4cde-92af-959334c4381e class="margin-20">mimetype</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c33db1b9-5c63-4975-8a86-77c874419702 class="margin-20">originalname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a886a177-68e8-4195-9d3b-1be51ccc3329 class="margin-20">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7d11e2b5-8661-4549-bfa8-1d23cad1f932 class="margin-20">size</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cdd97757-348d-47fd-b719-707a07f6fd0b class="margin-20">storageClass</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ca481b70-ad59-40de-9b1d-eeea3cca4ee9 class="margin-20">versionId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#64e15efc-a5f9-44c2-860c-467e739e5f2c class="margin-15">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#39b25ba9-5273-469f-b839-b62d8aadb2dd class="margin-15">neighborhood</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0c1313fd-ac32-4d4e-a18d-41568d219f6b class="margin-15">pixel</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6d279947-e770-4e79-bf50-6b595e5e1226 class="margin-15">principal_address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f9b21e85-e979-4eba-a29d-23b67eb3e1ca class="margin-15">promises</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d7f97ab6-3f18-4866-967f-8c9166a9342e class="margin-15">slogan</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fedf2777-e165-4cf9-943e-69e4adee81a2 class="margin-5">id_import</a></td><td class="no-break-word">string,objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6df057f3-3814-44b9-8170-1c542fbdbb64 class="margin-5">price</a></td><td class="no-break-word">numeric,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1a45535a-ba4a-49ff-ac38-89394c1590ea class="margin-0">import</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1ac5492c-d5aa-48ef-acf1-9284fbd10746 class="margin-0">shared_metadata</a></td><td class="no-break-word">document,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e5742997-2997-4328-80db-0b5f71b1cb22 class="margin-5">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9b3f0b4c-d6f8-417b-a39a-588ff0ede9f2 class="margin-10">shared_with</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f7711907-5827-4db9-819c-a1cf3f2d5e3c class="margin-0">shopify_product_id</a></td><td class="no-break-word">integer64</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#30437f95-1a0d-4bd1-ba56-1cd3e6b7a3e3 class="margin-0">shopify_product_name</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2717c1bb-7c90-4fbf-83e9-dd8afc75b765 class="margin-0">total_inventory</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6ab0ea65-e90e-4d69-82cc-d81a41b8c1d6 class="margin-0">warehouse</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e3e80165-9918-41df-9dd2-f8172e31ee28 class="margin-5">data</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#40e0d521-5a00-4d48-8fc5-ba250a311d09 class="margin-10">db_seller</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e796a6d9-8ac4-4396-8114-f4f11d73a92a class="margin-10">dbname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e4e0e0a6-adef-449d-b73a-cccb5c92784f class="margin-10">only_my_stores</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c4f2fc88-2a62-47b0-a2da-56ce5d8f35fe class="margin-10">shop</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7e65a5b1-d939-4514-bbab-697f2f2bc641 class="margin-15">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#06baa3ae-54c1-4999-ac14-0bca778dfb4a class="margin-15">carry</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2a1582dd-0b38-40e3-a8df-67a9c04c77a5 class="margin-15">cc_nit</a></td><td class="no-break-word">string,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6cd874cb-eed3-40c3-b240-273886a7ca63 class="margin-15">city</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9220dfbf-c565-4bde-a064-0c8fd7d977ab class="margin-20">_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#960d825f-91e9-48e5-b94a-9782a1765c51 class="margin-20">before_courrier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bb02387e-1f4d-44d1-b7c6-818d9db2c14f class="margin-20">checked</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0c05791e-a90b-4f50-9a0c-8bd29cf38d96 class="margin-20">city_code</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#61af89b2-cf58-4cc3-a7bb-417fe514c747 class="margin-20">cod_depto</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5b72ebd5-fa6a-4b97-80b8-e8e7ddbf8c1e class="margin-20">country</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f2b0518c-81f1-423c-999b-d06c8b6cbc4e class="margin-25">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#63165f1e-9e7e-4179-8bff-1889c8e74d90 class="margin-25">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ce12c088-65a8-4dbc-8b98-5b9a0a73de42 class="margin-25">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bd457df8-4c80-4ce6-a9fa-ec3934b43e45 class="margin-20">courrier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#169ce543-ea82-4f94-b5cf-58f6d32c30e6 class="margin-20">dane_code</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7348ec48-4648-4cd5-8038-5dee6679a70a class="margin-25">rocketfy</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0aa56542-2d12-41a2-ad8d-5f393f954867 class="margin-25">servientrega</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9dc4af32-93b4-4e47-9106-1e37d583d081 class="margin-20">disabled</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#898dbe2f-51d2-4710-b61b-40d1758bfc98 class="margin-20">forTest</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#615ddf5c-583b-4b87-9bfe-72f0b55c022c class="margin-20">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#05e715c5-0117-46ed-9f07-e5f27bec947c class="margin-20">postal_code</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#84d87f6d-6d6a-410c-98e2-a55ccf12fd3a class="margin-20">shipping_zone</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cd4d3097-8e0d-43ee-9e7e-3026da264318 class="margin-20">shop_error</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1b109b23-f5db-491d-8426-0331e6545fba class="margin-20">state</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#611a4139-1328-46ff-b487-6f630f3c8947 class="margin-25">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#09084d0d-ad82-4c08-8eaa-6cf784e7b1dc class="margin-25">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#79262244-802b-4918-b0b2-6cd6d8629f12 class="margin-25">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f10c9485-46bd-422e-a784-1d230161e2dc class="margin-15">cod_postal</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7cd4c528-9939-4840-849d-5addea177080 class="margin-15">color_primary</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#033149d2-bab4-4f3e-9f7a-4993f4522e68 class="margin-15">colors</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4ece7366-6291-455f-a769-f9afa0ca5712 class="margin-20">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ffc29497-3bc3-4c25-b1e5-4247ecc08740 class="margin-15">composed_address</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4aa1b272-4188-440f-b02a-d70f826eb269 class="margin-20">street</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9f912897-2bba-40fc-84f5-f10901eb5c85 class="margin-20">street_number_one</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#661cbb86-5e92-4ab2-9052-56aff6284552 class="margin-20">street_number_two</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0e75cc1c-bccc-4ae7-80f7-72b72ebf05e4 class="margin-15">country</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#686a0002-75b0-40aa-9a37-d84fab3c0ff4 class="margin-15">default</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#36e281d5-2127-4119-8084-691285e03899 class="margin-15">departament</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#813e50ab-c900-4e0b-be26-4c2b46126366 class="margin-20">_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#46ecf093-6038-4d7d-ba5b-5eeb2055d500 class="margin-20">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#08a01672-1f13-4ec7-a1e9-25659f4039db class="margin-20">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fcbc1d2b-7348-4a8b-b6cb-4dfb1d0f080c class="margin-15">email</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#967dfd8e-7118-492a-8c76-12962d552f52 class="margin-15">geolocation</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4d3e176f-7470-43f9-9b86-3945033fa12d class="margin-20">lat</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3299679b-dfcd-45fc-9d81-4a6f3c6cdbdb class="margin-20">lng</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f93ba1c6-00a0-4291-bf24-955562564b0e class="margin-15">gtag</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7ca8d788-bcee-49ad-a16f-45838a54b984 class="margin-15">horary</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#30cc4162-3cc2-4faa-8184-c01eb7e6c6c4 class="margin-20">final_horary</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8a0c69bd-2938-47ee-a682-576c48273550 class="margin-25">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c8c085ae-3616-4f71-a7e6-5be133b66623 class="margin-25">value</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d51cd821-c3b4-4e55-af0b-6f6708054bb7 class="margin-20">init_horary</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5803505b-a05f-4f02-bae7-2cfe80b89204 class="margin-25">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e8abbaeb-5674-4a5f-b9d1-1e7755868c21 class="margin-25">value</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f93e272d-e34e-41b8-b809-ce5171cce55b class="margin-15">indicative</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2e23ea77-eeae-49c1-b721-52f84300224e class="margin-15">large_description</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6c807e3c-8853-4be0-a7f9-7b177de01270 class="margin-15">location</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#550f09fb-b9bd-434c-8b96-b145a9cba7e7 class="margin-20">lat</a></td><td class="no-break-word">double</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2484af52-eabb-49ef-a3a3-4916ebf1a1fa class="margin-20">lng</a></td><td class="no-break-word">double</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#42b69d98-d5e7-4c25-9331-42f750589b0e class="margin-15">logo</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#980c4dce-931c-4713-8ee6-ca1794ffd26f class="margin-20">acl</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cf525fe7-1634-4206-a1c0-4a4ac1a700b4 class="margin-20">bucket</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#763f18e3-3ae3-4d3e-9cbc-881801103852 class="margin-20">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ef9220da-7eb6-46d4-b634-4a8664761019 class="margin-20">contentType</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#19e499c1-0b11-453b-9bca-6dda8f019a62 class="margin-20">created_time</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b817ddc3-485b-4117-a8fb-3fbaeeac9594 class="margin-20">encoding</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#075f14be-43df-4a76-89e8-ed8c7afa0053 class="margin-20">etag</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6aeb826d-248e-41fa-b08b-ff0d33a278e9 class="margin-20">fieldname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#29975f23-cff6-4c35-a239-679ad7ab4b3f class="margin-20">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b78587fc-5d41-49ea-8482-bc13d09e7dce class="margin-20">location</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9fef7e49-239e-49e1-a665-6fae0b443467 class="margin-20">metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dace8dad-78f0-474d-87b6-a1ebfe1e5245 class="margin-25">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#502a48b0-dcb0-4fa4-b9fd-d0b25de63778 class="margin-25">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cc625345-5009-4946-b616-ced89f6c768a class="margin-20">mimetype</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#084bdb92-951c-4d99-9f81-502e94529e4c class="margin-20">originalname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#47755034-235c-4bdc-af2a-7382a21e7cbc class="margin-20">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a78607c9-ad68-4265-a665-3d37ca123ddf class="margin-20">size</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#23f0e8e4-7ba6-445f-92e6-2528ba397b41 class="margin-20">storageClass</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ed64d430-c645-4d46-97b1-0b7ba3595348 class="margin-20">versionId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8e0795ca-dfe8-4865-b0c5-78e80af5bceb class="margin-15">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5a4be2ef-7c85-4be7-b056-1f4f6002a48c class="margin-15">neighborhood</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#519b049e-99dc-4ecf-9bdf-0cb1bf91a944 class="margin-15">pixel</a></td><td class="no-break-word">null,numeric,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#efd5e92b-a342-4742-a637-58785888a51e class="margin-15">principal_address</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2cf05f1b-5a17-426d-96c8-72bd5b8fbea3 class="margin-15">promises</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ca285719-ebd6-45b1-a009-bedefbab25c5 class="margin-15">slogan</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e4833a55-6ffa-444d-b5f8-25bb963c7ac1 class="margin-5">discount</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ec4b24ec-6e02-41e2-b768-277b867f10ac class="margin-5">father_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5acbdc17-e081-451b-9bdf-f178c35a0957 class="margin-5">id_father</a></td><td class="no-break-word">objectId,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2ce8cfe5-7729-4a36-9d08-796df8e480e7 class="margin-5">id_warehouse_rkf</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b78b79b5-d8d0-4160-916e-55990a4b6a1e class="margin-5">price</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7a3c1a5a-20a4-44ec-8cd1-cda7074c257b class="margin-5">product_warehouse_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c26de8d5-fb08-4487-89bc-8ad70bed6583 class="margin-5">shared_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ab139950-43ab-4d15-b847-51a630f15b2d class="margin-5">shipping</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#84e943fd-416c-4dcf-a01f-144c4d2c76fa class="margin-5">statistics</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#97702d1f-e38a-416e-b4e1-2ae5ff7c7751 class="margin-10">imports</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a1843152-e4bb-4614-b126-795c939abbee class="margin-10">sales</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#26e58736-bd32-481b-b724-78b129d4d6ff class="margin-5">store_price_equal_to_suggested_price</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#59e1e32e-4c39-466d-b357-335bd36b8bc0 class="margin-5">suggested</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ffbcc644-29cd-4006-9e02-d0195d70308e class="margin-5">suggested_price</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#666cbe97-7e43-45b1-bdc6-d56436e5eb43 class="margin-5">suggestions</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c2952542-ed1e-471a-8fc9-78544e99d250 class="margin-5">visible</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#72045e1a-dbdb-45cf-a66c-f0d060be17fa class="margin-5">warehouse_price</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a2d3d7c3-e6dc-4a85-9876-3fe1aa2ae0ab class="margin-0">woo_product_id</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#205be59b-4145-4848-8e62-2defdcf046d4 class="margin-0">woo_product_name</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="c2e733ac-c363-4663-b0da-e9a912d3b521"></a>

###### 2.1.2.6.2.1 Field **\_id**

###### 2.1.2.6.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="7fe1d3f5-2828-4c9e-978a-a54d10f6d4ae"></a>

###### 2.1.2.6.2.2 Field **establishment\_identifier**

###### 2.1.2.6.2.2.1 **establishment\_identifier** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>establishment_identifier</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#ec559fb7-4dbc-4d80-912e-a1628c5130b4>customers</a></td></tr><tr><td>Foreign field</td><td><a href=#7fa9b648-96f2-4145-b5c0-11a173cd0b0e>dbname</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr><tr><td>Sample</td><td>rocketfy_customer_testtwodrop_804079258</td></tr></tbody></table>

### <a id="bd963db3-9434-4930-ab98-d1b7d7b3915b"></a>

###### 2.1.2.6.2.3 Field **name**

###### 2.1.2.6.2.3.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>asfasfasf</td></tr></tbody></table>

### <a id="f7c9dc3d-a5ef-4b19-b3b2-24f2b892b9d4"></a>

###### 2.1.2.6.2.4 Field **type**

###### 2.1.2.6.2.4.1 **type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>variable</td></tr></tbody></table>

### <a id="c47e2221-02b8-422f-b72c-13eeb5125f13"></a>

###### 2.1.2.6.2.5 Field **short\_description**

###### 2.1.2.6.2.5.1 **short\_description** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>short_description</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="f3220f80-caa1-46ae-9392-710d66971b79"></a>

###### 2.1.2.6.2.6 Field **description**

###### 2.1.2.6.2.6.1 **description** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>description</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="dd82c179-795a-4065-8945-b2a1b9993b2d"></a>

###### 2.1.2.6.2.7 Field **price**

###### 2.1.2.6.2.7.1 **price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,string,null)</td></tr><tr><td></td><td>[object Object],[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ad1dd102-57fd-4f44-b8db-0f87aa267f85"></a>

###### 2.1.2.6.2.8 Field **sku**

###### 2.1.2.6.2.8.1 **sku** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>sku</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="15988e8a-0439-4291-8228-0f66872f5d7d"></a>

###### 2.1.2.6.2.9 Field **slug**

###### 2.1.2.6.2.9.1 **slug** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>slug</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>asfasfasf</td></tr></tbody></table>

### <a id="572823dd-2ba4-4614-beb7-b2c272524c53"></a>

###### 2.1.2.6.2.10 Field **visible**

###### 2.1.2.6.2.10.1 **visible** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>visible</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="ab7a6f64-7b25-41f1-b691-3c19020c2f41"></a>

###### 2.1.2.6.2.11 Field **imagePrin**

###### 2.1.2.6.2.11.1 **imagePrin** Hierarchy

Parent field: **unified\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#f5723ce9-8f40-49f7-92ea-3a12d9e738f8 class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.11.2 **imagePrin** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>imagePrin</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (document,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="f5723ce9-8f40-49f7-92ea-3a12d9e738f8"></a>

###### 2.1.2.6.2.12 Field **properties**

###### 2.1.2.6.2.12.1 **properties** Hierarchy

Parent field: **imagePrin**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#0d01b890-d401-4135-aba4-21da0aa215ce class="margin-NaN">fieldname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0c34ef4b-a2d6-4a32-acd7-087e3be93b1c class="margin-NaN">originalname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#22967070-8f87-479f-a068-548e39667939 class="margin-NaN">encoding</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#46d61eb9-36a8-41ba-95d3-f0939a98615d class="margin-NaN">mimetype</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fd06f01b-0582-4ce2-84be-75755c234341 class="margin-NaN">size</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1c7af080-4a50-463e-a82b-94ffa2fa0bcd class="margin-NaN">bucket</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a2e480e2-f9cb-45a8-9868-103f4ba5ba49 class="margin-NaN">key</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#de0ca1e9-c5cf-494c-a8d0-6260f4d8c427 class="margin-NaN">acl</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#78e2282a-3a7d-47ae-8590-18c34f1e4c41 class="margin-NaN">contentType</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c29be43b-5e54-4720-8fdc-b6092c4aeff6 class="margin-NaN">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#631e71e5-6a40-4421-a400-0abb94b5c904 class="margin-NaN">contentEncoding</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#453c36d8-3832-48b4-860b-c8e38cab5a83 class="margin-NaN">storageClass</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#032d95a5-805f-4f24-8c59-ff690858ff17 class="margin-NaN">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#74dfae74-ef96-45b7-924a-3d832f87f3ee class="margin-NaN">metadata</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8a8ac9e1-364d-495b-80b8-0b253d663a8a class="margin-NaN">location</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4816e825-4ec2-4d22-8797-8b3e0e7ae8cd class="margin-NaN">etag</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e0862985-60e0-476b-88b8-8a348b703796 class="margin-NaN">versionId</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1582e5a2-525f-4843-8cab-4a32010e6d4f class="margin-NaN">principal</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#71057d69-c002-4459-a700-c6fc8d35755c class="margin-NaN">status</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#840867ac-7462-4a2c-aab1-e5c3108e4bc1 class="margin-NaN">url</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.12.2 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="0d01b890-d401-4135-aba4-21da0aa215ce"></a>

###### 2.1.2.6.2.13 Field **fieldname**

###### 2.1.2.6.2.13.1 **fieldname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="0c34ef4b-a2d6-4a32-acd7-087e3be93b1c"></a>

###### 2.1.2.6.2.14 Field **originalname**

###### 2.1.2.6.2.14.1 **originalname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>originalname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="22967070-8f87-479f-a068-548e39667939"></a>

###### 2.1.2.6.2.15 Field **encoding**

###### 2.1.2.6.2.15.1 **encoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>encoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="46d61eb9-36a8-41ba-95d3-f0939a98615d"></a>

###### 2.1.2.6.2.16 Field **mimetype**

###### 2.1.2.6.2.16.1 **mimetype** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mimetype</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="fd06f01b-0582-4ce2-84be-75755c234341"></a>

###### 2.1.2.6.2.17 Field **size**

###### 2.1.2.6.2.17.1 **size** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>size</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="1c7af080-4a50-463e-a82b-94ffa2fa0bcd"></a>

###### 2.1.2.6.2.18 Field **bucket**

###### 2.1.2.6.2.18.1 **bucket** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>bucket</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a2e480e2-f9cb-45a8-9868-103f4ba5ba49"></a>

###### 2.1.2.6.2.19 Field **key**

###### 2.1.2.6.2.19.1 **key** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>key</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="de0ca1e9-c5cf-494c-a8d0-6260f4d8c427"></a>

###### 2.1.2.6.2.20 Field **acl**

###### 2.1.2.6.2.20.1 **acl** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>acl</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="78e2282a-3a7d-47ae-8590-18c34f1e4c41"></a>

###### 2.1.2.6.2.21 Field **contentType**

###### 2.1.2.6.2.21.1 **contentType** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentType</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c29be43b-5e54-4720-8fdc-b6092c4aeff6"></a>

###### 2.1.2.6.2.22 Field **contentDisposition**

###### 2.1.2.6.2.22.1 **contentDisposition** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentDisposition</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="631e71e5-6a40-4421-a400-0abb94b5c904"></a>

###### 2.1.2.6.2.23 Field **contentEncoding**

###### 2.1.2.6.2.23.1 **contentEncoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentEncoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="453c36d8-3832-48b4-860b-c8e38cab5a83"></a>

###### 2.1.2.6.2.24 Field **storageClass**

###### 2.1.2.6.2.24.1 **storageClass** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>storageClass</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="032d95a5-805f-4f24-8c59-ff690858ff17"></a>

###### 2.1.2.6.2.25 Field **serverSideEncryption**

###### 2.1.2.6.2.25.1 **serverSideEncryption** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>serverSideEncryption</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="74dfae74-ef96-45b7-924a-3d832f87f3ee"></a>

###### 2.1.2.6.2.26 Field **metadata**

###### 2.1.2.6.2.26.1 **metadata** Hierarchy

Parent field: **properties**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#38a59508-a6e6-4ff9-a026-5c96c89b5417 class="margin-NaN">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fbafb570-bba1-4a36-ada5-606318f6ef43 class="margin-NaN">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.26.2 **metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="38a59508-a6e6-4ff9-a026-5c96c89b5417"></a>

###### 2.1.2.6.2.27 Field **fieldName**

###### 2.1.2.6.2.27.1 **fieldName** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldName</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="fbafb570-bba1-4a36-ada5-606318f6ef43"></a>

###### 2.1.2.6.2.28 Field **Content-Type**

###### 2.1.2.6.2.28.1 **Content-Type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Content-Type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8a8ac9e1-364d-495b-80b8-0b253d663a8a"></a>

###### 2.1.2.6.2.29 Field **location**

###### 2.1.2.6.2.29.1 **location** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>location</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4816e825-4ec2-4d22-8797-8b3e0e7ae8cd"></a>

###### 2.1.2.6.2.30 Field **etag**

###### 2.1.2.6.2.30.1 **etag** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>etag</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="e0862985-60e0-476b-88b8-8a348b703796"></a>

###### 2.1.2.6.2.31 Field **versionId**

###### 2.1.2.6.2.31.1 **versionId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>versionId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="1582e5a2-525f-4843-8cab-4a32010e6d4f"></a>

###### 2.1.2.6.2.32 Field **principal**

###### 2.1.2.6.2.32.1 **principal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>principal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="71057d69-c002-4459-a700-c6fc8d35755c"></a>

###### 2.1.2.6.2.33 Field **status**

###### 2.1.2.6.2.33.1 **status** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>status</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="840867ac-7462-4a2c-aab1-e5c3108e4bc1"></a>

###### 2.1.2.6.2.34 Field **url**

###### 2.1.2.6.2.34.1 **url** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>url</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="56db0781-c00f-4564-b69f-2176419d1046"></a>

###### 2.1.2.6.2.35 Field **images**

###### 2.1.2.6.2.35.1 **images** Hierarchy

Parent field: **unified\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#3b5aed89-50c3-430c-809b-6368497374d5 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.35.2 **images** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>images</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="3b5aed89-50c3-430c-809b-6368497374d5"></a>

###### 2.1.2.6.2.36 Field **\[0\]**

###### 2.1.2.6.2.36.1 **\[0\]** Hierarchy

Parent field: **images**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#c686f935-2740-4d8b-9fc2-46b8585af7f0 class="margin-NaN">fieldname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c738dd4c-4e43-47a4-9003-1abae7350014 class="margin-NaN">originalname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#101b5017-8330-4ea6-94b0-5b9b50862bc2 class="margin-NaN">encoding</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5cc3b613-86a7-4444-b852-691ddeaf8b93 class="margin-NaN">mimetype</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#54535582-370b-4546-b7c0-6933a4faeb52 class="margin-NaN">size</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5620c2eb-2333-4260-b2ac-83bdc218458b class="margin-NaN">bucket</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e1cc1a56-56b0-4440-9084-0141e18cf0d3 class="margin-NaN">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#289944cd-6f27-4022-bc80-0c165f72a44b class="margin-NaN">acl</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#887e2027-7bd3-4275-acfb-18af7c01a3ed class="margin-NaN">contentType</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#153fbd33-b5a8-42f7-af71-01e559837999 class="margin-NaN">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0bf0e4c2-e11c-4327-a8e2-e54b2a2fa0ff class="margin-NaN">contentEncoding</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#aaf9958a-ff86-48f6-9a8f-46e7e13a6c42 class="margin-NaN">storageClass</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#555fe820-63d0-4dcb-936b-9f430e7858d7 class="margin-NaN">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3a2cc99a-80c9-4b13-ab36-d5505468163a class="margin-NaN">metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0709ef35-5346-4a2c-993a-cdab6632d44a class="margin-NaN">location</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#886283ea-66e7-44cb-8a09-a13062813cd1 class="margin-NaN">etag</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e841836f-60dc-42ef-a06a-975c300041ad class="margin-NaN">versionId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ae066e94-2e30-44dc-a0fe-a19ee72f26b3 class="margin-NaN">principal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6fe99682-df35-485a-a2ac-8c5ca5c8866f class="margin-NaN">status</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a93c0437-1a40-4f52-9e6e-f2866e425e39 class="margin-NaN">url</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.36.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="c686f935-2740-4d8b-9fc2-46b8585af7f0"></a>

###### 2.1.2.6.2.37 Field **fieldname**

###### 2.1.2.6.2.37.1 **fieldname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="c738dd4c-4e43-47a4-9003-1abae7350014"></a>

###### 2.1.2.6.2.38 Field **originalname**

###### 2.1.2.6.2.38.1 **originalname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>originalname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>producto-con-precio-alto-test-two-drop-1082362823.jpg</td></tr></tbody></table>

### <a id="101b5017-8330-4ea6-94b0-5b9b50862bc2"></a>

###### 2.1.2.6.2.39 Field **encoding**

###### 2.1.2.6.2.39.1 **encoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>encoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>7bit</td></tr></tbody></table>

### <a id="5cc3b613-86a7-4444-b852-691ddeaf8b93"></a>

###### 2.1.2.6.2.40 Field **mimetype**

###### 2.1.2.6.2.40.1 **mimetype** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mimetype</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="54535582-370b-4546-b7c0-6933a4faeb52"></a>

###### 2.1.2.6.2.41 Field **size**

###### 2.1.2.6.2.41.1 **size** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>size</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>433743</td></tr></tbody></table>

### <a id="5620c2eb-2333-4260-b2ac-83bdc218458b"></a>

###### 2.1.2.6.2.42 Field **bucket**

###### 2.1.2.6.2.42.1 **bucket** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>bucket</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>shopping-rocketfy-uploads</td></tr></tbody></table>

### <a id="e1cc1a56-56b0-4440-9084-0141e18cf0d3"></a>

###### 2.1.2.6.2.43 Field **key**

###### 2.1.2.6.2.43.1 **key** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>key</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>producto-con-precio-alto-test-two-drop-1082362823.jpg</td></tr></tbody></table>

### <a id="289944cd-6f27-4022-bc80-0c165f72a44b"></a>

###### 2.1.2.6.2.44 Field **acl**

###### 2.1.2.6.2.44.1 **acl** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>acl</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>public-read</td></tr></tbody></table>

### <a id="887e2027-7bd3-4275-acfb-18af7c01a3ed"></a>

###### 2.1.2.6.2.45 Field **contentType**

###### 2.1.2.6.2.45.1 **contentType** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentType</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="153fbd33-b5a8-42f7-af71-01e559837999"></a>

###### 2.1.2.6.2.46 Field **contentDisposition**

###### 2.1.2.6.2.46.1 **contentDisposition** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentDisposition</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="0bf0e4c2-e11c-4327-a8e2-e54b2a2fa0ff"></a>

###### 2.1.2.6.2.47 Field **contentEncoding**

###### 2.1.2.6.2.47.1 **contentEncoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentEncoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="aaf9958a-ff86-48f6-9a8f-46e7e13a6c42"></a>

###### 2.1.2.6.2.48 Field **storageClass**

###### 2.1.2.6.2.48.1 **storageClass** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>storageClass</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>STANDARD</td></tr></tbody></table>

### <a id="555fe820-63d0-4dcb-936b-9f430e7858d7"></a>

###### 2.1.2.6.2.49 Field **serverSideEncryption**

###### 2.1.2.6.2.49.1 **serverSideEncryption** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>serverSideEncryption</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="3a2cc99a-80c9-4b13-ab36-d5505468163a"></a>

###### 2.1.2.6.2.50 Field **metadata**

###### 2.1.2.6.2.50.1 **metadata** Hierarchy

Parent field: **\[0\]**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#31f03e24-0737-4cf1-a088-81c52c78f850 class="margin-NaN">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ba81aa85-1fcc-4d97-a4e2-7e64493ad105 class="margin-NaN">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.50.2 **metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="31f03e24-0737-4cf1-a088-81c52c78f850"></a>

###### 2.1.2.6.2.51 Field **fieldName**

###### 2.1.2.6.2.51.1 **fieldName** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldName</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="ba81aa85-1fcc-4d97-a4e2-7e64493ad105"></a>

###### 2.1.2.6.2.52 Field **Content-Type**

###### 2.1.2.6.2.52.1 **Content-Type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Content-Type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="0709ef35-5346-4a2c-993a-cdab6632d44a"></a>

###### 2.1.2.6.2.53 Field **location**

###### 2.1.2.6.2.53.1 **location** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>location</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://s3-uploads.rocketfy.co/producto-con-precio-alto-test-two-drop-1082362823.jpg</td></tr></tbody></table>

### <a id="886283ea-66e7-44cb-8a09-a13062813cd1"></a>

###### 2.1.2.6.2.54 Field **etag**

###### 2.1.2.6.2.54.1 **etag** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>etag</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>"a8496b7adf1c77cf2e3701d916a7e148"</td></tr></tbody></table>

### <a id="e841836f-60dc-42ef-a06a-975c300041ad"></a>

###### 2.1.2.6.2.55 Field **versionId**

###### 2.1.2.6.2.55.1 **versionId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>versionId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>kTaDCFESdH55UhfJxZ_IkcbOdpaRYpcx</td></tr></tbody></table>

### <a id="ae066e94-2e30-44dc-a0fe-a19ee72f26b3"></a>

###### 2.1.2.6.2.56 Field **principal**

###### 2.1.2.6.2.56.1 **principal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>principal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="6fe99682-df35-485a-a2ac-8c5ca5c8866f"></a>

###### 2.1.2.6.2.57 Field **status**

###### 2.1.2.6.2.57.1 **status** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>status</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a93c0437-1a40-4f52-9e6e-f2866e425e39"></a>

###### 2.1.2.6.2.58 Field **url**

###### 2.1.2.6.2.58.1 **url** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>url</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="42b2bf3a-f812-48a1-a913-7880d714045a"></a>

###### 2.1.2.6.2.59 Field **created\_time**

###### 2.1.2.6.2.59.1 **created\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1731094800</td></tr></tbody></table>

### <a id="2ea922c1-1214-4d52-82e3-666ab2d6cc81"></a>

###### 2.1.2.6.2.60 Field **attributes**

###### 2.1.2.6.2.60.1 **attributes** Hierarchy

Parent field: **unified\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#179632ee-411d-4d24-94d7-1c61e20d24cc class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.60.2 **attributes** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>attributes</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="179632ee-411d-4d24-94d7-1c61e20d24cc"></a>

###### 2.1.2.6.2.61 Field **\[0\]**

###### 2.1.2.6.2.61.1 **\[0\]** Hierarchy

Parent field: **attributes**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#08f2224d-59b3-4c45-8170-ced5917c06ee class="margin-NaN">checked</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4ea6e8f1-151c-47cf-a30a-d2fea8e2acfa class="margin-NaN">id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1b9e8856-58e6-4174-965d-418b418523ff class="margin-NaN">items</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8e3b1294-82f7-4ad7-89f1-2706ebdfc6e8 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a555f9d3-8d93-4684-9f6d-d8d7d9169917 class="margin-NaN">subname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.61.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="08f2224d-59b3-4c45-8170-ced5917c06ee"></a>

###### 2.1.2.6.2.62 Field **checked**

###### 2.1.2.6.2.62.1 **checked** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>checked</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4ea6e8f1-151c-47cf-a30a-d2fea8e2acfa"></a>

###### 2.1.2.6.2.63 Field **id**

###### 2.1.2.6.2.63.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="1b9e8856-58e6-4174-965d-418b418523ff"></a>

###### 2.1.2.6.2.64 Field **items**

###### 2.1.2.6.2.64.1 **items** Hierarchy

Parent field: **\[0\]**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#04f74a6f-3076-4545-b746-49dbbae97aa5 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.64.2 **items** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>items</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="04f74a6f-3076-4545-b746-49dbbae97aa5"></a>

###### 2.1.2.6.2.65 Field **\[0\]**

###### 2.1.2.6.2.65.1 **\[0\]** Hierarchy

Parent field: **items**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#e832363c-24b8-4436-bf84-e9c56bff258f class="margin-NaN">checked</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cbef175b-2641-4eab-881c-dba19174ba3c class="margin-NaN">id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1eaed199-b89d-4d80-b123-6164f8860846 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.65.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="e832363c-24b8-4436-bf84-e9c56bff258f"></a>

###### 2.1.2.6.2.66 Field **checked**

###### 2.1.2.6.2.66.1 **checked** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>checked</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="cbef175b-2641-4eab-881c-dba19174ba3c"></a>

###### 2.1.2.6.2.67 Field **id**

###### 2.1.2.6.2.67.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="1eaed199-b89d-4d80-b123-6164f8860846"></a>

###### 2.1.2.6.2.68 Field **name**

###### 2.1.2.6.2.68.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8e3b1294-82f7-4ad7-89f1-2706ebdfc6e8"></a>

###### 2.1.2.6.2.69 Field **name**

###### 2.1.2.6.2.69.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a555f9d3-8d93-4684-9f6d-d8d7d9169917"></a>

###### 2.1.2.6.2.70 Field **subname**

###### 2.1.2.6.2.70.1 **subname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>subname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="52bfa870-b5a9-44cd-97c9-95f82ac920f8"></a>

###### 2.1.2.6.2.71 Field **variations**

###### 2.1.2.6.2.71.1 **variations** Hierarchy

Parent field: **unified\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#c59a1fab-d614-4876-900f-97173b597049 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.71.2 **variations** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>variations</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="c59a1fab-d614-4876-900f-97173b597049"></a>

###### 2.1.2.6.2.72 Field **\[0\]**

###### 2.1.2.6.2.72.1 **\[0\]** Hierarchy

Parent field: **variations**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#4865ea6b-5409-4d44-8708-ab6f4965806e class="margin-NaN">establishment_identifier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f8acffc8-769b-4713-ae33-d525e050fb49 class="margin-NaN">inventory_id</a></td><td class="no-break-word">string,objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#398a2f96-3430-4213-b233-a4520be52909 class="margin-NaN">product_id</a></td><td class="no-break-word">string,objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c89b7285-1934-4f50-8fcd-ad9318016a79 class="margin-NaN">created_time</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6f9afe6c-0b35-483d-aff9-d45623c0a24d class="margin-NaN">variation_id</a></td><td class="no-break-word">string,null,array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#14d330b0-6fb5-4bbc-9001-92519038780a class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#42ad854e-4022-4853-a8fd-020047e41c60 class="margin-NaN">sku</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0f7b9cf8-d23d-426d-87bb-dcd235a5f967 class="margin-NaN">price</a></td><td class="no-break-word">numeric,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ead153dc-8aa9-4937-b239-b8da3764a414 class="margin-NaN">image</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c37a7bcd-bc64-4344-a9df-a8ebb8b9f4b3 class="margin-NaN">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cbd508ea-c129-4c8e-a9af-0c813cf17c64 class="margin-NaN">props</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#50425cca-d753-4c4e-b00f-35e77a329f3d class="margin-NaN">quantity</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3db8b469-67f6-4984-be67-c8e18f1e40fe class="margin-NaN">_id</a></td><td class="no-break-word">string,objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c1076876-cd9b-46ab-b508-0de2dd46ce3a class="margin-NaN">cost</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ca122f41-8063-4d21-ba30-5a29659b99f6 class="margin-NaN">dropshipper_price</a></td><td class="no-break-word">numeric,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#95518af7-8089-452d-a1c1-9c8962405c90 class="margin-NaN">id</a></td><td class="no-break-word">string,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d9d2f444-64ce-4172-8a92-5bfa4be2f835 class="margin-NaN">isValidForm</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8c0e102d-d3b9-4de4-a3a9-11d4acb853db class="margin-NaN">profit</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#59fa553a-1dab-4d86-8ecd-b80d69984bd1 class="margin-NaN">shopify_variant_id</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#79b1be1a-9713-4a68-858f-5bdef15837fd class="margin-NaN">warehouse_price</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e14e4034-60da-44c8-988f-b6b61cc82274 class="margin-NaN">woo_variant_id</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.72.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="4865ea6b-5409-4d44-8708-ab6f4965806e"></a>

###### 2.1.2.6.2.73 Field **establishment\_identifier**

###### 2.1.2.6.2.73.1 **establishment\_identifier** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>establishment_identifier</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>rocketfy_customer_testtwodrop_804079258</td></tr></tbody></table>

### <a id="f8acffc8-769b-4713-ae33-d525e050fb49"></a>

###### 2.1.2.6.2.74 Field **inventory\_id**

###### 2.1.2.6.2.74.1 **inventory\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>inventory_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,objectId)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="398a2f96-3430-4213-b233-a4520be52909"></a>

###### 2.1.2.6.2.75 Field **product\_id**

###### 2.1.2.6.2.75.1 **product\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>product_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,objectId)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c89b7285-1934-4f50-8fcd-ad9318016a79"></a>

###### 2.1.2.6.2.76 Field **created\_time**

###### 2.1.2.6.2.76.1 **created\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1731094800</td></tr></tbody></table>

### <a id="6f9afe6c-0b35-483d-aff9-d45623c0a24d"></a>

###### 2.1.2.6.2.77 Field **variation\_id**

###### 2.1.2.6.2.77.1 **variation\_id** Hierarchy

Parent field: **\[0\]**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#abebda3a-28d1-4414-b1f8-14175dd45cb5 class="margin-NaN">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.77.2 **variation\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>variation_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null,array)</td></tr><tr><td></td><td>[object Object],[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="abebda3a-28d1-4414-b1f8-14175dd45cb5"></a>

###### 2.1.2.6.2.78 Field **items**

###### 2.1.2.6.2.78.1 **items** Hierarchy

Parent field: **variation\_id**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#0ed9d24d-ce31-4bd4-9cbe-76b722380f62 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.78.2 **items** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="0ed9d24d-ce31-4bd4-9cbe-76b722380f62"></a>

###### 2.1.2.6.2.79 Field **\[0\]**

###### 2.1.2.6.2.79.1 **\[0\]** Hierarchy

Parent field: **items**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#e101a458-2558-4ba3-82f3-58807a7c2102 class="margin-NaN">attr_id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#088b14b8-9b02-4120-9e1b-90a77a40ea17 class="margin-NaN">attr_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f3feba5c-581f-4286-922f-cc92da29af11 class="margin-NaN">id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0f0066fe-54f7-479f-9594-2447634e210a class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.79.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="e101a458-2558-4ba3-82f3-58807a7c2102"></a>

###### 2.1.2.6.2.80 Field **attr\_id**

###### 2.1.2.6.2.80.1 **attr\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>attr_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="088b14b8-9b02-4120-9e1b-90a77a40ea17"></a>

###### 2.1.2.6.2.81 Field **attr\_name**

###### 2.1.2.6.2.81.1 **attr\_name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>attr_name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="f3feba5c-581f-4286-922f-cc92da29af11"></a>

###### 2.1.2.6.2.82 Field **id**

###### 2.1.2.6.2.82.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="0f0066fe-54f7-479f-9594-2447634e210a"></a>

###### 2.1.2.6.2.83 Field **name**

###### 2.1.2.6.2.83.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="14d330b0-6fb5-4bbc-9001-92519038780a"></a>

###### 2.1.2.6.2.84 Field **name**

###### 2.1.2.6.2.84.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Producto con precio alto</td></tr></tbody></table>

### <a id="42ad854e-4022-4853-a8fd-020047e41c60"></a>

###### 2.1.2.6.2.85 Field **sku**

###### 2.1.2.6.2.85.1 **sku** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>sku</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>PR-10</td></tr></tbody></table>

### <a id="0f7b9cf8-d23d-426d-87bb-dcd235a5f967"></a>

###### 2.1.2.6.2.86 Field **price**

###### 2.1.2.6.2.86.1 **price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ead153dc-8aa9-4937-b239-b8da3764a414"></a>

###### 2.1.2.6.2.87 Field **image**

###### 2.1.2.6.2.87.1 **image** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>image</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c37a7bcd-bc64-4344-a9df-a8ebb8b9f4b3"></a>

###### 2.1.2.6.2.88 Field **active**

###### 2.1.2.6.2.88.1 **active** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>active</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="cbd508ea-c129-4c8e-a9af-0c813cf17c64"></a>

###### 2.1.2.6.2.89 Field **props**

###### 2.1.2.6.2.89.1 **props** Hierarchy

Parent field: **\[0\]**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#5960bdb5-fe5f-4d90-ab4b-6d4bfdf979e2 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.89.2 **props** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>props</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="5960bdb5-fe5f-4d90-ab4b-6d4bfdf979e2"></a>

###### 2.1.2.6.2.90 Field **\[0\]**

###### 2.1.2.6.2.90.1 **\[0\]** Hierarchy

Parent field: **props**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#bf958466-3b5a-44ce-84ce-0dbc55be690f class="margin-NaN">id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#db2a854a-aba7-4148-a633-82791de76b2d class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#50f7c782-7862-4a3d-95cd-3348d75a69ec class="margin-NaN">attr_id</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b4d058a1-97f0-4788-9c47-2a1674010be5 class="margin-NaN">attr_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.90.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="bf958466-3b5a-44ce-84ce-0dbc55be690f"></a>

###### 2.1.2.6.2.91 Field **id**

###### 2.1.2.6.2.91.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>771899800</td></tr></tbody></table>

### <a id="db2a854a-aba7-4148-a633-82791de76b2d"></a>

###### 2.1.2.6.2.92 Field **name**

###### 2.1.2.6.2.92.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Producto con precio alto</td></tr></tbody></table>

### <a id="50f7c782-7862-4a3d-95cd-3348d75a69ec"></a>

###### 2.1.2.6.2.93 Field **attr\_id**

###### 2.1.2.6.2.93.1 **attr\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>attr_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer64</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>725095205051581</td></tr></tbody></table>

### <a id="b4d058a1-97f0-4788-9c47-2a1674010be5"></a>

###### 2.1.2.6.2.94 Field **attr\_name**

###### 2.1.2.6.2.94.1 **attr\_name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>attr_name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Producto</td></tr></tbody></table>

### <a id="50425cca-d753-4c4e-b00f-35e77a329f3d"></a>

###### 2.1.2.6.2.95 Field **quantity**

###### 2.1.2.6.2.95.1 **quantity** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>quantity</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="3db8b469-67f6-4984-be67-c8e18f1e40fe"></a>

###### 2.1.2.6.2.96 Field **\_id**

###### 2.1.2.6.2.96.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,objectId)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c1076876-cd9b-46ab-b508-0de2dd46ce3a"></a>

###### 2.1.2.6.2.97 Field **cost**

###### 2.1.2.6.2.97.1 **cost** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cost</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ca122f41-8063-4d21-ba30-5a29659b99f6"></a>

###### 2.1.2.6.2.98 Field **dropshipper\_price**

###### 2.1.2.6.2.98.1 **dropshipper\_price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dropshipper_price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="95518af7-8089-452d-a1c1-9c8962405c90"></a>

###### 2.1.2.6.2.99 Field **id**

###### 2.1.2.6.2.99.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="d9d2f444-64ce-4172-8a92-5bfa4be2f835"></a>

###### 2.1.2.6.2.100 Field **isValidForm**

###### 2.1.2.6.2.100.1 **isValidForm** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>isValidForm</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8c0e102d-d3b9-4de4-a3a9-11d4acb853db"></a>

###### 2.1.2.6.2.101 Field **profit**

###### 2.1.2.6.2.101.1 **profit** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>profit</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="59fa553a-1dab-4d86-8ecd-b80d69984bd1"></a>

###### 2.1.2.6.2.102 Field **shopify\_variant\_id**

###### 2.1.2.6.2.102.1 **shopify\_variant\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shopify_variant_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="79b1be1a-9713-4a68-858f-5bdef15837fd"></a>

###### 2.1.2.6.2.103 Field **warehouse\_price**

###### 2.1.2.6.2.103.1 **warehouse\_price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>warehouse_price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="e14e4034-60da-44c8-988f-b6b61cc82274"></a>

###### 2.1.2.6.2.104 Field **woo\_variant\_id**

###### 2.1.2.6.2.104.1 **woo\_variant\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>woo_variant_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="7243c27a-250b-425b-ae09-72302109974b"></a>

###### 2.1.2.6.2.105 Field **dimensions**

###### 2.1.2.6.2.105.1 **dimensions** Hierarchy

Parent field: **unified\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#4a888b99-dc04-4630-820b-9f86901e2924 class="margin-NaN">width</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#673990aa-44ab-488a-b096-fad4fabb3923 class="margin-NaN">height</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#50a7f458-fa57-45fd-b2e7-282cf4c0cbf6 class="margin-NaN">large</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#02498d75-d2e6-4fd1-a53a-57abc98a38f1 class="margin-NaN">weight</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#13b29a06-b616-437e-9fb1-d380df8721a1 class="margin-NaN">weight_unit</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8cd8373a-c742-450c-af35-2ef1e566306c class="margin-NaN">weight_in_unit</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d55107f9-4c71-45f7-8631-22cad9d61e09 class="margin-NaN">volume</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.105.2 **dimensions** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dimensions</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="4a888b99-dc04-4630-820b-9f86901e2924"></a>

###### 2.1.2.6.2.106 Field **width**

###### 2.1.2.6.2.106.1 **width** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>width</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>55</td></tr></tbody></table>

### <a id="673990aa-44ab-488a-b096-fad4fabb3923"></a>

###### 2.1.2.6.2.107 Field **height**

###### 2.1.2.6.2.107.1 **height** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>height</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>40</td></tr></tbody></table>

### <a id="50a7f458-fa57-45fd-b2e7-282cf4c0cbf6"></a>

###### 2.1.2.6.2.108 Field **large**

###### 2.1.2.6.2.108.1 **large** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>large</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>52</td></tr></tbody></table>

### <a id="02498d75-d2e6-4fd1-a53a-57abc98a38f1"></a>

###### 2.1.2.6.2.109 Field **weight**

###### 2.1.2.6.2.109.1 **weight** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>weight</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0.2</td></tr></tbody></table>

### <a id="13b29a06-b616-437e-9fb1-d380df8721a1"></a>

###### 2.1.2.6.2.110 Field **weight\_unit**

###### 2.1.2.6.2.110.1 **weight\_unit** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>weight_unit</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>kg</td></tr></tbody></table>

### <a id="8cd8373a-c742-450c-af35-2ef1e566306c"></a>

###### 2.1.2.6.2.111 Field **weight\_in\_unit**

###### 2.1.2.6.2.111.1 **weight\_in\_unit** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>weight_in_unit</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>2</td></tr></tbody></table>

### <a id="d55107f9-4c71-45f7-8631-22cad9d61e09"></a>

###### 2.1.2.6.2.112 Field **volume**

###### 2.1.2.6.2.112.1 **volume** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>volume</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>49500</td></tr></tbody></table>

### <a id="261c6bf7-55dd-41c9-a945-08becb5a4768"></a>

###### 2.1.2.6.2.113 Field **metadata**

###### 2.1.2.6.2.113.1 **metadata** Hierarchy

Parent field: **unified\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#94bf96ba-09ef-4497-ba1a-dc249771d8f0 class="margin-NaN">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.113.2 **metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (array,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="94bf96ba-09ef-4497-ba1a-dc249771d8f0"></a>

###### 2.1.2.6.2.114 Field **items**

###### 2.1.2.6.2.114.1 **items** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="3d3f46c8-19a3-4bb2-9833-c494566aec4c"></a>

###### 2.1.2.6.2.115 Field **free\_shipping**

###### 2.1.2.6.2.115.1 **free\_shipping** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>free_shipping</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (boolean,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="06ad3d4b-16e2-49ee-8ecf-b87e30d988f8"></a>

###### 2.1.2.6.2.116 Field **category\_id**

###### 2.1.2.6.2.116.1 **category\_id** Hierarchy

Parent field: **unified\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#55c6af7a-5289-4d30-8e88-b4071c8785ac class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#122cb18d-7b57-4023-9d51-948ed46f9e7f class="margin-NaN">name</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.116.2 **category\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>category_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="55c6af7a-5289-4d30-8e88-b4071c8785ac"></a>

###### 2.1.2.6.2.117 Field **id**

###### 2.1.2.6.2.117.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>5f6bbe0d988fee49206329c5</td></tr></tbody></table>

### <a id="122cb18d-7b57-4023-9d51-948ed46f9e7f"></a>

###### 2.1.2.6.2.118 Field **name**

###### 2.1.2.6.2.118.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="aed38f15-3584-4d7c-8a6e-c9dc6f28cfa7"></a>

###### 2.1.2.6.2.119 Field **category**

###### 2.1.2.6.2.119.1 **category** Hierarchy

Parent field: **unified\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#57cdd698-979f-4852-a8bc-4135c9c893ba class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.119.2 **category** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>category</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (document,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="57cdd698-979f-4852-a8bc-4135c9c893ba"></a>

###### 2.1.2.6.2.120 Field **properties**

###### 2.1.2.6.2.120.1 **properties** Hierarchy

Parent field: **category**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#c91f4b13-769c-41c8-bbbb-7d4490f9d989 class="margin-NaN">_id</a></td><td class="no-break-word">objectId,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#79a276ac-88f1-493c-a182-f5869d769e0e class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1e4b5c1e-6f2f-434d-8e8f-0da97a8fee49 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#04469280-4a2d-4e5a-9c8b-d9afee432c3d class="margin-NaN">category_father</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8e0ffb1c-0a91-484f-b0d5-2c754ac0f593 class="margin-NaN">path_from_root</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#62322fb0-913f-4187-a17b-4d2ef2fd6900 class="margin-NaN">children_categories</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5cbe5b44-18fc-4318-8897-a9ec2f73d1cf class="margin-NaN">settings</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5d55bd13-8be2-414a-aa4f-7373586044d2 class="margin-NaN">country</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e05be836-4250-4593-a414-ca2a17cda55e class="margin-NaN">date_created</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#615881a6-c7d6-405f-bb94-d275b5609a7f class="margin-NaN">permalink</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0e889ec9-4927-4c39-b707-e58e25a8e955 class="margin-NaN">picture</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.120.2 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="c91f4b13-769c-41c8-bbbb-7d4490f9d989"></a>

###### 2.1.2.6.2.121 Field **\_id**

###### 2.1.2.6.2.121.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (objectId,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="79a276ac-88f1-493c-a182-f5869d769e0e"></a>

###### 2.1.2.6.2.122 Field **id**

###### 2.1.2.6.2.122.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="1e4b5c1e-6f2f-434d-8e8f-0da97a8fee49"></a>

###### 2.1.2.6.2.123 Field **name**

###### 2.1.2.6.2.123.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="04469280-4a2d-4e5a-9c8b-d9afee432c3d"></a>

###### 2.1.2.6.2.124 Field **category\_father**

###### 2.1.2.6.2.124.1 **category\_father** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>category_father</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8e0ffb1c-0a91-484f-b0d5-2c754ac0f593"></a>

###### 2.1.2.6.2.125 Field **path\_from\_root**

###### 2.1.2.6.2.125.1 **path\_from\_root** Hierarchy

Parent field: **properties**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#432b6d58-e2fb-43ff-9a46-3ef52843bdac class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.125.2 **path\_from\_root** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>path_from_root</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="432b6d58-e2fb-43ff-9a46-3ef52843bdac"></a>

###### 2.1.2.6.2.126 Field **\[0\]**

###### 2.1.2.6.2.126.1 **\[0\]** Hierarchy

Parent field: **path\_from\_root**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#2de57d55-9f3e-456a-b82d-e0bbffcfaed3 class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d2660199-c7fa-464b-96cd-aca76cfd5543 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.126.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="2de57d55-9f3e-456a-b82d-e0bbffcfaed3"></a>

###### 2.1.2.6.2.127 Field **id**

###### 2.1.2.6.2.127.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="d2660199-c7fa-464b-96cd-aca76cfd5543"></a>

###### 2.1.2.6.2.128 Field **name**

###### 2.1.2.6.2.128.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="62322fb0-913f-4187-a17b-4d2ef2fd6900"></a>

###### 2.1.2.6.2.129 Field **children\_categories**

###### 2.1.2.6.2.129.1 **children\_categories** Hierarchy

Parent field: **properties**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#6b2cffb5-952c-49a5-9236-8028a2d508c9 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.129.2 **children\_categories** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>children_categories</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="6b2cffb5-952c-49a5-9236-8028a2d508c9"></a>

###### 2.1.2.6.2.130 Field **\[0\]**

###### 2.1.2.6.2.130.1 **\[0\]** Hierarchy

Parent field: **children\_categories**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#1734d25f-a2bf-4449-9366-623d0f69ac33 class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#82cbdf12-378a-4332-92d5-ef605d7c8e9b class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.130.2 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="1734d25f-a2bf-4449-9366-623d0f69ac33"></a>

###### 2.1.2.6.2.131 Field **id**

###### 2.1.2.6.2.131.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="82cbdf12-378a-4332-92d5-ef605d7c8e9b"></a>

###### 2.1.2.6.2.132 Field **name**

###### 2.1.2.6.2.132.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5cbe5b44-18fc-4318-8897-a9ec2f73d1cf"></a>

###### 2.1.2.6.2.133 Field **settings**

###### 2.1.2.6.2.133.1 **settings** Hierarchy

Parent field: **properties**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#c6ef5842-8ac4-48df-9c7d-81ad11b99dfd class="margin-NaN">adult_content</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dfd0b5b8-018c-49d1-add6-b0829a4ca80b class="margin-NaN">fragile</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c4c5f436-97cb-4f58-96ca-d1993adabe48 class="margin-NaN">status</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#59280c2e-b823-423b-a282-989fa1714895 class="margin-NaN">currencies</a></td><td class="no-break-word">array</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0c02c5a2-a8b8-42f4-aa04-f34c67b078c9 class="margin-NaN">inmediate_payment</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cf7d8e94-1c9f-4235-a148-10ddc4a1dea2 class="margin-NaN">items_review_allowed</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e761427f-4b52-45be-b232-2ed00a9c6ae7 class="margin-NaN">listing_allowed</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2fe6d910-e7ae-4969-803c-e80cd9ed9b4a class="margin-NaN">max_description_length</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c64ce533-cbaf-4ca1-90d5-139cb244e123 class="margin-NaN">max_pictures_per_item</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7c346327-bd82-410d-bc58-0a782291f701 class="margin-NaN">max_pictures_per_item_var</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5841fc12-ba0f-44e2-a3be-65163143da9e class="margin-NaN">max_sub_title_length</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bd8b7d40-e35c-4e40-a3e3-19e5c2b2ad8a class="margin-NaN">max_title_length</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7858c557-11f9-4dd8-9e5e-cd78ab1a017c class="margin-NaN">maximum_price</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dec9ef3a-0cdf-47f1-98a9-ea5be11546ef class="margin-NaN">maximum_price_currency</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#54d7e874-ece5-4f35-8d40-ed558fa97cb0 class="margin-NaN">minimum_price</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5f0a6210-dde0-4c7d-a2d1-f814a91741fe class="margin-NaN">minimum_price_currency</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a827e458-921a-4afb-b448-be3c5d73915e class="margin-NaN">sat_product_code_mexico</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#59e812a3-ff28-46b2-ba3f-0a13a2c72c12 class="margin-NaN">sat_product_description_mexico</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#599d0478-2466-444e-a153-e8f44fec14b5 class="margin-NaN">seller_contact</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.133.2 **settings** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>settings</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="c6ef5842-8ac4-48df-9c7d-81ad11b99dfd"></a>

###### 2.1.2.6.2.134 Field **adult\_content**

###### 2.1.2.6.2.134.1 **adult\_content** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>adult_content</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="dfd0b5b8-018c-49d1-add6-b0829a4ca80b"></a>

###### 2.1.2.6.2.135 Field **fragile**

###### 2.1.2.6.2.135.1 **fragile** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fragile</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c4c5f436-97cb-4f58-96ca-d1993adabe48"></a>

###### 2.1.2.6.2.136 Field **status**

###### 2.1.2.6.2.136.1 **status** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>status</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="59280c2e-b823-423b-a282-989fa1714895"></a>

###### 2.1.2.6.2.137 Field **currencies**

###### 2.1.2.6.2.137.1 **currencies** Hierarchy

Parent field: **settings**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#08e14ce9-3367-42fa-ae97-4b321cea86c5 class="margin-NaN">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.137.2 **currencies** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>currencies</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="08e14ce9-3367-42fa-ae97-4b321cea86c5"></a>

###### 2.1.2.6.2.138 Field **\[0\]**

###### 2.1.2.6.2.138.1 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr></tbody></table>

### <a id="0c02c5a2-a8b8-42f4-aa04-f34c67b078c9"></a>

###### 2.1.2.6.2.139 Field **inmediate\_payment**

###### 2.1.2.6.2.139.1 **inmediate\_payment** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>inmediate_payment</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="cf7d8e94-1c9f-4235-a148-10ddc4a1dea2"></a>

###### 2.1.2.6.2.140 Field **items\_review\_allowed**

###### 2.1.2.6.2.140.1 **items\_review\_allowed** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>items_review_allowed</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="e761427f-4b52-45be-b232-2ed00a9c6ae7"></a>

###### 2.1.2.6.2.141 Field **listing\_allowed**

###### 2.1.2.6.2.141.1 **listing\_allowed** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>listing_allowed</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="2fe6d910-e7ae-4969-803c-e80cd9ed9b4a"></a>

###### 2.1.2.6.2.142 Field **max\_description\_length**

###### 2.1.2.6.2.142.1 **max\_description\_length** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>max_description_length</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c64ce533-cbaf-4ca1-90d5-139cb244e123"></a>

###### 2.1.2.6.2.143 Field **max\_pictures\_per\_item**

###### 2.1.2.6.2.143.1 **max\_pictures\_per\_item** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>max_pictures_per_item</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="7c346327-bd82-410d-bc58-0a782291f701"></a>

###### 2.1.2.6.2.144 Field **max\_pictures\_per\_item\_var**

###### 2.1.2.6.2.144.1 **max\_pictures\_per\_item\_var** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>max_pictures_per_item_var</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5841fc12-ba0f-44e2-a3be-65163143da9e"></a>

###### 2.1.2.6.2.145 Field **max\_sub\_title\_length**

###### 2.1.2.6.2.145.1 **max\_sub\_title\_length** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>max_sub_title_length</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="bd8b7d40-e35c-4e40-a3e3-19e5c2b2ad8a"></a>

###### 2.1.2.6.2.146 Field **max\_title\_length**

###### 2.1.2.6.2.146.1 **max\_title\_length** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>max_title_length</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="7858c557-11f9-4dd8-9e5e-cd78ab1a017c"></a>

###### 2.1.2.6.2.147 Field **maximum\_price**

###### 2.1.2.6.2.147.1 **maximum\_price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>maximum_price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="dec9ef3a-0cdf-47f1-98a9-ea5be11546ef"></a>

###### 2.1.2.6.2.148 Field **maximum\_price\_currency**

###### 2.1.2.6.2.148.1 **maximum\_price\_currency** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>maximum_price_currency</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="54d7e874-ece5-4f35-8d40-ed558fa97cb0"></a>

###### 2.1.2.6.2.149 Field **minimum\_price**

###### 2.1.2.6.2.149.1 **minimum\_price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>minimum_price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5f0a6210-dde0-4c7d-a2d1-f814a91741fe"></a>

###### 2.1.2.6.2.150 Field **minimum\_price\_currency**

###### 2.1.2.6.2.150.1 **minimum\_price\_currency** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>minimum_price_currency</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a827e458-921a-4afb-b448-be3c5d73915e"></a>

###### 2.1.2.6.2.151 Field **sat\_product\_code\_mexico**

###### 2.1.2.6.2.151.1 **sat\_product\_code\_mexico** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>sat_product_code_mexico</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="59e812a3-ff28-46b2-ba3f-0a13a2c72c12"></a>

###### 2.1.2.6.2.152 Field **sat\_product\_description\_mexico**

###### 2.1.2.6.2.152.1 **sat\_product\_description\_mexico** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>sat_product_description_mexico</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="599d0478-2466-444e-a153-e8f44fec14b5"></a>

###### 2.1.2.6.2.153 Field **seller\_contact**

###### 2.1.2.6.2.153.1 **seller\_contact** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>seller_contact</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5d55bd13-8be2-414a-aa4f-7373586044d2"></a>

###### 2.1.2.6.2.154 Field **country**

###### 2.1.2.6.2.154.1 **country** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="e05be836-4250-4593-a414-ca2a17cda55e"></a>

###### 2.1.2.6.2.155 Field **date\_created**

###### 2.1.2.6.2.155.1 **date\_created** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>date_created</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="615881a6-c7d6-405f-bb94-d275b5609a7f"></a>

###### 2.1.2.6.2.156 Field **permalink**

###### 2.1.2.6.2.156.1 **permalink** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>permalink</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="0e889ec9-4927-4c39-b707-e58e25a8e955"></a>

###### 2.1.2.6.2.157 Field **picture**

###### 2.1.2.6.2.157.1 **picture** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>picture</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c75e6333-afa2-4c68-8438-0e6763a7942c"></a>

###### 2.1.2.6.2.158 Field **warranty**

###### 2.1.2.6.2.158.1 **warranty** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>warranty</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="9bee1cfe-0b40-44dc-8b5a-e5bd377e0551"></a>

###### 2.1.2.6.2.159 Field **warranty\_description**

###### 2.1.2.6.2.159.1 **warranty\_description** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>warranty_description</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ad4d5f9a-09fd-46c4-95f8-24eda3d77d0d"></a>

###### 2.1.2.6.2.160 Field **country\_ref**

###### 2.1.2.6.2.160.1 **country\_ref** Hierarchy

Parent field: **unified\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#fd2fe4a1-6806-45e2-aa00-add083b683b2 class="margin-NaN">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f384f56f-30e5-406b-89f3-60ccd30e53d5 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5b74f234-d47e-4aef-8d97-eae19adf0143 class="margin-NaN">iso2</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#48ff6ffc-d5f1-4ef3-acf9-a7554ad1bb49 class="margin-NaN">iso3</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ac51ee37-90a9-47e2-853c-c1cfdf8716bb class="margin-NaN">flag_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#501e81e4-6013-4d5d-91be-f5382f70520e class="margin-NaN">phone_code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.160.2 **country\_ref** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country_ref</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="fd2fe4a1-6806-45e2-aa00-add083b683b2"></a>

###### 2.1.2.6.2.161 Field **\_id**

###### 2.1.2.6.2.161.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="f384f56f-30e5-406b-89f3-60ccd30e53d5"></a>

###### 2.1.2.6.2.162 Field **name**

###### 2.1.2.6.2.162.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Colombia</td></tr></tbody></table>

### <a id="5b74f234-d47e-4aef-8d97-eae19adf0143"></a>

###### 2.1.2.6.2.163 Field **iso2**

###### 2.1.2.6.2.163.1 **iso2** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>iso2</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>CO</td></tr></tbody></table>

### <a id="48ff6ffc-d5f1-4ef3-acf9-a7554ad1bb49"></a>

###### 2.1.2.6.2.164 Field **iso3**

###### 2.1.2.6.2.164.1 **iso3** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>iso3</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>COL</td></tr></tbody></table>

### <a id="ac51ee37-90a9-47e2-853c-c1cfdf8716bb"></a>

###### 2.1.2.6.2.165 Field **flag\_url**

###### 2.1.2.6.2.165.1 **flag\_url** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>flag_url</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://www.geonames.org/flags/x/co.gif</td></tr></tbody></table>

### <a id="501e81e4-6013-4d5d-91be-f5382f70520e"></a>

###### 2.1.2.6.2.166 Field **phone\_code**

###### 2.1.2.6.2.166.1 **phone\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>phone_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>57</td></tr></tbody></table>

### <a id="cc4b35b6-8f54-43ed-a4a4-fac9ec5e1af3"></a>

###### 2.1.2.6.2.167 Field **shared**

###### 2.1.2.6.2.167.1 **shared** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shared</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="24696a36-7a61-4cef-bf7d-43dd68caf232"></a>

###### 2.1.2.6.2.168 Field **disabled**

###### 2.1.2.6.2.168.1 **disabled** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>disabled</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a2bb589d-72b9-486c-81ce-46cab7afac87"></a>

###### 2.1.2.6.2.169 Field **disabled\_by\_inactivity**

###### 2.1.2.6.2.169.1 **disabled\_by\_inactivity** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>disabled_by_inactivity</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="6cc02d56-0a5c-47e1-8678-6a3ebc71ed97"></a>

###### 2.1.2.6.2.170 Field **dropshipper**

###### 2.1.2.6.2.170.1 **dropshipper** Hierarchy

Parent field: **unified\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#ed046033-2ebc-4716-94a7-05161132e010 class="margin-NaN">data</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fedf2777-e165-4cf9-943e-69e4adee81a2 class="margin-NaN">id_import</a></td><td class="no-break-word">string,objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6df057f3-3814-44b9-8170-1c542fbdbb64 class="margin-NaN">price</a></td><td class="no-break-word">numeric,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.170.2 **dropshipper** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dropshipper</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="ed046033-2ebc-4716-94a7-05161132e010"></a>

###### 2.1.2.6.2.171 Field **data**

###### 2.1.2.6.2.171.1 **data** Hierarchy

Parent field: **dropshipper**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#d511caa6-7a72-48aa-9f60-5bd926221a62 class="margin-NaN">db_importer</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#31ea1152-0af5-47d3-ac25-64e767c3b923 class="margin-NaN">shop</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.171.2 **data** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>data</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="d511caa6-7a72-48aa-9f60-5bd926221a62"></a>

###### 2.1.2.6.2.172 Field **db\_importer**

###### 2.1.2.6.2.172.1 **db\_importer** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>db_importer</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>testtwodrop_804079258</td></tr></tbody></table>

### <a id="31ea1152-0af5-47d3-ac25-64e767c3b923"></a>

###### 2.1.2.6.2.173 Field **shop**

###### 2.1.2.6.2.173.1 **shop** Hierarchy

Parent field: **data**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#d386ded4-5918-4156-b663-c09d38b8ea6e class="margin-NaN">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#53db87e4-1b13-4d1d-a7f5-bee112a930d2 class="margin-NaN">carry</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#42707f3f-f30a-432e-83a1-4ffe1e6dac4d class="margin-NaN">cc_nit</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#57bde019-33ba-49c3-a0f4-d3f332bda31d class="margin-NaN">city</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2bcdec1a-b328-46e8-a92b-4313e6aae9c2 class="margin-NaN">cod_postal</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f902f797-78a6-4ac0-9d6d-a52714cd667e class="margin-NaN">color_primary</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#24e86e8a-18d9-46b4-a1e7-3ec2720b3669 class="margin-NaN">colors</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c431ab09-6d31-4e86-8591-fe9f80f47376 class="margin-NaN">composed_address</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1270cf9c-273c-4b2e-b7f1-f3a4c9f941dc class="margin-NaN">country</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#021a2d22-e241-4272-b12f-b52b3a3dda19 class="margin-NaN">default</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b4fa7d4b-101c-4a79-8b96-9bb0f0f29d6f class="margin-NaN">departament</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ec25ddb8-f978-4042-ba18-a8463127ba57 class="margin-NaN">email</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f9dcb654-2ce8-4eb0-a2fc-59061c84b473 class="margin-NaN">geolocation</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6bedeab5-eb49-4d7f-82ee-22b705c3da8b class="margin-NaN">gtag</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1f1786a6-0de8-4b38-9a5c-1d692e79f850 class="margin-NaN">indicative</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8b8bcc68-b8a7-4902-a833-ee8ef2ede116 class="margin-NaN">large_description</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a5fd1468-2377-46ad-941d-d210a1a2a3e1 class="margin-NaN">location</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a1df519e-c6f4-4eba-aec9-f3c2940d4e6e class="margin-NaN">logo</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#64e15efc-a5f9-44c2-860c-467e739e5f2c class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#39b25ba9-5273-469f-b839-b62d8aadb2dd class="margin-NaN">neighborhood</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0c1313fd-ac32-4d4e-a18d-41568d219f6b class="margin-NaN">pixel</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6d279947-e770-4e79-bf50-6b595e5e1226 class="margin-NaN">principal_address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f9b21e85-e979-4eba-a29d-23b67eb3e1ca class="margin-NaN">promises</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d7f97ab6-3f18-4866-967f-8c9166a9342e class="margin-NaN">slogan</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.173.2 **shop** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shop</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="d386ded4-5918-4156-b663-c09d38b8ea6e"></a>

###### 2.1.2.6.2.174 Field **address**

###### 2.1.2.6.2.174.1 **address** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>address</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Carrera 48 # 45 - 44</td></tr></tbody></table>

### <a id="53db87e4-1b13-4d1d-a7f5-bee112a930d2"></a>

###### 2.1.2.6.2.175 Field **carry**

###### 2.1.2.6.2.175.1 **carry** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>carry</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="42707f3f-f30a-432e-83a1-4ffe1e6dac4d"></a>

###### 2.1.2.6.2.176 Field **cc\_nit**

###### 2.1.2.6.2.176.1 **cc\_nit** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cc_nit</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6513232</td></tr></tbody></table>

### <a id="57bde019-33ba-49c3-a0f4-d3f332bda31d"></a>

###### 2.1.2.6.2.177 Field **city**

###### 2.1.2.6.2.177.1 **city** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#ac8ac35b-8e21-45d5-b31f-354d8fc194ba class="margin-NaN">_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#be7e564c-a031-4e8f-9fb9-ffcd252c83e8 class="margin-NaN">before_courrier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8be037db-2863-403e-9556-4df1d59c7e66 class="margin-NaN">checked</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bc159314-81ae-4e54-ba0d-c8561f540c1a class="margin-NaN">city_code</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0b705d40-a8d0-40c0-bbd1-b91bd8b1021f class="margin-NaN">cod_depto</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e234c789-3272-423c-b8af-2471cd674241 class="margin-NaN">country</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e145bb01-2f7b-4600-a3e8-febb7e1932cb class="margin-NaN">courrier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#109f30e6-6db0-4f70-b04f-b49f2135e0ac class="margin-NaN">dane_code</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8018c9ec-be4c-4513-ab84-e8289bc1ae20 class="margin-NaN">disabled</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f732cc36-9392-44c7-87d7-49a4901a2ceb class="margin-NaN">forTest</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#da6d497a-b825-40f8-b01e-5192f94c74f1 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7566ba06-5df9-4ac0-83d2-4af15b1433d3 class="margin-NaN">postal_code</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5684cd81-4be5-4d93-9981-192e4ac50dd4 class="margin-NaN">shipping_zone</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2989c74b-8893-4e26-bfd7-18cb235bc5cd class="margin-NaN">shop_error</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c594be0d-1559-4dc5-8014-0608af88b916 class="margin-NaN">state</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.177.2 **city** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>city</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="ac8ac35b-8e21-45d5-b31f-354d8fc194ba"></a>

###### 2.1.2.6.2.178 Field **\_id**

###### 2.1.2.6.2.178.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6047cb9b2a977165ccde8d2c</td></tr></tbody></table>

### <a id="be7e564c-a031-4e8f-9fb9-ffcd252c83e8"></a>

###### 2.1.2.6.2.179 Field **before\_courrier**

###### 2.1.2.6.2.179.1 **before\_courrier** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>before_courrier</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>tcc</td></tr></tbody></table>

### <a id="8be037db-2863-403e-9556-4df1d59c7e66"></a>

###### 2.1.2.6.2.180 Field **checked**

###### 2.1.2.6.2.180.1 **checked** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>checked</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="bc159314-81ae-4e54-ba0d-c8561f540c1a"></a>

###### 2.1.2.6.2.181 Field **city\_code**

###### 2.1.2.6.2.181.1 **city\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>city_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>5001000</td></tr></tbody></table>

### <a id="0b705d40-a8d0-40c0-bbd1-b91bd8b1021f"></a>

###### 2.1.2.6.2.182 Field **cod\_depto**

###### 2.1.2.6.2.182.1 **cod\_depto** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cod_depto</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>05</td></tr></tbody></table>

### <a id="e234c789-3272-423c-b8af-2471cd674241"></a>

###### 2.1.2.6.2.183 Field **country**

###### 2.1.2.6.2.183.1 **country** Hierarchy

Parent field: **city**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#3a80fa46-e603-4ce5-9e07-4b28876e84a6 class="margin-NaN">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ec61a93e-eac0-47a3-b3d3-8633098378bb class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d3398ba5-31c1-467b-81de-7833b478bf45 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.183.2 **country** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="3a80fa46-e603-4ce5-9e07-4b28876e84a6"></a>

###### 2.1.2.6.2.184 Field **code**

###### 2.1.2.6.2.184.1 **code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>COL</td></tr></tbody></table>

### <a id="ec61a93e-eac0-47a3-b3d3-8633098378bb"></a>

###### 2.1.2.6.2.185 Field **id**

###### 2.1.2.6.2.185.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6047cb912a977165ccde8cd1</td></tr></tbody></table>

### <a id="d3398ba5-31c1-467b-81de-7833b478bf45"></a>

###### 2.1.2.6.2.186 Field **name**

###### 2.1.2.6.2.186.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Colombia</td></tr></tbody></table>

### <a id="e145bb01-2f7b-4600-a3e8-febb7e1932cb"></a>

###### 2.1.2.6.2.187 Field **courrier**

###### 2.1.2.6.2.187.1 **courrier** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>courrier</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>servientrega</td></tr></tbody></table>

### <a id="109f30e6-6db0-4f70-b04f-b49f2135e0ac"></a>

###### 2.1.2.6.2.188 Field **dane\_code**

###### 2.1.2.6.2.188.1 **dane\_code** Hierarchy

Parent field: **city**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#7d725b85-a38c-4ffa-87b2-71edd7626db2 class="margin-NaN">rocketfy</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#59acfc1c-58f1-4bfb-99db-124595c59a33 class="margin-NaN">servientrega</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.188.2 **dane\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dane_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="7d725b85-a38c-4ffa-87b2-71edd7626db2"></a>

###### 2.1.2.6.2.189 Field **rocketfy**

###### 2.1.2.6.2.189.1 **rocketfy** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>rocketfy</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>05360</td></tr></tbody></table>

### <a id="59acfc1c-58f1-4bfb-99db-124595c59a33"></a>

###### 2.1.2.6.2.190 Field **servientrega**

###### 2.1.2.6.2.190.1 **servientrega** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>servientrega</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>05360</td></tr></tbody></table>

### <a id="8018c9ec-be4c-4513-ab84-e8289bc1ae20"></a>

###### 2.1.2.6.2.191 Field **disabled**

###### 2.1.2.6.2.191.1 **disabled** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>disabled</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="f732cc36-9392-44c7-87d7-49a4901a2ceb"></a>

###### 2.1.2.6.2.192 Field **forTest**

###### 2.1.2.6.2.192.1 **forTest** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>forTest</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="da6d497a-b825-40f8-b01e-5192f94c74f1"></a>

###### 2.1.2.6.2.193 Field **name**

###### 2.1.2.6.2.193.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Itagui</td></tr></tbody></table>

### <a id="7566ba06-5df9-4ac0-83d2-4af15b1433d3"></a>

###### 2.1.2.6.2.194 Field **postal\_code**

###### 2.1.2.6.2.194.1 **postal\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>postal_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>05360000</td></tr></tbody></table>

### <a id="5684cd81-4be5-4d93-9981-192e4ac50dd4"></a>

###### 2.1.2.6.2.195 Field **shipping\_zone**

###### 2.1.2.6.2.195.1 **shipping\_zone** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shipping_zone</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="2989c74b-8893-4e26-bfd7-18cb235bc5cd"></a>

###### 2.1.2.6.2.196 Field **shop\_error**

###### 2.1.2.6.2.196.1 **shop\_error** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shop_error</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="c594be0d-1559-4dc5-8014-0608af88b916"></a>

###### 2.1.2.6.2.197 Field **state**

###### 2.1.2.6.2.197.1 **state** Hierarchy

Parent field: **city**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#65d27686-c1a7-4293-803c-bcf5f91eff89 class="margin-NaN">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#45fd203a-2362-4983-ad2e-e00a5366ad1e class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#46c250e3-3071-4ad6-8e2b-53331aa96f72 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.197.2 **state** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>state</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="65d27686-c1a7-4293-803c-bcf5f91eff89"></a>

###### 2.1.2.6.2.198 Field **code**

###### 2.1.2.6.2.198.1 **code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>25</td></tr></tbody></table>

### <a id="45fd203a-2362-4983-ad2e-e00a5366ad1e"></a>

###### 2.1.2.6.2.199 Field **id**

###### 2.1.2.6.2.199.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6047cb912a977165ccde8cdb</td></tr></tbody></table>

### <a id="46c250e3-3071-4ad6-8e2b-53331aa96f72"></a>

###### 2.1.2.6.2.200 Field **name**

###### 2.1.2.6.2.200.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Cundinamarca</td></tr></tbody></table>

### <a id="2bcdec1a-b328-46e8-a92b-4313e6aae9c2"></a>

###### 2.1.2.6.2.201 Field **cod\_postal**

###### 2.1.2.6.2.201.1 **cod\_postal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cod_postal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>050021</td></tr></tbody></table>

### <a id="f902f797-78a6-4ac0-9d6d-a52714cd667e"></a>

###### 2.1.2.6.2.202 Field **color\_primary**

###### 2.1.2.6.2.202.1 **color\_primary** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>color_primary</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>#161114</td></tr></tbody></table>

### <a id="24e86e8a-18d9-46b4-a1e7-3ec2720b3669"></a>

###### 2.1.2.6.2.203 Field **colors**

###### 2.1.2.6.2.203.1 **colors** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#abdc360f-ab50-4a6a-9704-74fadb316583 class="margin-NaN">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.203.2 **colors** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>colors</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="abdc360f-ab50-4a6a-9704-74fadb316583"></a>

###### 2.1.2.6.2.204 Field **\[0\]**

###### 2.1.2.6.2.204.1 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Sample</td><td>#756055</td></tr></tbody></table>

### <a id="c431ab09-6d31-4e86-8591-fe9f80f47376"></a>

###### 2.1.2.6.2.205 Field **composed\_address**

###### 2.1.2.6.2.205.1 **composed\_address** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#cc382011-090f-4b5f-aef1-efb8d34f9d8e class="margin-NaN">street</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7f7eefc7-df9f-43b8-92c8-3259b1ebd62c class="margin-NaN">street_number_one</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#84d49e59-0005-42de-b99d-1c00286d1d58 class="margin-NaN">street_number_two</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.205.2 **composed\_address** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>composed_address</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="cc382011-090f-4b5f-aef1-efb8d34f9d8e"></a>

###### 2.1.2.6.2.206 Field **street**

###### 2.1.2.6.2.206.1 **street** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>street</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Carrera 48</td></tr></tbody></table>

### <a id="7f7eefc7-df9f-43b8-92c8-3259b1ebd62c"></a>

###### 2.1.2.6.2.207 Field **street\_number\_one**

###### 2.1.2.6.2.207.1 **street\_number\_one** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>street_number_one</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>45</td></tr></tbody></table>

### <a id="84d49e59-0005-42de-b99d-1c00286d1d58"></a>

###### 2.1.2.6.2.208 Field **street\_number\_two**

###### 2.1.2.6.2.208.1 **street\_number\_two** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>street_number_two</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>44</td></tr></tbody></table>

### <a id="1270cf9c-273c-4b2e-b7f1-f3a4c9f941dc"></a>

###### 2.1.2.6.2.209 Field **country**

###### 2.1.2.6.2.209.1 **country** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>COL</td></tr></tbody></table>

### <a id="021a2d22-e241-4272-b12f-b52b3a3dda19"></a>

###### 2.1.2.6.2.210 Field **default**

###### 2.1.2.6.2.210.1 **default** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>default</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="b4fa7d4b-101c-4a79-8b96-9bb0f0f29d6f"></a>

###### 2.1.2.6.2.211 Field **departament**

###### 2.1.2.6.2.211.1 **departament** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#5f4bb39d-24a9-42c3-9d6b-e0a0d613d180 class="margin-NaN">_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3c92b036-0857-43f2-8614-9aa53e451fac class="margin-NaN">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#787a542c-2165-4ae1-ab6e-e2ed80432422 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.211.2 **departament** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>departament</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="5f4bb39d-24a9-42c3-9d6b-e0a0d613d180"></a>

###### 2.1.2.6.2.212 Field **\_id**

###### 2.1.2.6.2.212.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6047cb912a977165ccde8cd2</td></tr></tbody></table>

### <a id="3c92b036-0857-43f2-8614-9aa53e451fac"></a>

###### 2.1.2.6.2.213 Field **code**

###### 2.1.2.6.2.213.1 **code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>05</td></tr></tbody></table>

### <a id="787a542c-2165-4ae1-ab6e-e2ed80432422"></a>

###### 2.1.2.6.2.214 Field **name**

###### 2.1.2.6.2.214.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Antioquia</td></tr></tbody></table>

### <a id="ec25ddb8-f978-4042-ba18-a8463127ba57"></a>

###### 2.1.2.6.2.215 Field **email**

###### 2.1.2.6.2.215.1 **email** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>email</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>asccmml@adfaf.co</td></tr></tbody></table>

### <a id="f9dcb654-2ce8-4eb0-a2fc-59061c84b473"></a>

###### 2.1.2.6.2.216 Field **geolocation**

###### 2.1.2.6.2.216.1 **geolocation** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#1949d2aa-32aa-426c-a71a-e533c464b4fd class="margin-NaN">lat</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f39f9f4f-2e64-47c8-b2ad-0e9635032675 class="margin-NaN">lng</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.216.2 **geolocation** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>geolocation</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="1949d2aa-32aa-426c-a71a-e533c464b4fd"></a>

###### 2.1.2.6.2.217 Field **lat**

###### 2.1.2.6.2.217.1 **lat** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>lat</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="f39f9f4f-2e64-47c8-b2ad-0e9635032675"></a>

###### 2.1.2.6.2.218 Field **lng**

###### 2.1.2.6.2.218.1 **lng** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>lng</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="6bedeab5-eb49-4d7f-82ee-22b705c3da8b"></a>

###### 2.1.2.6.2.219 Field **gtag**

###### 2.1.2.6.2.219.1 **gtag** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>gtag</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>GTM-WQDJT8B</td></tr></tbody></table>

### <a id="1f1786a6-0de8-4b38-9a5c-1d692e79f850"></a>

###### 2.1.2.6.2.220 Field **indicative**

###### 2.1.2.6.2.220.1 **indicative** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>indicative</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>57</td></tr></tbody></table>

### <a id="8b8bcc68-b8a7-4902-a833-ee8ef2ede116"></a>

###### 2.1.2.6.2.221 Field **large\_description**

###### 2.1.2.6.2.221.1 **large\_description** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>large_description</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a5fd1468-2377-46ad-941d-d210a1a2a3e1"></a>

###### 2.1.2.6.2.222 Field **location**

###### 2.1.2.6.2.222.1 **location** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>location</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="a1df519e-c6f4-4eba-aec9-f3c2940d4e6e"></a>

###### 2.1.2.6.2.223 Field **logo**

###### 2.1.2.6.2.223.1 **logo** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#b3c0819e-6f40-417b-b5c7-e3a2fe8c41b2 class="margin-NaN">acl</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#04effb38-cf40-45c7-bf6c-107c189d4d9e class="margin-NaN">bucket</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2af742fa-448e-4ceb-9385-1488deb95e7b class="margin-NaN">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ef2089e0-46b1-49f6-b9d8-ae5eb53b8e87 class="margin-NaN">contentType</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#80d77e22-e039-4a97-984b-c1f2351e3f25 class="margin-NaN">created_time</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#52776beb-8dbd-4c68-ab5e-132924ab7595 class="margin-NaN">encoding</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0bd9dded-efe2-4263-bc79-49bb5db42ba1 class="margin-NaN">etag</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#87ed7b42-0652-40b6-8baa-1e240b1c851b class="margin-NaN">fieldname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#64441011-5f81-4522-97f8-1f0c4b1114db class="margin-NaN">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8b15faed-b0be-4ce2-9e18-65b4f2d3ecee class="margin-NaN">location</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8f8c28d7-ed1c-4ab5-a2ce-d7455d2e7bf4 class="margin-NaN">metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#12cc603f-b035-4cde-92af-959334c4381e class="margin-NaN">mimetype</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c33db1b9-5c63-4975-8a86-77c874419702 class="margin-NaN">originalname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a886a177-68e8-4195-9d3b-1be51ccc3329 class="margin-NaN">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7d11e2b5-8661-4549-bfa8-1d23cad1f932 class="margin-NaN">size</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cdd97757-348d-47fd-b719-707a07f6fd0b class="margin-NaN">storageClass</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ca481b70-ad59-40de-9b1d-eeea3cca4ee9 class="margin-NaN">versionId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.223.2 **logo** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>logo</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="b3c0819e-6f40-417b-b5c7-e3a2fe8c41b2"></a>

###### 2.1.2.6.2.224 Field **acl**

###### 2.1.2.6.2.224.1 **acl** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>acl</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>public-read</td></tr></tbody></table>

### <a id="04effb38-cf40-45c7-bf6c-107c189d4d9e"></a>

###### 2.1.2.6.2.225 Field **bucket**

###### 2.1.2.6.2.225.1 **bucket** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>bucket</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>shopping-rocketfy-uploads</td></tr></tbody></table>

### <a id="2af742fa-448e-4ceb-9385-1488deb95e7b"></a>

###### 2.1.2.6.2.226 Field **contentDisposition**

###### 2.1.2.6.2.226.1 **contentDisposition** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentDisposition</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ef2089e0-46b1-49f6-b9d8-ae5eb53b8e87"></a>

###### 2.1.2.6.2.227 Field **contentType**

###### 2.1.2.6.2.227.1 **contentType** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentType</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="80d77e22-e039-4a97-984b-c1f2351e3f25"></a>

###### 2.1.2.6.2.228 Field **created\_time**

###### 2.1.2.6.2.228.1 **created\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="52776beb-8dbd-4c68-ab5e-132924ab7595"></a>

###### 2.1.2.6.2.229 Field **encoding**

###### 2.1.2.6.2.229.1 **encoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>encoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>7bit</td></tr></tbody></table>

### <a id="0bd9dded-efe2-4263-bc79-49bb5db42ba1"></a>

###### 2.1.2.6.2.230 Field **etag**

###### 2.1.2.6.2.230.1 **etag** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>etag</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>"6e3aad264a7efb2be5567ecc968adac6"</td></tr></tbody></table>

### <a id="87ed7b42-0652-40b6-8baa-1e240b1c851b"></a>

###### 2.1.2.6.2.231 Field **fieldname**

###### 2.1.2.6.2.231.1 **fieldname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="64441011-5f81-4522-97f8-1f0c4b1114db"></a>

###### 2.1.2.6.2.232 Field **key**

###### 2.1.2.6.2.232.1 **key** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>key</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>testtwodrop_804079258_121642999_10221463163479893_6069666320517077970_n44.jpg</td></tr></tbody></table>

### <a id="8b15faed-b0be-4ce2-9e18-65b4f2d3ecee"></a>

###### 2.1.2.6.2.233 Field **location**

###### 2.1.2.6.2.233.1 **location** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>location</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://shopping-rocketfy-uploads.s3.amazonaws.com/testtwodrop_804079258_121642999_10221463163479893_6069666320517077970_n44.jpg</td></tr></tbody></table>

### <a id="8f8c28d7-ed1c-4ab5-a2ce-d7455d2e7bf4"></a>

###### 2.1.2.6.2.234 Field **metadata**

###### 2.1.2.6.2.234.1 **metadata** Hierarchy

Parent field: **logo**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#118d626c-9743-46cf-9fbf-b1d5f5773484 class="margin-NaN">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#144191bf-86f7-4dad-9b11-59a5c624d91c class="margin-NaN">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.234.2 **metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="118d626c-9743-46cf-9fbf-b1d5f5773484"></a>

###### 2.1.2.6.2.235 Field **Content-Type**

###### 2.1.2.6.2.235.1 **Content-Type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Content-Type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="144191bf-86f7-4dad-9b11-59a5c624d91c"></a>

###### 2.1.2.6.2.236 Field **fieldName**

###### 2.1.2.6.2.236.1 **fieldName** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldName</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="12cc603f-b035-4cde-92af-959334c4381e"></a>

###### 2.1.2.6.2.237 Field **mimetype**

###### 2.1.2.6.2.237.1 **mimetype** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mimetype</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="c33db1b9-5c63-4975-8a86-77c874419702"></a>

###### 2.1.2.6.2.238 Field **originalname**

###### 2.1.2.6.2.238.1 **originalname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>originalname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>testtwodrop_804079258_121642999_10221463163479893_6069666320517077970_n44.jpg</td></tr></tbody></table>

### <a id="a886a177-68e8-4195-9d3b-1be51ccc3329"></a>

###### 2.1.2.6.2.239 Field **serverSideEncryption**

###### 2.1.2.6.2.239.1 **serverSideEncryption** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>serverSideEncryption</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="7d11e2b5-8661-4549-bfa8-1d23cad1f932"></a>

###### 2.1.2.6.2.240 Field **size**

###### 2.1.2.6.2.240.1 **size** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>size</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>49920</td></tr></tbody></table>

### <a id="cdd97757-348d-47fd-b719-707a07f6fd0b"></a>

###### 2.1.2.6.2.241 Field **storageClass**

###### 2.1.2.6.2.241.1 **storageClass** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>storageClass</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>STANDARD</td></tr></tbody></table>

### <a id="ca481b70-ad59-40de-9b1d-eeea3cca4ee9"></a>

###### 2.1.2.6.2.242 Field **versionId**

###### 2.1.2.6.2.242.1 **versionId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>versionId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>YwuL_Q7QgcwdEMBRJZnahbpqpbdwlb.R</td></tr></tbody></table>

### <a id="64e15efc-a5f9-44c2-860c-467e739e5f2c"></a>

###### 2.1.2.6.2.243 Field **name**

###### 2.1.2.6.2.243.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>test two drop</td></tr></tbody></table>

### <a id="39b25ba9-5273-469f-b839-b62d8aadb2dd"></a>

###### 2.1.2.6.2.244 Field **neighborhood**

###### 2.1.2.6.2.244.1 **neighborhood** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>neighborhood</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Itagui</td></tr></tbody></table>

### <a id="0c1313fd-ac32-4d4e-a18d-41568d219f6b"></a>

###### 2.1.2.6.2.245 Field **pixel**

###### 2.1.2.6.2.245.1 **pixel** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>pixel</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="6d279947-e770-4e79-bf50-6b595e5e1226"></a>

###### 2.1.2.6.2.246 Field **principal\_address**

###### 2.1.2.6.2.246.1 **principal\_address** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>principal_address</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6009d0c2987a62252084d5e9</td></tr></tbody></table>

### <a id="f9b21e85-e979-4eba-a29d-23b67eb3e1ca"></a>

###### 2.1.2.6.2.247 Field **promises**

###### 2.1.2.6.2.247.1 **promises** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>promises</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="d7f97ab6-3f18-4866-967f-8c9166a9342e"></a>

###### 2.1.2.6.2.248 Field **slogan**

###### 2.1.2.6.2.248.1 **slogan** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>slogan</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="fedf2777-e165-4cf9-943e-69e4adee81a2"></a>

###### 2.1.2.6.2.249 Field **id\_import**

###### 2.1.2.6.2.249.1 **id\_import** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id_import</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,objectId)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="6df057f3-3814-44b9-8170-1c542fbdbb64"></a>

###### 2.1.2.6.2.250 Field **price**

###### 2.1.2.6.2.250.1 **price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="1a45535a-ba4a-49ff-ac38-89394c1590ea"></a>

###### 2.1.2.6.2.251 Field **import**

###### 2.1.2.6.2.251.1 **import** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>import</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="1ac5492c-d5aa-48ef-acf1-9284fbd10746"></a>

###### 2.1.2.6.2.252 Field **shared\_metadata**

###### 2.1.2.6.2.252.1 **shared\_metadata** Hierarchy

Parent field: **unified\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#e5742997-2997-4328-80db-0b5f71b1cb22 class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.252.2 **shared\_metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shared_metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (document,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="e5742997-2997-4328-80db-0b5f71b1cb22"></a>

###### 2.1.2.6.2.253 Field **properties**

###### 2.1.2.6.2.253.1 **properties** Hierarchy

Parent field: **shared\_metadata**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#9b3f0b4c-d6f8-417b-a39a-588ff0ede9f2 class="margin-NaN">shared_with</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.253.2 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="9b3f0b4c-d6f8-417b-a39a-588ff0ede9f2"></a>

###### 2.1.2.6.2.254 Field **shared\_with**

###### 2.1.2.6.2.254.1 **shared\_with** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shared_with</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="f7711907-5827-4db9-819c-a1cf3f2d5e3c"></a>

###### 2.1.2.6.2.255 Field **shopify\_product\_id**

###### 2.1.2.6.2.255.1 **shopify\_product\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shopify_product_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer64</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>8304200646946</td></tr></tbody></table>

### <a id="30437f95-1a0d-4bd1-ba56-1cd3e6b7a3e3"></a>

###### 2.1.2.6.2.256 Field **shopify\_product\_name**

###### 2.1.2.6.2.256.1 **shopify\_product\_name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shopify_product_name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Producto Test</td></tr></tbody></table>

### <a id="2717c1bb-7c90-4fbf-83e9-dd8afc75b765"></a>

###### 2.1.2.6.2.257 Field **total\_inventory**

###### 2.1.2.6.2.257.1 **total\_inventory** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>total_inventory</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="6ab0ea65-e90e-4d69-82cc-d81a41b8c1d6"></a>

###### 2.1.2.6.2.258 Field **warehouse**

###### 2.1.2.6.2.258.1 **warehouse** Hierarchy

Parent field: **unified\_products**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#e3e80165-9918-41df-9dd2-f8172e31ee28 class="margin-NaN">data</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e4833a55-6ffa-444d-b5f8-25bb963c7ac1 class="margin-NaN">discount</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ec4b24ec-6e02-41e2-b768-277b867f10ac class="margin-NaN">father_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5acbdc17-e081-451b-9bdf-f178c35a0957 class="margin-NaN">id_father</a></td><td class="no-break-word">objectId,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2ce8cfe5-7729-4a36-9d08-796df8e480e7 class="margin-NaN">id_warehouse_rkf</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b78b79b5-d8d0-4160-916e-55990a4b6a1e class="margin-NaN">price</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7a3c1a5a-20a4-44ec-8cd1-cda7074c257b class="margin-NaN">product_warehouse_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c26de8d5-fb08-4487-89bc-8ad70bed6583 class="margin-NaN">shared_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ab139950-43ab-4d15-b847-51a630f15b2d class="margin-NaN">shipping</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#84e943fd-416c-4dcf-a01f-144c4d2c76fa class="margin-NaN">statistics</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#26e58736-bd32-481b-b724-78b129d4d6ff class="margin-NaN">store_price_equal_to_suggested_price</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#59e1e32e-4c39-466d-b357-335bd36b8bc0 class="margin-NaN">suggested</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ffbcc644-29cd-4006-9e02-d0195d70308e class="margin-NaN">suggested_price</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#666cbe97-7e43-45b1-bdc6-d56436e5eb43 class="margin-NaN">suggestions</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c2952542-ed1e-471a-8fc9-78544e99d250 class="margin-NaN">visible</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#72045e1a-dbdb-45cf-a66c-f0d060be17fa class="margin-NaN">warehouse_price</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.258.2 **warehouse** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>warehouse</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="e3e80165-9918-41df-9dd2-f8172e31ee28"></a>

###### 2.1.2.6.2.259 Field **data**

###### 2.1.2.6.2.259.1 **data** Hierarchy

Parent field: **warehouse**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#40e0d521-5a00-4d48-8fc5-ba250a311d09 class="margin-NaN">db_seller</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e796a6d9-8ac4-4396-8114-f4f11d73a92a class="margin-NaN">dbname</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e4e0e0a6-adef-449d-b73a-cccb5c92784f class="margin-NaN">only_my_stores</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c4f2fc88-2a62-47b0-a2da-56ce5d8f35fe class="margin-NaN">shop</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.259.2 **data** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>data</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="40e0d521-5a00-4d48-8fc5-ba250a311d09"></a>

###### 2.1.2.6.2.260 Field **db\_seller**

###### 2.1.2.6.2.260.1 **db\_seller** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>db_seller</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>testtwodrop_804079258</td></tr></tbody></table>

### <a id="e796a6d9-8ac4-4396-8114-f4f11d73a92a"></a>

###### 2.1.2.6.2.261 Field **dbname**

###### 2.1.2.6.2.261.1 **dbname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dbname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>testtwodrop_804079258</td></tr></tbody></table>

### <a id="e4e0e0a6-adef-449d-b73a-cccb5c92784f"></a>

###### 2.1.2.6.2.262 Field **only\_my\_stores**

###### 2.1.2.6.2.262.1 **only\_my\_stores** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>only_my_stores</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="c4f2fc88-2a62-47b0-a2da-56ce5d8f35fe"></a>

###### 2.1.2.6.2.263 Field **shop**

###### 2.1.2.6.2.263.1 **shop** Hierarchy

Parent field: **data**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#7e65a5b1-d939-4514-bbab-697f2f2bc641 class="margin-NaN">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#06baa3ae-54c1-4999-ac14-0bca778dfb4a class="margin-NaN">carry</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2a1582dd-0b38-40e3-a8df-67a9c04c77a5 class="margin-NaN">cc_nit</a></td><td class="no-break-word">string,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6cd874cb-eed3-40c3-b240-273886a7ca63 class="margin-NaN">city</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f10c9485-46bd-422e-a784-1d230161e2dc class="margin-NaN">cod_postal</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7cd4c528-9939-4840-849d-5addea177080 class="margin-NaN">color_primary</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#033149d2-bab4-4f3e-9f7a-4993f4522e68 class="margin-NaN">colors</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ffc29497-3bc3-4c25-b1e5-4247ecc08740 class="margin-NaN">composed_address</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0e75cc1c-bccc-4ae7-80f7-72b72ebf05e4 class="margin-NaN">country</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#686a0002-75b0-40aa-9a37-d84fab3c0ff4 class="margin-NaN">default</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#36e281d5-2127-4119-8084-691285e03899 class="margin-NaN">departament</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fcbc1d2b-7348-4a8b-b6cb-4dfb1d0f080c class="margin-NaN">email</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#967dfd8e-7118-492a-8c76-12962d552f52 class="margin-NaN">geolocation</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f93ba1c6-00a0-4291-bf24-955562564b0e class="margin-NaN">gtag</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7ca8d788-bcee-49ad-a16f-45838a54b984 class="margin-NaN">horary</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f93e272d-e34e-41b8-b809-ce5171cce55b class="margin-NaN">indicative</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2e23ea77-eeae-49c1-b721-52f84300224e class="margin-NaN">large_description</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6c807e3c-8853-4be0-a7f9-7b177de01270 class="margin-NaN">location</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#42b69d98-d5e7-4c25-9331-42f750589b0e class="margin-NaN">logo</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8e0795ca-dfe8-4865-b0c5-78e80af5bceb class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5a4be2ef-7c85-4be7-b056-1f4f6002a48c class="margin-NaN">neighborhood</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#519b049e-99dc-4ecf-9bdf-0cb1bf91a944 class="margin-NaN">pixel</a></td><td class="no-break-word">null,numeric,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#efd5e92b-a342-4742-a637-58785888a51e class="margin-NaN">principal_address</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2cf05f1b-5a17-426d-96c8-72bd5b8fbea3 class="margin-NaN">promises</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ca285719-ebd6-45b1-a009-bedefbab25c5 class="margin-NaN">slogan</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.263.2 **shop** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shop</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="7e65a5b1-d939-4514-bbab-697f2f2bc641"></a>

###### 2.1.2.6.2.264 Field **address**

###### 2.1.2.6.2.264.1 **address** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>address</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Carrera 48 # 45 - 44</td></tr></tbody></table>

### <a id="06baa3ae-54c1-4999-ac14-0bca778dfb4a"></a>

###### 2.1.2.6.2.265 Field **carry**

###### 2.1.2.6.2.265.1 **carry** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>carry</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="2a1582dd-0b38-40e3-a8df-67a9c04c77a5"></a>

###### 2.1.2.6.2.266 Field **cc\_nit**

###### 2.1.2.6.2.266.1 **cc\_nit** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cc_nit</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="6cd874cb-eed3-40c3-b240-273886a7ca63"></a>

###### 2.1.2.6.2.267 Field **city**

###### 2.1.2.6.2.267.1 **city** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#9220dfbf-c565-4bde-a064-0c8fd7d977ab class="margin-NaN">_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#960d825f-91e9-48e5-b94a-9782a1765c51 class="margin-NaN">before_courrier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bb02387e-1f4d-44d1-b7c6-818d9db2c14f class="margin-NaN">checked</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0c05791e-a90b-4f50-9a0c-8bd29cf38d96 class="margin-NaN">city_code</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#61af89b2-cf58-4cc3-a7bb-417fe514c747 class="margin-NaN">cod_depto</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5b72ebd5-fa6a-4b97-80b8-e8e7ddbf8c1e class="margin-NaN">country</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bd457df8-4c80-4ce6-a9fa-ec3934b43e45 class="margin-NaN">courrier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#169ce543-ea82-4f94-b5cf-58f6d32c30e6 class="margin-NaN">dane_code</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9dc4af32-93b4-4e47-9106-1e37d583d081 class="margin-NaN">disabled</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#898dbe2f-51d2-4710-b61b-40d1758bfc98 class="margin-NaN">forTest</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#615ddf5c-583b-4b87-9bfe-72f0b55c022c class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#05e715c5-0117-46ed-9f07-e5f27bec947c class="margin-NaN">postal_code</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#84d87f6d-6d6a-410c-98e2-a55ccf12fd3a class="margin-NaN">shipping_zone</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cd4d3097-8e0d-43ee-9e7e-3026da264318 class="margin-NaN">shop_error</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1b109b23-f5db-491d-8426-0331e6545fba class="margin-NaN">state</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.267.2 **city** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>city</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="9220dfbf-c565-4bde-a064-0c8fd7d977ab"></a>

###### 2.1.2.6.2.268 Field **\_id**

###### 2.1.2.6.2.268.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6047cb9b2a977165ccde8d2c</td></tr></tbody></table>

### <a id="960d825f-91e9-48e5-b94a-9782a1765c51"></a>

###### 2.1.2.6.2.269 Field **before\_courrier**

###### 2.1.2.6.2.269.1 **before\_courrier** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>before_courrier</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>tcc</td></tr></tbody></table>

### <a id="bb02387e-1f4d-44d1-b7c6-818d9db2c14f"></a>

###### 2.1.2.6.2.270 Field **checked**

###### 2.1.2.6.2.270.1 **checked** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>checked</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="0c05791e-a90b-4f50-9a0c-8bd29cf38d96"></a>

###### 2.1.2.6.2.271 Field **city\_code**

###### 2.1.2.6.2.271.1 **city\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>city_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>5001000</td></tr></tbody></table>

### <a id="61af89b2-cf58-4cc3-a7bb-417fe514c747"></a>

###### 2.1.2.6.2.272 Field **cod\_depto**

###### 2.1.2.6.2.272.1 **cod\_depto** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cod_depto</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>05</td></tr></tbody></table>

### <a id="5b72ebd5-fa6a-4b97-80b8-e8e7ddbf8c1e"></a>

###### 2.1.2.6.2.273 Field **country**

###### 2.1.2.6.2.273.1 **country** Hierarchy

Parent field: **city**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#f2b0518c-81f1-423c-999b-d06c8b6cbc4e class="margin-NaN">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#63165f1e-9e7e-4179-8bff-1889c8e74d90 class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ce12c088-65a8-4dbc-8b98-5b9a0a73de42 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.273.2 **country** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="f2b0518c-81f1-423c-999b-d06c8b6cbc4e"></a>

###### 2.1.2.6.2.274 Field **code**

###### 2.1.2.6.2.274.1 **code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>COL</td></tr></tbody></table>

### <a id="63165f1e-9e7e-4179-8bff-1889c8e74d90"></a>

###### 2.1.2.6.2.275 Field **id**

###### 2.1.2.6.2.275.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6047cb912a977165ccde8cd1</td></tr></tbody></table>

### <a id="ce12c088-65a8-4dbc-8b98-5b9a0a73de42"></a>

###### 2.1.2.6.2.276 Field **name**

###### 2.1.2.6.2.276.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Colombia</td></tr></tbody></table>

### <a id="bd457df8-4c80-4ce6-a9fa-ec3934b43e45"></a>

###### 2.1.2.6.2.277 Field **courrier**

###### 2.1.2.6.2.277.1 **courrier** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>courrier</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>servientrega</td></tr></tbody></table>

### <a id="169ce543-ea82-4f94-b5cf-58f6d32c30e6"></a>

###### 2.1.2.6.2.278 Field **dane\_code**

###### 2.1.2.6.2.278.1 **dane\_code** Hierarchy

Parent field: **city**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#7348ec48-4648-4cd5-8038-5dee6679a70a class="margin-NaN">rocketfy</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0aa56542-2d12-41a2-ad8d-5f393f954867 class="margin-NaN">servientrega</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.278.2 **dane\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dane_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="7348ec48-4648-4cd5-8038-5dee6679a70a"></a>

###### 2.1.2.6.2.279 Field **rocketfy**

###### 2.1.2.6.2.279.1 **rocketfy** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>rocketfy</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>05360</td></tr></tbody></table>

### <a id="0aa56542-2d12-41a2-ad8d-5f393f954867"></a>

###### 2.1.2.6.2.280 Field **servientrega**

###### 2.1.2.6.2.280.1 **servientrega** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>servientrega</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>05360</td></tr></tbody></table>

### <a id="9dc4af32-93b4-4e47-9106-1e37d583d081"></a>

###### 2.1.2.6.2.281 Field **disabled**

###### 2.1.2.6.2.281.1 **disabled** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>disabled</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="898dbe2f-51d2-4710-b61b-40d1758bfc98"></a>

###### 2.1.2.6.2.282 Field **forTest**

###### 2.1.2.6.2.282.1 **forTest** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>forTest</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="615ddf5c-583b-4b87-9bfe-72f0b55c022c"></a>

###### 2.1.2.6.2.283 Field **name**

###### 2.1.2.6.2.283.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Itagui</td></tr></tbody></table>

### <a id="05e715c5-0117-46ed-9f07-e5f27bec947c"></a>

###### 2.1.2.6.2.284 Field **postal\_code**

###### 2.1.2.6.2.284.1 **postal\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>postal_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="84d87f6d-6d6a-410c-98e2-a55ccf12fd3a"></a>

###### 2.1.2.6.2.285 Field **shipping\_zone**

###### 2.1.2.6.2.285.1 **shipping\_zone** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shipping_zone</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="cd4d3097-8e0d-43ee-9e7e-3026da264318"></a>

###### 2.1.2.6.2.286 Field **shop\_error**

###### 2.1.2.6.2.286.1 **shop\_error** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shop_error</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="1b109b23-f5db-491d-8426-0331e6545fba"></a>

###### 2.1.2.6.2.287 Field **state**

###### 2.1.2.6.2.287.1 **state** Hierarchy

Parent field: **city**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#611a4139-1328-46ff-b487-6f630f3c8947 class="margin-NaN">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#09084d0d-ad82-4c08-8eaa-6cf784e7b1dc class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#79262244-802b-4918-b0b2-6cd6d8629f12 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.287.2 **state** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>state</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="611a4139-1328-46ff-b487-6f630f3c8947"></a>

###### 2.1.2.6.2.288 Field **code**

###### 2.1.2.6.2.288.1 **code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>05</td></tr></tbody></table>

### <a id="09084d0d-ad82-4c08-8eaa-6cf784e7b1dc"></a>

###### 2.1.2.6.2.289 Field **id**

###### 2.1.2.6.2.289.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6047cb912a977165ccde8cd2</td></tr></tbody></table>

### <a id="79262244-802b-4918-b0b2-6cd6d8629f12"></a>

###### 2.1.2.6.2.290 Field **name**

###### 2.1.2.6.2.290.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Antioquia</td></tr></tbody></table>

### <a id="f10c9485-46bd-422e-a784-1d230161e2dc"></a>

###### 2.1.2.6.2.291 Field **cod\_postal**

###### 2.1.2.6.2.291.1 **cod\_postal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cod_postal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>050021</td></tr></tbody></table>

### <a id="7cd4c528-9939-4840-849d-5addea177080"></a>

###### 2.1.2.6.2.292 Field **color\_primary**

###### 2.1.2.6.2.292.1 **color\_primary** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>color_primary</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>#161114</td></tr></tbody></table>

### <a id="033149d2-bab4-4f3e-9f7a-4993f4522e68"></a>

###### 2.1.2.6.2.293 Field **colors**

###### 2.1.2.6.2.293.1 **colors** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#4ece7366-6291-455f-a769-f9afa0ca5712 class="margin-NaN">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.293.2 **colors** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>colors</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="4ece7366-6291-455f-a769-f9afa0ca5712"></a>

###### 2.1.2.6.2.294 Field **\[0\]**

###### 2.1.2.6.2.294.1 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Sample</td><td>#756055</td></tr></tbody></table>

### <a id="ffc29497-3bc3-4c25-b1e5-4247ecc08740"></a>

###### 2.1.2.6.2.295 Field **composed\_address**

###### 2.1.2.6.2.295.1 **composed\_address** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#4aa1b272-4188-440f-b02a-d70f826eb269 class="margin-NaN">street</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9f912897-2bba-40fc-84f5-f10901eb5c85 class="margin-NaN">street_number_one</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#661cbb86-5e92-4ab2-9052-56aff6284552 class="margin-NaN">street_number_two</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.295.2 **composed\_address** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>composed_address</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="4aa1b272-4188-440f-b02a-d70f826eb269"></a>

###### 2.1.2.6.2.296 Field **street**

###### 2.1.2.6.2.296.1 **street** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>street</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Carrera 48</td></tr></tbody></table>

### <a id="9f912897-2bba-40fc-84f5-f10901eb5c85"></a>

###### 2.1.2.6.2.297 Field **street\_number\_one**

###### 2.1.2.6.2.297.1 **street\_number\_one** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>street_number_one</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>45</td></tr></tbody></table>

### <a id="661cbb86-5e92-4ab2-9052-56aff6284552"></a>

###### 2.1.2.6.2.298 Field **street\_number\_two**

###### 2.1.2.6.2.298.1 **street\_number\_two** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>street_number_two</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>44</td></tr></tbody></table>

### <a id="0e75cc1c-bccc-4ae7-80f7-72b72ebf05e4"></a>

###### 2.1.2.6.2.299 Field **country**

###### 2.1.2.6.2.299.1 **country** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>COL</td></tr></tbody></table>

### <a id="686a0002-75b0-40aa-9a37-d84fab3c0ff4"></a>

###### 2.1.2.6.2.300 Field **default**

###### 2.1.2.6.2.300.1 **default** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>default</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="36e281d5-2127-4119-8084-691285e03899"></a>

###### 2.1.2.6.2.301 Field **departament**

###### 2.1.2.6.2.301.1 **departament** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#813e50ab-c900-4e0b-be26-4c2b46126366 class="margin-NaN">_id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#46ecf093-6038-4d7d-ba5b-5eeb2055d500 class="margin-NaN">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#08a01672-1f13-4ec7-a1e9-25659f4039db class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.301.2 **departament** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>departament</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="813e50ab-c900-4e0b-be26-4c2b46126366"></a>

###### 2.1.2.6.2.302 Field **\_id**

###### 2.1.2.6.2.302.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6047cb912a977165ccde8cd2</td></tr></tbody></table>

### <a id="46ecf093-6038-4d7d-ba5b-5eeb2055d500"></a>

###### 2.1.2.6.2.303 Field **code**

###### 2.1.2.6.2.303.1 **code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>05</td></tr></tbody></table>

### <a id="08a01672-1f13-4ec7-a1e9-25659f4039db"></a>

###### 2.1.2.6.2.304 Field **name**

###### 2.1.2.6.2.304.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Antioquia</td></tr></tbody></table>

### <a id="fcbc1d2b-7348-4a8b-b6cb-4dfb1d0f080c"></a>

###### 2.1.2.6.2.305 Field **email**

###### 2.1.2.6.2.305.1 **email** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>email</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>asccmml@adfaf.co</td></tr></tbody></table>

### <a id="967dfd8e-7118-492a-8c76-12962d552f52"></a>

###### 2.1.2.6.2.306 Field **geolocation**

###### 2.1.2.6.2.306.1 **geolocation** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#4d3e176f-7470-43f9-9b86-3945033fa12d class="margin-NaN">lat</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3299679b-dfcd-45fc-9d81-4a6f3c6cdbdb class="margin-NaN">lng</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.306.2 **geolocation** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>geolocation</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="4d3e176f-7470-43f9-9b86-3945033fa12d"></a>

###### 2.1.2.6.2.307 Field **lat**

###### 2.1.2.6.2.307.1 **lat** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>lat</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="3299679b-dfcd-45fc-9d81-4a6f3c6cdbdb"></a>

###### 2.1.2.6.2.308 Field **lng**

###### 2.1.2.6.2.308.1 **lng** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>lng</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="f93ba1c6-00a0-4291-bf24-955562564b0e"></a>

###### 2.1.2.6.2.309 Field **gtag**

###### 2.1.2.6.2.309.1 **gtag** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>gtag</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="7ca8d788-bcee-49ad-a16f-45838a54b984"></a>

###### 2.1.2.6.2.310 Field **horary**

###### 2.1.2.6.2.310.1 **horary** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#30cc4162-3cc2-4faa-8184-c01eb7e6c6c4 class="margin-NaN">final_horary</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d51cd821-c3b4-4e55-af0b-6f6708054bb7 class="margin-NaN">init_horary</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.310.2 **horary** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>horary</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="30cc4162-3cc2-4faa-8184-c01eb7e6c6c4"></a>

###### 2.1.2.6.2.311 Field **final\_horary**

###### 2.1.2.6.2.311.1 **final\_horary** Hierarchy

Parent field: **horary**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#8a0c69bd-2938-47ee-a682-576c48273550 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c8c085ae-3616-4f71-a7e6-5be133b66623 class="margin-NaN">value</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.311.2 **final\_horary** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>final_horary</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="8a0c69bd-2938-47ee-a682-576c48273550"></a>

###### 2.1.2.6.2.312 Field **name**

###### 2.1.2.6.2.312.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6 p.m.</td></tr></tbody></table>

### <a id="c8c085ae-3616-4f71-a7e6-5be133b66623"></a>

###### 2.1.2.6.2.313 Field **value**

###### 2.1.2.6.2.313.1 **value** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>value</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>19</td></tr></tbody></table>

### <a id="d51cd821-c3b4-4e55-af0b-6f6708054bb7"></a>

###### 2.1.2.6.2.314 Field **init\_horary**

###### 2.1.2.6.2.314.1 **init\_horary** Hierarchy

Parent field: **horary**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#5803505b-a05f-4f02-bae7-2cfe80b89204 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e8abbaeb-5674-4a5f-b9d1-1e7755868c21 class="margin-NaN">value</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.314.2 **init\_horary** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>init_horary</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="5803505b-a05f-4f02-bae7-2cfe80b89204"></a>

###### 2.1.2.6.2.315 Field **name**

###### 2.1.2.6.2.315.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>8 a.m.</td></tr></tbody></table>

### <a id="e8abbaeb-5674-4a5f-b9d1-1e7755868c21"></a>

###### 2.1.2.6.2.316 Field **value**

###### 2.1.2.6.2.316.1 **value** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>value</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>10</td></tr></tbody></table>

### <a id="f93e272d-e34e-41b8-b809-ce5171cce55b"></a>

###### 2.1.2.6.2.317 Field **indicative**

###### 2.1.2.6.2.317.1 **indicative** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>indicative</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>57</td></tr></tbody></table>

### <a id="2e23ea77-eeae-49c1-b721-52f84300224e"></a>

###### 2.1.2.6.2.318 Field **large\_description**

###### 2.1.2.6.2.318.1 **large\_description** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>large_description</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="6c807e3c-8853-4be0-a7f9-7b177de01270"></a>

###### 2.1.2.6.2.319 Field **location**

###### 2.1.2.6.2.319.1 **location** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#550f09fb-b9bd-434c-8b96-b145a9cba7e7 class="margin-NaN">lat</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2484af52-eabb-49ef-a3a3-4916ebf1a1fa class="margin-NaN">lng</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.319.2 **location** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>location</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="550f09fb-b9bd-434c-8b96-b145a9cba7e7"></a>

###### 2.1.2.6.2.320 Field **lat**

###### 2.1.2.6.2.320.1 **lat** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>lat</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>4.620459299999999</td></tr></tbody></table>

### <a id="2484af52-eabb-49ef-a3a3-4916ebf1a1fa"></a>

###### 2.1.2.6.2.321 Field **lng**

###### 2.1.2.6.2.321.1 **lng** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>lng</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>-74.073411</td></tr></tbody></table>

### <a id="42b69d98-d5e7-4c25-9331-42f750589b0e"></a>

###### 2.1.2.6.2.322 Field **logo**

###### 2.1.2.6.2.322.1 **logo** Hierarchy

Parent field: **shop**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#980c4dce-931c-4713-8ee6-ca1794ffd26f class="margin-NaN">acl</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cf525fe7-1634-4206-a1c0-4a4ac1a700b4 class="margin-NaN">bucket</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#763f18e3-3ae3-4d3e-9cbc-881801103852 class="margin-NaN">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ef9220da-7eb6-46d4-b634-4a8664761019 class="margin-NaN">contentType</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#19e499c1-0b11-453b-9bca-6dda8f019a62 class="margin-NaN">created_time</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b817ddc3-485b-4117-a8fb-3fbaeeac9594 class="margin-NaN">encoding</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#075f14be-43df-4a76-89e8-ed8c7afa0053 class="margin-NaN">etag</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6aeb826d-248e-41fa-b08b-ff0d33a278e9 class="margin-NaN">fieldname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#29975f23-cff6-4c35-a239-679ad7ab4b3f class="margin-NaN">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b78587fc-5d41-49ea-8482-bc13d09e7dce class="margin-NaN">location</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9fef7e49-239e-49e1-a665-6fae0b443467 class="margin-NaN">metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cc625345-5009-4946-b616-ced89f6c768a class="margin-NaN">mimetype</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#084bdb92-951c-4d99-9f81-502e94529e4c class="margin-NaN">originalname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#47755034-235c-4bdc-af2a-7382a21e7cbc class="margin-NaN">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a78607c9-ad68-4265-a665-3d37ca123ddf class="margin-NaN">size</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#23f0e8e4-7ba6-445f-92e6-2528ba397b41 class="margin-NaN">storageClass</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ed64d430-c645-4d46-97b1-0b7ba3595348 class="margin-NaN">versionId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.322.2 **logo** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>logo</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="980c4dce-931c-4713-8ee6-ca1794ffd26f"></a>

###### 2.1.2.6.2.323 Field **acl**

###### 2.1.2.6.2.323.1 **acl** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>acl</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>public-read</td></tr></tbody></table>

### <a id="cf525fe7-1634-4206-a1c0-4a4ac1a700b4"></a>

###### 2.1.2.6.2.324 Field **bucket**

###### 2.1.2.6.2.324.1 **bucket** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>bucket</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>shopping-rocketfy-uploads</td></tr></tbody></table>

### <a id="763f18e3-3ae3-4d3e-9cbc-881801103852"></a>

###### 2.1.2.6.2.325 Field **contentDisposition**

###### 2.1.2.6.2.325.1 **contentDisposition** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentDisposition</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ef9220da-7eb6-46d4-b634-4a8664761019"></a>

###### 2.1.2.6.2.326 Field **contentType**

###### 2.1.2.6.2.326.1 **contentType** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentType</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="19e499c1-0b11-453b-9bca-6dda8f019a62"></a>

###### 2.1.2.6.2.327 Field **created\_time**

###### 2.1.2.6.2.327.1 **created\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="b817ddc3-485b-4117-a8fb-3fbaeeac9594"></a>

###### 2.1.2.6.2.328 Field **encoding**

###### 2.1.2.6.2.328.1 **encoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>encoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>7bit</td></tr></tbody></table>

### <a id="075f14be-43df-4a76-89e8-ed8c7afa0053"></a>

###### 2.1.2.6.2.329 Field **etag**

###### 2.1.2.6.2.329.1 **etag** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>etag</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>"6e3aad264a7efb2be5567ecc968adac6"</td></tr></tbody></table>

### <a id="6aeb826d-248e-41fa-b08b-ff0d33a278e9"></a>

###### 2.1.2.6.2.330 Field **fieldname**

###### 2.1.2.6.2.330.1 **fieldname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="29975f23-cff6-4c35-a239-679ad7ab4b3f"></a>

###### 2.1.2.6.2.331 Field **key**

###### 2.1.2.6.2.331.1 **key** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>key</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>testtwodrop_804079258_121642999_10221463163479893_6069666320517077970_n44.jpg</td></tr></tbody></table>

### <a id="b78587fc-5d41-49ea-8482-bc13d09e7dce"></a>

###### 2.1.2.6.2.332 Field **location**

###### 2.1.2.6.2.332.1 **location** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>location</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://shopping-rocketfy-uploads.s3.amazonaws.com/testtwodrop_804079258_121642999_10221463163479893_6069666320517077970_n44.jpg</td></tr></tbody></table>

### <a id="9fef7e49-239e-49e1-a665-6fae0b443467"></a>

###### 2.1.2.6.2.333 Field **metadata**

###### 2.1.2.6.2.333.1 **metadata** Hierarchy

Parent field: **logo**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#dace8dad-78f0-474d-87b6-a1ebfe1e5245 class="margin-NaN">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#502a48b0-dcb0-4fa4-b9fd-d0b25de63778 class="margin-NaN">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.333.2 **metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="dace8dad-78f0-474d-87b6-a1ebfe1e5245"></a>

###### 2.1.2.6.2.334 Field **Content-Type**

###### 2.1.2.6.2.334.1 **Content-Type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Content-Type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="502a48b0-dcb0-4fa4-b9fd-d0b25de63778"></a>

###### 2.1.2.6.2.335 Field **fieldName**

###### 2.1.2.6.2.335.1 **fieldName** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldName</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="cc625345-5009-4946-b616-ced89f6c768a"></a>

###### 2.1.2.6.2.336 Field **mimetype**

###### 2.1.2.6.2.336.1 **mimetype** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mimetype</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="084bdb92-951c-4d99-9f81-502e94529e4c"></a>

###### 2.1.2.6.2.337 Field **originalname**

###### 2.1.2.6.2.337.1 **originalname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>originalname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>testtwodrop_804079258_121642999_10221463163479893_6069666320517077970_n44.jpg</td></tr></tbody></table>

### <a id="47755034-235c-4bdc-af2a-7382a21e7cbc"></a>

###### 2.1.2.6.2.338 Field **serverSideEncryption**

###### 2.1.2.6.2.338.1 **serverSideEncryption** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>serverSideEncryption</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a78607c9-ad68-4265-a665-3d37ca123ddf"></a>

###### 2.1.2.6.2.339 Field **size**

###### 2.1.2.6.2.339.1 **size** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>size</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>568993</td></tr></tbody></table>

### <a id="23f0e8e4-7ba6-445f-92e6-2528ba397b41"></a>

###### 2.1.2.6.2.340 Field **storageClass**

###### 2.1.2.6.2.340.1 **storageClass** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>storageClass</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>STANDARD</td></tr></tbody></table>

### <a id="ed64d430-c645-4d46-97b1-0b7ba3595348"></a>

###### 2.1.2.6.2.341 Field **versionId**

###### 2.1.2.6.2.341.1 **versionId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>versionId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>YwuL_Q7QgcwdEMBRJZnahbpqpbdwlb.R</td></tr></tbody></table>

### <a id="8e0795ca-dfe8-4865-b0c5-78e80af5bceb"></a>

###### 2.1.2.6.2.342 Field **name**

###### 2.1.2.6.2.342.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>test two drop</td></tr></tbody></table>

### <a id="5a4be2ef-7c85-4be7-b056-1f4f6002a48c"></a>

###### 2.1.2.6.2.343 Field **neighborhood**

###### 2.1.2.6.2.343.1 **neighborhood** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>neighborhood</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Itagui</td></tr></tbody></table>

### <a id="519b049e-99dc-4ecf-9bdf-0cb1bf91a944"></a>

###### 2.1.2.6.2.344 Field **pixel**

###### 2.1.2.6.2.344.1 **pixel** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>pixel</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,numeric,string)</td></tr><tr><td></td><td>[object Object],[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="efd5e92b-a342-4742-a637-58785888a51e"></a>

###### 2.1.2.6.2.345 Field **principal\_address**

###### 2.1.2.6.2.345.1 **principal\_address** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>principal_address</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>5ffe1ef85bc63e1b073c33a8</td></tr></tbody></table>

### <a id="2cf05f1b-5a17-426d-96c8-72bd5b8fbea3"></a>

###### 2.1.2.6.2.346 Field **promises**

###### 2.1.2.6.2.346.1 **promises** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>promises</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ca285719-ebd6-45b1-a009-bedefbab25c5"></a>

###### 2.1.2.6.2.347 Field **slogan**

###### 2.1.2.6.2.347.1 **slogan** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>slogan</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="e4833a55-6ffa-444d-b5f8-25bb963c7ac1"></a>

###### 2.1.2.6.2.348 Field **discount**

###### 2.1.2.6.2.348.1 **discount** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>discount</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ec4b24ec-6e02-41e2-b768-277b867f10ac"></a>

###### 2.1.2.6.2.349 Field **father\_id**

###### 2.1.2.6.2.349.1 **father\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>father_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>601dd177fa8844010c99136e</td></tr></tbody></table>

### <a id="5acbdc17-e081-451b-9bdf-f178c35a0957"></a>

###### 2.1.2.6.2.350 Field **id\_father**

###### 2.1.2.6.2.350.1 **id\_father** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id_father</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (objectId,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="2ce8cfe5-7729-4a36-9d08-796df8e480e7"></a>

###### 2.1.2.6.2.351 Field **id\_warehouse\_rkf**

###### 2.1.2.6.2.351.1 **id\_warehouse\_rkf** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id_warehouse_rkf</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>601dd177fa8844010c991377</td></tr></tbody></table>

### <a id="b78b79b5-d8d0-4160-916e-55990a4b6a1e"></a>

###### 2.1.2.6.2.352 Field **price**

###### 2.1.2.6.2.352.1 **price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="7a3c1a5a-20a4-44ec-8cd1-cda7074c257b"></a>

###### 2.1.2.6.2.353 Field **product\_warehouse\_id**

###### 2.1.2.6.2.353.1 **product\_warehouse\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>product_warehouse_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>602ab3bade09a83fb2bc4163</td></tr></tbody></table>

### <a id="c26de8d5-fb08-4487-89bc-8ad70bed6583"></a>

###### 2.1.2.6.2.354 Field **shared\_id**

###### 2.1.2.6.2.354.1 **shared\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shared_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>601993761193ff13ac9f8007</td></tr></tbody></table>

### <a id="ab139950-43ab-4d15-b847-51a630f15b2d"></a>

###### 2.1.2.6.2.355 Field **shipping**

###### 2.1.2.6.2.355.1 **shipping** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shipping</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="84e943fd-416c-4dcf-a01f-144c4d2c76fa"></a>

###### 2.1.2.6.2.356 Field **statistics**

###### 2.1.2.6.2.356.1 **statistics** Hierarchy

Parent field: **warehouse**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#97702d1f-e38a-416e-b4e1-2ae5ff7c7751 class="margin-NaN">imports</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a1843152-e4bb-4614-b126-795c939abbee class="margin-NaN">sales</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.356.2 **statistics** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>statistics</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="97702d1f-e38a-416e-b4e1-2ae5ff7c7751"></a>

###### 2.1.2.6.2.357 Field **imports**

###### 2.1.2.6.2.357.1 **imports** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>imports</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1013</td></tr></tbody></table>

### <a id="a1843152-e4bb-4614-b126-795c939abbee"></a>

###### 2.1.2.6.2.358 Field **sales**

###### 2.1.2.6.2.358.1 **sales** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>sales</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="26e58736-bd32-481b-b724-78b129d4d6ff"></a>

###### 2.1.2.6.2.359 Field **store\_price\_equal\_to\_suggested\_price**

###### 2.1.2.6.2.359.1 **store\_price\_equal\_to\_suggested\_price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>store_price_equal_to_suggested_price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="59e1e32e-4c39-466d-b357-335bd36b8bc0"></a>

###### 2.1.2.6.2.360 Field **suggested**

###### 2.1.2.6.2.360.1 **suggested** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>suggested</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="ffbcc644-29cd-4006-9e02-d0195d70308e"></a>

###### 2.1.2.6.2.361 Field **suggested\_price**

###### 2.1.2.6.2.361.1 **suggested\_price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>suggested_price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>500022</td></tr></tbody></table>

### <a id="666cbe97-7e43-45b1-bdc6-d56436e5eb43"></a>

###### 2.1.2.6.2.362 Field **suggestions**

###### 2.1.2.6.2.362.1 **suggestions** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>suggestions</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c2952542-ed1e-471a-8fc9-78544e99d250"></a>

###### 2.1.2.6.2.363 Field **visible**

###### 2.1.2.6.2.363.1 **visible** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>visible</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="72045e1a-dbdb-45cf-a66c-f0d060be17fa"></a>

###### 2.1.2.6.2.364 Field **warehouse\_price**

###### 2.1.2.6.2.364.1 **warehouse\_price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>warehouse_price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a2d3d7c3-e6dc-4a85-9876-3fe1aa2ae0ab"></a>

###### 2.1.2.6.2.365 Field **woo\_product\_id**

###### 2.1.2.6.2.365.1 **woo\_product\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>woo_product_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>94</td></tr></tbody></table>

### <a id="205be59b-4145-4848-8e62-2defdcf046d4"></a>

###### 2.1.2.6.2.366 Field **woo\_product\_name**

###### 2.1.2.6.2.366.1 **woo\_product\_name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>woo_product_name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Hoodie Rocketfy</td></tr></tbody></table>

###### 2.1.2.6.3 **unified\_products** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">visible_-1</td><td class="table-column-property">import_-1</td><td class="table-column-property">slug_-1</td><td class="table-column-property">created_time_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">visible_-1</td><td class="table-column-indexes">import_-1</td><td class="table-column-indexes">slug_-1</td><td class="table-column-indexes">created_time_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">undefined('ascending')</td><td class="table-column-indexes">undefined('descending')</td><td class="table-column-indexes">undefined('descending')</td><td class="table-column-indexes">undefined('descending')</td><td class="table-column-indexes">undefined('descending')</td></tr></tbody></table>

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">variations.inventory_id_1</td><td class="table-column-property">category.id_-1</td><td class="table-column-property">establishment_identifier_-1_created_time_-1</td><td class="table-column-property">establishment_identifier_-1_warehouse.shared_id_-1</td><td class="table-column-property">name_text</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">variations.inventory_id_1</td><td class="table-column-indexes">category.id_-1</td><td class="table-column-indexes">establishment_identifier_-1_created_time_-1</td><td class="table-column-indexes">establishment_identifier_-1_warehouse.shared_id_-1</td><td class="table-column-indexes">name_text</td></tr><tr><td>Key</td><td class="table-column-indexes">inventory_id('ascending')</td><td class="table-column-indexes"></td><td class="table-column-indexes">undefined('descending'), undefined('descending')</td><td class="table-column-indexes">undefined('descending'), shared_id('descending')</td><td class="table-column-indexes">undefined('text')</td></tr></tbody></table>

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">variations._id_1</td><td class="table-column-property">shopify_product_id_1_variations.shopify_variant_id_1</td><td class="table-column-property">establishment_identifier_1_shopify_product_id_1</td><td class="table-column-property">variations.variation_id_1_shared_1_visible_1</td><td class="table-column-property">country_ref.iso3_1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">variations._id_1</td><td class="table-column-indexes">shopify_product_id_1_variations.shopify_variant_id_1</td><td class="table-column-indexes">establishment_identifier_1_shopify_product_id_1</td><td class="table-column-indexes">variations.variation_id_1_shared_1_visible_1</td><td class="table-column-indexes">country_ref.iso3_1</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">undefined('ascending'), shopify_variant_id('ascending')</td><td class="table-column-indexes">undefined('ascending'), undefined('ascending')</td><td class="table-column-indexes">variation_id('ascending'), undefined('ascending'), undefined('ascending')</td><td class="table-column-indexes">iso3('ascending')</td></tr></tbody></table>

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">warehouse.shared_id_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">warehouse.shared_id_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">shared_id('descending')</td></tr></tbody></table>

### <a id="relationships"></a>

## 3\. Relationships

### <a id="0ad7ae99-e80c-4e35-a43c-7126b3c4ab03"></a>

### 3.7 Relationship **products-variations**

#### 3.7.1 **products-variations** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#9e7d9462-9ccb-449b-a053-38685a5f26cd>unified_products</a></td><td><a href=#3db8b469-67f6-4984-be67-c8e18f1e40fe>variations.[-1]._id</a></td></tr></tbody></table>

![Hackolade image](Modulo-dropshipping/image15.png?raw=true)![Hackolade image](Modulo-dropshipping/image16.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#d074212d-2fa6-426a-91f6-8ae358bcca95>unified_variations</a></td><td><a href=#9950b4f8-54a7-48e0-9612-f77fc94596f8>_id</a></td></tr></tbody></table>

#### 3.7.2 **products-variations** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>products-variations</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#9e7d9462-9ccb-449b-a053-38685a5f26cd>unified_products</a></td></tr><tr><td>Parent field</td><td><a href=#3db8b469-67f6-4984-be67-c8e18f1e40fe>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#d074212d-2fa6-426a-91f6-8ae358bcca95>unified_variations</a></td></tr><tr><td>Child field</td><td><a href=#9950b4f8-54a7-48e0-9612-f77fc94596f8>_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="fae6f210-947b-4b1e-8e59-f676ff6e0aa2"></a>

### 3.8 Relationship **products-inventories**

#### 3.8.1 **products-inventories** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#9e7d9462-9ccb-449b-a053-38685a5f26cd>unified_products</a></td><td><a href=#f8acffc8-769b-4713-ae33-d525e050fb49>variations.[-1].inventory_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-dropshipping/image17.png?raw=true)![Hackolade image](Modulo-dropshipping/image18.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#7dbbb739-9112-4fed-8747-72e93d10c0d8>unified_inventories</a></td><td><a href=#49690ee3-a80c-40fd-a8df-9f81d77e3fb6>_id</a></td></tr></tbody></table>

#### 3.8.2 **products-inventories** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>products-inventories</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#9e7d9462-9ccb-449b-a053-38685a5f26cd>unified_products</a></td></tr><tr><td>Parent field</td><td><a href=#f8acffc8-769b-4713-ae33-d525e050fb49>inventory_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#7dbbb739-9112-4fed-8747-72e93d10c0d8>unified_inventories</a></td></tr><tr><td>Child field</td><td><a href=#49690ee3-a80c-40fd-a8df-9f81d77e3fb6>_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="42ea0620-581d-4451-9973-7e6dc61a8648"></a>

### 3.9 Relationship **customers-products**

#### 3.9.1 **customers-products** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#ec559fb7-4dbc-4d80-912e-a1628c5130b4>customers</a></td><td><a href=#7fa9b648-96f2-4145-b5c0-11a173cd0b0e>dbname</a></td></tr></tbody></table>

![Hackolade image](Modulo-dropshipping/image19.png?raw=true)![Hackolade image](Modulo-dropshipping/image20.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#9e7d9462-9ccb-449b-a053-38685a5f26cd>unified_products</a></td><td><a href=#7fe1d3f5-2828-4c9e-978a-a54d10f6d4ae>establishment_identifier</a></td></tr></tbody></table>

#### 3.9.2 **customers-products** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>customers-products</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#ec559fb7-4dbc-4d80-912e-a1628c5130b4>customers</a></td></tr><tr><td>Parent field</td><td><a href=#7fa9b648-96f2-4145-b5c0-11a173cd0b0e>dbname</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#9e7d9462-9ccb-449b-a053-38685a5f26cd>unified_products</a></td></tr><tr><td>Child field</td><td><a href=#7fe1d3f5-2828-4c9e-978a-a54d10f6d4ae>establishment_identifier</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="ca9bfddb-da39-4704-82d6-5f7fc21a64d0"></a>

### 3.10 Relationship **warehouse\_imports-warehouse\_products**

#### 3.10.1 **warehouse\_imports-warehouse\_products** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#0caea05c-4c87-43e4-9955-63f1a5327efe>wearehouse_products</a></td><td><a href=#29f0288a-ccf4-405c-949e-93f27f97f667>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-dropshipping/image21.png?raw=true)![Hackolade image](Modulo-dropshipping/image22.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#d9546eb8-72ab-4118-ac98-345b9b52d0e6>warehouse_imports</a></td><td><a href=#871dd2cf-bb8d-4297-9db9-fcde06bbb2b9>product_id</a></td></tr></tbody></table>

#### 3.10.2 **warehouse\_imports-warehouse\_products** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>warehouse_imports-warehouse_products</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#0caea05c-4c87-43e4-9955-63f1a5327efe>wearehouse_products</a></td></tr><tr><td>Parent field</td><td><a href=#29f0288a-ccf4-405c-949e-93f27f97f667>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#d9546eb8-72ab-4118-ac98-345b9b52d0e6>warehouse_imports</a></td></tr><tr><td>Child field</td><td><a href=#871dd2cf-bb8d-4297-9db9-fcde06bbb2b9>product_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

