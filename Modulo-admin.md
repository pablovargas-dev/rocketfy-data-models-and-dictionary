     

### <a id="documentation-body"></a>

![Hackolade image](Modulo-admin/image1.png?raw=true)

Módulo Admin - MongoDB Physical Model
----------------------

#### Schema for:

Model name: Módulo Admin

Author: Rocketfy Development Team

Version: 1.0

### <a id="contents"></a>

*   [Table of Contents](#contents)
*   [1\. Model](#model)
*   [2\. Databases](#containers)
    *   [2.1 rocketfy](#ac7a68bf-ef02-4449-964e-455eda30c57b)
        
        [2.1.2. Collections](#ac7a68bf-ef02-4449-964e-455eda30c57b-children)
        
        [2.1.2.1 users](#635abd72-5aab-496e-a47e-31cf5060165e)
        
        [2.1.2.2 users\_sticker\_guide](#a2628771-9510-48ad-b4bb-3461c7ac2da1)
        
        [2.1.2.3 metrics\_use](#e35d3b15-e7a0-46d4-b3e6-523b15c328fd)
        
        [2.1.2.4 mfa](#9dfd6d06-1625-47c9-806c-ff10078f8786)
        
        [2.1.2.5 user\_sessions](#2620e329-587f-4ad6-936b-0cf39da379f0)
        
        [2.1.2.6 customers](#b3cf6f21-4a4d-4a9d-afec-691df5296b74)
        
*   [3\. Relationships](#relationships)
    *   [3.33 customers-users](#9be71d53-344d-4713-aff2-0adee88bf92e)
    *   [3.34 users-mfa](#5016ed4d-34f1-40c7-805f-580b326b0d00)
    *   [3.35 users-user\_sessions](#792ea2f7-b783-41e2-af95-410ff3dea258)
    *   [3.36 customers-user\_sticker\_guide](#61b45523-079f-46eb-ac68-e6c79a716afb)
    *   [3.37 customers-metrics\_use](#94e62133-7c1f-4ee7-ab8d-f07c6a0bd4e6)

### <a id="model"></a>

## 1\. Model

### 1.1 Model **Rocketfy**

#### 1.1.1 **Rocketfy** Entity Relationship Diagram

![Hackolade image](Modulo-admin/image2.png?raw=true)

#### 1.1.2 **Rocketfy** Properties

##### 1.1.2.1 **Details** tab

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td><span>Model name</span></td><td>Rocketfy</td></tr><tr><td><span>Target</span></td><td>MongoDB</td></tr><tr><td><span>DB version</span></td><td>v8.0</td></tr><tr><td><span>Lineage capture</span></td><td></td></tr></tbody></table>

##### 1.1.2.2 **Options** tab

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

#### 1.1.3 **Rocketfy** DB Definitions

### <a id="containers"></a>

## 2\. Databases

### <a id="ac7a68bf-ef02-4449-964e-455eda30c57b"></a>

### 2.1 Database **rocketfy**

#### 2.1.1 **rocketfy** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Database name</td><td>rocketfy</td></tr><tr><td>Activated</td><td>true</td></tr></tbody></table>

### <a id="ac7a68bf-ef02-4449-964e-455eda30c57b-children"></a>

#### 2.1.2 **rocketfy** Collections

### <a id="635abd72-5aab-496e-a47e-31cf5060165e"></a>

##### 2.1.2.1 Collection **users**

###### 2.1.2.1.1 **users** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>users</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#ac7a68bf-ef02-4449-964e-455eda30c57b><span class="name-container">rocketfy</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.1.2 **users** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#7ded5fdf-322e-4b41-b104-4dda07c2c04c class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk, dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#06395d9c-9f15-442d-b482-7b06b93a474c class="margin-0">dbname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cd4547b7-f02b-4317-b8fc-23d68be8c71a class="margin-0">user</a></td><td class="no-break-word">string</td><td>true</td><td>dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e7fac12d-5edd-403f-8ef1-d3347188b37c class="margin-0">idRol</a></td><td class="no-break-word">string,numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dbff98ec-351a-4317-826d-3b6365572297 class="margin-0">client_id</a></td><td class="no-break-word">string,objectId</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cab235cf-ce83-4e40-b004-5eeab21c7756 class="margin-0">port_asterisk</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#abaf46d2-7b03-4d53-93ad-424dd8c3afb0 class="margin-0">perms</a></td><td class="no-break-word">document,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4a96188f-5834-493f-9089-a077dd16be18 class="margin-5">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1101d8d5-f5c7-4d3c-a1bf-b036d38f64bf class="margin-10">academy</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#eeb76044-0ebc-46fb-8b60-3ea056f54a39 class="margin-10">leads</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4887ed76-2487-4e6d-81ab-dbc0fb2e918b class="margin-10">shopping</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#072dd828-2407-4a28-80d9-f47e152727c8 class="margin-0">activated</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d7cd3d86-0a75-431d-94b4-7e15ff5d7809 class="margin-0">created_date</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a7e6ca7b-1fb0-4dd6-9f3f-63b0748856a9 class="margin-0">status</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d7c64969-50a8-48d9-8b7a-29f9aa024fe6 class="margin-0">hashedPass</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cf8bf07c-5258-46e0-beb8-98a7a180ff0d class="margin-0">mfa</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6b7347e3-acaf-49f6-a048-c6d5c7e1c1ba class="margin-5">email</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c9e4c938-92a2-4070-b0b0-0ef3d39a10f5 class="margin-5">phone</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ba47ee3f-0083-48d3-af0f-b5ebac0e144f class="margin-0">owner</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#759b8722-d3d2-463c-b5a8-5948733b7d5b class="margin-0">blocked_for_payments</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8c17c05b-d66c-46b6-8273-4bbdfadc36de class="margin-0">blocking_from_support</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fa7b4484-9824-415f-ae39-41cf5cee48e1 class="margin-0">establishment_identifier</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#34975757-e447-42cc-a713-73a09440c821 class="margin-0">inactive_user_cluster</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f0315dd9-cace-4196-baa2-31d5ba10515b class="margin-0">mensajeroRol</a></td><td class="no-break-word">null,boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3ee2c595-8234-4fe4-aa01-fb357acf9fff class="margin-0">name</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4b542658-304a-47d3-8082-d5708fe7b982 class="margin-0">phone</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5d6c48e1-42f2-47a7-8778-b6ba1726d4bc class="margin-5">full_number</a></td><td class="no-break-word">string,numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e7a6ec49-4cdb-4d8d-a88a-be2f21cefc2b class="margin-5">indicative</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b60022f9-a9b4-41c2-83d1-bc006f88e079 class="margin-5">number_phone</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#29375ad5-601f-47ea-946a-ca3e2a9bdf1f class="margin-0">rocketId</a></td><td class="no-break-word">objectId</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9fc64250-079b-4a5e-b62a-a0eea7cc7dcb class="margin-0">user_phone</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="7ded5fdf-322e-4b41-b104-4dda07c2c04c"></a>

###### 2.1.2.1.2.1 Field **\_id**

###### 2.1.2.1.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="06395d9c-9f15-442d-b482-7b06b93a474c"></a>

###### 2.1.2.1.2.2 Field **dbname**

###### 2.1.2.1.2.2.1 **dbname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dbname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>loquegustes_305747720</td></tr></tbody></table>

### <a id="cd4547b7-f02b-4317-b8fc-23d68be8c71a"></a>

###### 2.1.2.1.2.3 Field **user**

###### 2.1.2.1.2.3.1 **user** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>user</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>edwinargue@gmail.com</td></tr></tbody></table>

### <a id="e7fac12d-5edd-403f-8ef1-d3347188b37c"></a>

###### 2.1.2.1.2.4 Field **idRol**

###### 2.1.2.1.2.4.1 **idRol** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>idRol</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="dbff98ec-351a-4317-826d-3b6365572297"></a>

###### 2.1.2.1.2.5 Field **client\_id**

###### 2.1.2.1.2.5.1 **client\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>client_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,objectId)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#b3cf6f21-4a4d-4a9d-afec-691df5296b74>customers</a></td></tr><tr><td>Foreign field</td><td><a href=#bd0c7b13-73ce-421c-9eea-7225ef09517d>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="cab235cf-ce83-4e40-b004-5eeab21c7756"></a>

###### 2.1.2.1.2.6 Field **port\_asterisk**

###### 2.1.2.1.2.6.1 **port\_asterisk** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>port_asterisk</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="abaf46d2-7b03-4d53-93ad-424dd8c3afb0"></a>

###### 2.1.2.1.2.7 Field **perms**

###### 2.1.2.1.2.7.1 **perms** Tree Diagram

![Hackolade image](Modulo-admin/image3.png?raw=true)

###### 2.1.2.1.2.7.2 **perms** Hierarchy

Parent field: **users**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#4a96188f-5834-493f-9089-a077dd16be18 class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.1.2.7.3 **perms** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>perms</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (document,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4a96188f-5834-493f-9089-a077dd16be18"></a>

###### 2.1.2.1.2.8 Field **properties**

###### 2.1.2.1.2.8.1 **properties** Tree Diagram

![Hackolade image](Modulo-admin/image4.png?raw=true)

###### 2.1.2.1.2.8.2 **properties** Hierarchy

Parent field: **perms**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#1101d8d5-f5c7-4d3c-a1bf-b036d38f64bf class="margin-NaN">academy</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#eeb76044-0ebc-46fb-8b60-3ea056f54a39 class="margin-NaN">leads</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4887ed76-2487-4e6d-81ab-dbc0fb2e918b class="margin-NaN">shopping</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.1.2.8.3 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="1101d8d5-f5c7-4d3c-a1bf-b036d38f64bf"></a>

###### 2.1.2.1.2.9 Field **academy**

###### 2.1.2.1.2.9.1 **academy** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>academy</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="eeb76044-0ebc-46fb-8b60-3ea056f54a39"></a>

###### 2.1.2.1.2.10 Field **leads**

###### 2.1.2.1.2.10.1 **leads** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>leads</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4887ed76-2487-4e6d-81ab-dbc0fb2e918b"></a>

###### 2.1.2.1.2.11 Field **shopping**

###### 2.1.2.1.2.11.1 **shopping** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shopping</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="072dd828-2407-4a28-80d9-f47e152727c8"></a>

###### 2.1.2.1.2.12 Field **activated**

###### 2.1.2.1.2.12.1 **activated** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>activated</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="d7cd3d86-0a75-431d-94b4-7e15ff5d7809"></a>

###### 2.1.2.1.2.13 Field **created\_date**

###### 2.1.2.1.2.13.1 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1743461260</td></tr></tbody></table>

### <a id="a7e6ca7b-1fb0-4dd6-9f3f-63b0748856a9"></a>

###### 2.1.2.1.2.14 Field **status**

###### 2.1.2.1.2.14.1 **status** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>status</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>active</td></tr></tbody></table>

### <a id="d7c64969-50a8-48d9-8b7a-29f9aa024fe6"></a>

###### 2.1.2.1.2.15 Field **hashedPass**

###### 2.1.2.1.2.15.1 **hashedPass** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>hashedPass</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>$2b$10$8lluLo2u3rblMd8GmpDhYuWkRJ0EaL5vt0JRmpjHaCK6D/bP/mYUK</td></tr></tbody></table>

### <a id="cf8bf07c-5258-46e0-beb8-98a7a180ff0d"></a>

###### 2.1.2.1.2.16 Field **mfa**

###### 2.1.2.1.2.16.1 **mfa** Tree Diagram

![Hackolade image](Modulo-admin/image5.png?raw=true)

###### 2.1.2.1.2.16.2 **mfa** Hierarchy

Parent field: **users**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#6b7347e3-acaf-49f6-a048-c6d5c7e1c1ba class="margin-NaN">email</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c9e4c938-92a2-4070-b0b0-0ef3d39a10f5 class="margin-NaN">phone</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.1.2.16.3 **mfa** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mfa</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="6b7347e3-acaf-49f6-a048-c6d5c7e1c1ba"></a>

###### 2.1.2.1.2.17 Field **email**

###### 2.1.2.1.2.17.1 **email** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>email</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="c9e4c938-92a2-4070-b0b0-0ef3d39a10f5"></a>

###### 2.1.2.1.2.18 Field **phone**

###### 2.1.2.1.2.18.1 **phone** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>phone</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="ba47ee3f-0083-48d3-af0f-b5ebac0e144f"></a>

###### 2.1.2.1.2.19 Field **owner**

###### 2.1.2.1.2.19.1 **owner** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>owner</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="759b8722-d3d2-463c-b5a8-5948733b7d5b"></a>

###### 2.1.2.1.2.20 Field **blocked\_for\_payments**

###### 2.1.2.1.2.20.1 **blocked\_for\_payments** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>blocked_for_payments</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="8c17c05b-d66c-46b6-8273-4bbdfadc36de"></a>

###### 2.1.2.1.2.21 Field **blocking\_from\_support**

###### 2.1.2.1.2.21.1 **blocking\_from\_support** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>blocking_from_support</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="fa7b4484-9824-415f-ae39-41cf5cee48e1"></a>

###### 2.1.2.1.2.22 Field **establishment\_identifier**

###### 2.1.2.1.2.22.1 **establishment\_identifier** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>establishment_identifier</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>rocketfy_customer_tiendavirtual4447_1124779708</td></tr></tbody></table>

### <a id="34975757-e447-42cc-a713-73a09440c821"></a>

###### 2.1.2.1.2.23 Field **inactive\_user\_cluster**

###### 2.1.2.1.2.23.1 **inactive\_user\_cluster** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>inactive_user_cluster</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="f0315dd9-cace-4196-baa2-31d5ba10515b"></a>

###### 2.1.2.1.2.24 Field **mensajeroRol**

###### 2.1.2.1.2.24.1 **mensajeroRol** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mensajeroRol</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,boolean)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="3ee2c595-8234-4fe4-aa01-fb357acf9fff"></a>

###### 2.1.2.1.2.25 Field **name**

###### 2.1.2.1.2.25.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4b542658-304a-47d3-8082-d5708fe7b982"></a>

###### 2.1.2.1.2.26 Field **phone**

###### 2.1.2.1.2.26.1 **phone** Tree Diagram

![Hackolade image](Modulo-admin/image6.png?raw=true)

###### 2.1.2.1.2.26.2 **phone** Hierarchy

Parent field: **users**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#5d6c48e1-42f2-47a7-8778-b6ba1726d4bc class="margin-NaN">full_number</a></td><td class="no-break-word">string,numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e7a6ec49-4cdb-4d8d-a88a-be2f21cefc2b class="margin-NaN">indicative</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b60022f9-a9b4-41c2-83d1-bc006f88e079 class="margin-NaN">number_phone</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.1.2.26.3 **phone** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>phone</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="5d6c48e1-42f2-47a7-8778-b6ba1726d4bc"></a>

###### 2.1.2.1.2.27 Field **full\_number**

###### 2.1.2.1.2.27.1 **full\_number** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>full_number</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="e7a6ec49-4cdb-4d8d-a88a-be2f21cefc2b"></a>

###### 2.1.2.1.2.28 Field **indicative**

###### 2.1.2.1.2.28.1 **indicative** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>indicative</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>57</td></tr></tbody></table>

### <a id="b60022f9-a9b4-41c2-83d1-bc006f88e079"></a>

###### 2.1.2.1.2.29 Field **number\_phone**

###### 2.1.2.1.2.29.1 **number\_phone** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>number_phone</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>3170317850</td></tr></tbody></table>

### <a id="29375ad5-601f-47ea-946a-ca3e2a9bdf1f"></a>

###### 2.1.2.1.2.30 Field **rocketId**

###### 2.1.2.1.2.30.1 **rocketId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>rocketId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="9fc64250-079b-4a5e-b62a-a0eea7cc7dcb"></a>

###### 2.1.2.1.2.31 Field **user\_phone**

###### 2.1.2.1.2.31.1 **user\_phone** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>user_phone</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

###### 2.1.2.1.3 **users** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">client_id_-1</td><td class="table-column-property">user_-1</td><td class="table-column-property">dbname_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">client_id_-1</td><td class="table-column-indexes">user_-1</td><td class="table-column-indexes">dbname_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">client_id('descending')</td><td class="table-column-indexes">user('descending')</td><td class="table-column-indexes">dbname('descending')</td></tr></tbody></table>

### <a id="a2628771-9510-48ad-b4bb-3461c7ac2da1"></a>

##### 2.1.2.2 Collection **users\_sticker\_guide**

###### 2.1.2.2.1 **users\_sticker\_guide** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>users_sticker_guide</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#ac7a68bf-ef02-4449-964e-455eda30c57b><span class="name-container">rocketfy</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.2.2 **users\_sticker\_guide** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#8e792b63-de76-4b46-b8ab-5bd54bb6fe0e class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#51e20567-a0f4-4234-9832-f69555196f67 class="margin-0">db_name</a></td><td class="no-break-word">string</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#54660f51-0c11-4d3b-ab8c-3b947b7a7a3d class="margin-0">courriers</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f174241f-cfc1-4e94-b56c-670005fe5a60 class="margin-5">servientrega</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7b08a469-68ea-42c0-91cc-06c11a9e1d1a class="margin-5">interrapidisimo</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9cb0ecc8-0e39-4adc-b64a-db21a181e7f1 class="margin-5">envia</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#de02bded-7792-4ca1-bd64-3abca56ca66a class="margin-5">tcc</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="8e792b63-de76-4b46-b8ab-5bd54bb6fe0e"></a>

###### 2.1.2.2.2.1 Field **\_id**

###### 2.1.2.2.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="51e20567-a0f4-4234-9832-f69555196f67"></a>

###### 2.1.2.2.2.2 Field **db\_name**

###### 2.1.2.2.2.2.1 **db\_name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>db_name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#b3cf6f21-4a4d-4a9d-afec-691df5296b74>customers</a></td></tr><tr><td>Foreign field</td><td><a href=#075e0e77-aa2a-4a97-9b16-8527a6a301b5>dbname</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr><tr><td>Sample</td><td>shekinah_399607862</td></tr></tbody></table>

### <a id="54660f51-0c11-4d3b-ab8c-3b947b7a7a3d"></a>

###### 2.1.2.2.2.3 Field **courriers**

###### 2.1.2.2.2.3.1 **courriers** Tree Diagram

![Hackolade image](Modulo-admin/image7.png?raw=true)

###### 2.1.2.2.2.3.2 **courriers** Hierarchy

Parent field: **users\_sticker\_guide**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#f174241f-cfc1-4e94-b56c-670005fe5a60 class="margin-NaN">servientrega</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7b08a469-68ea-42c0-91cc-06c11a9e1d1a class="margin-NaN">interrapidisimo</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9cb0ecc8-0e39-4adc-b64a-db21a181e7f1 class="margin-NaN">envia</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#de02bded-7792-4ca1-bd64-3abca56ca66a class="margin-NaN">tcc</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.2.2.3.3 **courriers** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>courriers</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="f174241f-cfc1-4e94-b56c-670005fe5a60"></a>

###### 2.1.2.2.2.4 Field **servientrega**

###### 2.1.2.2.2.4.1 **servientrega** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>servientrega</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="7b08a469-68ea-42c0-91cc-06c11a9e1d1a"></a>

###### 2.1.2.2.2.5 Field **interrapidisimo**

###### 2.1.2.2.2.5.1 **interrapidisimo** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>interrapidisimo</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="9cb0ecc8-0e39-4adc-b64a-db21a181e7f1"></a>

###### 2.1.2.2.2.6 Field **envia**

###### 2.1.2.2.2.6.1 **envia** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>envia</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="de02bded-7792-4ca1-bd64-3abca56ca66a"></a>

###### 2.1.2.2.2.7 Field **tcc**

###### 2.1.2.2.2.7.1 **tcc** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>tcc</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

###### 2.1.2.2.3 **users\_sticker\_guide** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">db_name_1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">db_name_1</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">db_name('ascending')</td></tr></tbody></table>

### <a id="e35d3b15-e7a0-46d4-b3e6-523b15c328fd"></a>

##### 2.1.2.3 Collection **metrics\_use**

###### 2.1.2.3.1 **metrics\_use** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>metrics_use</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#ac7a68bf-ef02-4449-964e-455eda30c57b><span class="name-container">rocketfy</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.3.2 **metrics\_use** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#296938eb-178d-4f73-938a-e65089c14416 class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#44162bcb-a743-477f-b5b4-b75e56c00287 class="margin-0">type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f1b99fec-8189-4a9e-91c3-f388d9a8149f class="margin-0">subtype</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0de701c3-d53d-4d23-ac25-33f614aa0d78 class="margin-0">store_id</a></td><td class="no-break-word">string</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#828ee881-99b3-4542-855f-239a93079e42 class="margin-0">created_at</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5c3cf5aa-764b-4be2-8b08-037a4eca56f0 class="margin-0">count</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5b220661-8d7b-4df4-adf9-0fa9e6732178 class="margin-0">detail</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#14f51713-9f52-4ed7-8b95-0c8fe9c860f4 class="margin-5">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1becc817-415a-428b-b92a-82661cf9b115 class="margin-10">date</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9069630d-8b18-4fd4-8b4e-373f494047ff class="margin-10">metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b8a4e1b0-6f93-4b27-bc8f-3da59dc7e471 class="margin-15">order_id</a></td><td class="no-break-word">objectId</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c8bb7f2c-ac15-47e1-b043-f63877e8b0d7 class="margin-15">user</a></td><td class="no-break-word">null,document,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fda39b4d-31ee-412d-9801-c64ffebe28a0 class="margin-20">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f460aa96-d9c9-4b63-99c3-c85fa6017f90 class="margin-25">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f7ef4413-95dc-478a-be01-8bfb09c2125b class="margin-25">admin_mode</a></td><td class="no-break-word">null,boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fe2b589c-aa9d-4837-b06a-04e8db37ea92 class="margin-25">admin_user</a></td><td class="no-break-word">null,document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1dcced54-90e4-4c03-8a1b-498d53915912 class="margin-30">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d28bf265-a566-4dde-be34-43ab34769a74 class="margin-35">_id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5f51c76d-bb43-4977-91fa-c3d059e3dc54 class="margin-35">email</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3fe9575b-675f-406e-b089-cff27eb57cc8 class="margin-25">email</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a4e01109-f461-4a51-88bd-935798c39079 class="margin-15">agent</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#20edb517-9255-4c5c-a3ca-ecb0b2a0ebce class="margin-15">browser</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#560118ba-f9a5-47f1-b8a8-60366927a6d6 class="margin-15">clientIp</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b71767ab-2aea-4578-bf47-f47dd044f0b2 class="margin-15">forwardedFor</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4d5ab69b-d29d-4ca6-9299-cdf7a09058f8 class="margin-15">os</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#af66a5ea-a470-4ac9-9908-7ec83df82fd7 class="margin-15">query</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#48533695-1e7d-4c1e-9eef-0b35cbf1a99d class="margin-20">$and</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a7a5620b-e773-4ff6-bdc4-fe1e7114a125 class="margin-25">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0d9598e4-8834-4b94-86d8-dd49d940662d class="margin-30">created_time</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2caef203-61d1-4895-bdba-27879b602a04 class="margin-35">$gte</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bea5cc0e-c558-489e-bc3c-5ab06fda2ef4 class="margin-35">$lte</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="296938eb-178d-4f73-938a-e65089c14416"></a>

###### 2.1.2.3.2.1 Field **\_id**

###### 2.1.2.3.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="44162bcb-a743-477f-b5b4-b75e56c00287"></a>

###### 2.1.2.3.2.2 Field **type**

###### 2.1.2.3.2.2.1 **type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>orders</td></tr></tbody></table>

### <a id="f1b99fec-8189-4a9e-91c3-f388d9a8149f"></a>

###### 2.1.2.3.2.3 Field **subtype**

###### 2.1.2.3.2.3.1 **subtype** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>subtype</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>has_started_logistic_chat</td></tr></tbody></table>

### <a id="0de701c3-d53d-4d23-ac25-33f614aa0d78"></a>

###### 2.1.2.3.2.4 Field **store\_id**

###### 2.1.2.3.2.4.1 **store\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>store_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#b3cf6f21-4a4d-4a9d-afec-691df5296b74>customers</a></td></tr><tr><td>Foreign field</td><td><a href=#bd0c7b13-73ce-421c-9eea-7225ef09517d>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr><tr><td>Sample</td><td>nexoravitalcom_646707397</td></tr></tbody></table>

### <a id="828ee881-99b3-4542-855f-239a93079e42"></a>

###### 2.1.2.3.2.5 Field **created\_at**

###### 2.1.2.3.2.5.1 **created\_at** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_at</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5c3cf5aa-764b-4be2-8b08-037a4eca56f0"></a>

###### 2.1.2.3.2.6 Field **count**

###### 2.1.2.3.2.6.1 **count** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>count</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>273</td></tr></tbody></table>

### <a id="5b220661-8d7b-4df4-adf9-0fa9e6732178"></a>

###### 2.1.2.3.2.7 Field **detail**

###### 2.1.2.3.2.7.1 **detail** Tree Diagram

![Hackolade image](Modulo-admin/image8.png?raw=true)

###### 2.1.2.3.2.7.2 **detail** Hierarchy

Parent field: **metrics\_use**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#14f51713-9f52-4ed7-8b95-0c8fe9c860f4 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.3.2.7.3 **detail** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>detail</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="14f51713-9f52-4ed7-8b95-0c8fe9c860f4"></a>

###### 2.1.2.3.2.8 Field **\[0\]**

###### 2.1.2.3.2.8.1 **\[0\]** Tree Diagram

![Hackolade image](Modulo-admin/image9.png?raw=true)

###### 2.1.2.3.2.8.2 **\[0\]** Hierarchy

Parent field: **detail**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#1becc817-415a-428b-b92a-82661cf9b115 class="margin-NaN">date</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9069630d-8b18-4fd4-8b4e-373f494047ff class="margin-NaN">metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.3.2.8.3 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="1becc817-415a-428b-b92a-82661cf9b115"></a>

###### 2.1.2.3.2.9 Field **date**

###### 2.1.2.3.2.9.1 **date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="9069630d-8b18-4fd4-8b4e-373f494047ff"></a>

###### 2.1.2.3.2.10 Field **metadata**

###### 2.1.2.3.2.10.1 **metadata** Tree Diagram

![Hackolade image](Modulo-admin/image10.png?raw=true)

###### 2.1.2.3.2.10.2 **metadata** Hierarchy

Parent field: **\[0\]**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#b8a4e1b0-6f93-4b27-bc8f-3da59dc7e471 class="margin-NaN">order_id</a></td><td class="no-break-word">objectId</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c8bb7f2c-ac15-47e1-b043-f63877e8b0d7 class="margin-NaN">user</a></td><td class="no-break-word">null,document,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a4e01109-f461-4a51-88bd-935798c39079 class="margin-NaN">agent</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#20edb517-9255-4c5c-a3ca-ecb0b2a0ebce class="margin-NaN">browser</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#560118ba-f9a5-47f1-b8a8-60366927a6d6 class="margin-NaN">clientIp</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b71767ab-2aea-4578-bf47-f47dd044f0b2 class="margin-NaN">forwardedFor</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4d5ab69b-d29d-4ca6-9299-cdf7a09058f8 class="margin-NaN">os</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#af66a5ea-a470-4ac9-9908-7ec83df82fd7 class="margin-NaN">query</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.3.2.10.3 **metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="b8a4e1b0-6f93-4b27-bc8f-3da59dc7e471"></a>

###### 2.1.2.3.2.11 Field **order\_id**

###### 2.1.2.3.2.11.1 **order\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>order_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c8bb7f2c-ac15-47e1-b043-f63877e8b0d7"></a>

###### 2.1.2.3.2.12 Field **user**

###### 2.1.2.3.2.12.1 **user** Tree Diagram

![Hackolade image](Modulo-admin/image11.png?raw=true)

###### 2.1.2.3.2.12.2 **user** Hierarchy

Parent field: **metadata**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#fda39b4d-31ee-412d-9801-c64ffebe28a0 class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.3.2.12.3 **user** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>user</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,document,string)</td></tr><tr><td></td><td>[object Object],[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="fda39b4d-31ee-412d-9801-c64ffebe28a0"></a>

###### 2.1.2.3.2.13 Field **properties**

###### 2.1.2.3.2.13.1 **properties** Tree Diagram

![Hackolade image](Modulo-admin/image12.png?raw=true)

###### 2.1.2.3.2.13.2 **properties** Hierarchy

Parent field: **user**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#f460aa96-d9c9-4b63-99c3-c85fa6017f90 class="margin-NaN">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f7ef4413-95dc-478a-be01-8bfb09c2125b class="margin-NaN">admin_mode</a></td><td class="no-break-word">null,boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fe2b589c-aa9d-4837-b06a-04e8db37ea92 class="margin-NaN">admin_user</a></td><td class="no-break-word">null,document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3fe9575b-675f-406e-b089-cff27eb57cc8 class="margin-NaN">email</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.3.2.13.3 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="f460aa96-d9c9-4b63-99c3-c85fa6017f90"></a>

###### 2.1.2.3.2.14 Field **\_id**

###### 2.1.2.3.2.14.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="f7ef4413-95dc-478a-be01-8bfb09c2125b"></a>

###### 2.1.2.3.2.15 Field **admin\_mode**

###### 2.1.2.3.2.15.1 **admin\_mode** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>admin_mode</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,boolean)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="fe2b589c-aa9d-4837-b06a-04e8db37ea92"></a>

###### 2.1.2.3.2.16 Field **admin\_user**

###### 2.1.2.3.2.16.1 **admin\_user** Tree Diagram

![Hackolade image](Modulo-admin/image13.png?raw=true)

###### 2.1.2.3.2.16.2 **admin\_user** Hierarchy

Parent field: **properties**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#1dcced54-90e4-4c03-8a1b-498d53915912 class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.3.2.16.3 **admin\_user** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>admin_user</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,document)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="1dcced54-90e4-4c03-8a1b-498d53915912"></a>

###### 2.1.2.3.2.17 Field **properties**

###### 2.1.2.3.2.17.1 **properties** Tree Diagram

![Hackolade image](Modulo-admin/image14.png?raw=true)

###### 2.1.2.3.2.17.2 **properties** Hierarchy

Parent field: **admin\_user**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#d28bf265-a566-4dde-be34-43ab34769a74 class="margin-NaN">_id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5f51c76d-bb43-4977-91fa-c3d059e3dc54 class="margin-NaN">email</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.3.2.17.3 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="d28bf265-a566-4dde-be34-43ab34769a74"></a>

###### 2.1.2.3.2.18 Field **\_id**

###### 2.1.2.3.2.18.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5f51c76d-bb43-4977-91fa-c3d059e3dc54"></a>

###### 2.1.2.3.2.19 Field **email**

###### 2.1.2.3.2.19.1 **email** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>email</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="3fe9575b-675f-406e-b089-cff27eb57cc8"></a>

###### 2.1.2.3.2.20 Field **email**

###### 2.1.2.3.2.20.1 **email** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>email</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a4e01109-f461-4a51-88bd-935798c39079"></a>

###### 2.1.2.3.2.21 Field **agent**

###### 2.1.2.3.2.21.1 **agent** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>agent</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="20edb517-9255-4c5c-a3ca-ecb0b2a0ebce"></a>

###### 2.1.2.3.2.22 Field **browser**

###### 2.1.2.3.2.22.1 **browser** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>browser</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="560118ba-f9a5-47f1-b8a8-60366927a6d6"></a>

###### 2.1.2.3.2.23 Field **clientIp**

###### 2.1.2.3.2.23.1 **clientIp** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>clientIp</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="b71767ab-2aea-4578-bf47-f47dd044f0b2"></a>

###### 2.1.2.3.2.24 Field **forwardedFor**

###### 2.1.2.3.2.24.1 **forwardedFor** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>forwardedFor</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4d5ab69b-d29d-4ca6-9299-cdf7a09058f8"></a>

###### 2.1.2.3.2.25 Field **os**

###### 2.1.2.3.2.25.1 **os** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>os</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="af66a5ea-a470-4ac9-9908-7ec83df82fd7"></a>

###### 2.1.2.3.2.26 Field **query**

###### 2.1.2.3.2.26.1 **query** Tree Diagram

![Hackolade image](Modulo-admin/image15.png?raw=true)

###### 2.1.2.3.2.26.2 **query** Hierarchy

Parent field: **metadata**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#48533695-1e7d-4c1e-9eef-0b35cbf1a99d class="margin-NaN">$and</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.3.2.26.3 **query** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>query</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="48533695-1e7d-4c1e-9eef-0b35cbf1a99d"></a>

###### 2.1.2.3.2.27 Field **$and**

###### 2.1.2.3.2.27.1 **$and** Tree Diagram

![Hackolade image](Modulo-admin/image16.png?raw=true)

###### 2.1.2.3.2.27.2 **$and** Hierarchy

Parent field: **query**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#a7a5620b-e773-4ff6-bdc4-fe1e7114a125 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.3.2.27.3 **$and** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>$and</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="a7a5620b-e773-4ff6-bdc4-fe1e7114a125"></a>

###### 2.1.2.3.2.28 Field **\[0\]**

###### 2.1.2.3.2.28.1 **\[0\]** Tree Diagram

![Hackolade image](Modulo-admin/image17.png?raw=true)

###### 2.1.2.3.2.28.2 **\[0\]** Hierarchy

Parent field: **$and**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#0d9598e4-8834-4b94-86d8-dd49d940662d class="margin-NaN">created_time</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.3.2.28.3 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="0d9598e4-8834-4b94-86d8-dd49d940662d"></a>

###### 2.1.2.3.2.29 Field **created\_time**

###### 2.1.2.3.2.29.1 **created\_time** Tree Diagram

![Hackolade image](Modulo-admin/image18.png?raw=true)

###### 2.1.2.3.2.29.2 **created\_time** Hierarchy

Parent field: **\[0\]**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#2caef203-61d1-4895-bdba-27879b602a04 class="margin-NaN">$gte</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bea5cc0e-c558-489e-bc3c-5ab06fda2ef4 class="margin-NaN">$lte</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.3.2.29.3 **created\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="2caef203-61d1-4895-bdba-27879b602a04"></a>

###### 2.1.2.3.2.30 Field **$gte**

###### 2.1.2.3.2.30.1 **$gte** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>$gte</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="bea5cc0e-c558-489e-bc3c-5ab06fda2ef4"></a>

###### 2.1.2.3.2.31 Field **$lte**

###### 2.1.2.3.2.31.1 **$lte** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>$lte</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

###### 2.1.2.3.3 **metrics\_use** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">subtype_-1</td><td class="table-column-property">detail.metadata.user.admin_mode_-1</td><td class="table-column-property">store_id_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">subtype_-1</td><td class="table-column-indexes">detail.metadata.user.admin_mode_-1</td><td class="table-column-indexes">store_id_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">subtype('descending')</td><td class="table-column-indexes"></td><td class="table-column-indexes">store_id('descending')</td></tr></tbody></table>

### <a id="9dfd6d06-1625-47c9-806c-ff10078f8786"></a>

##### 2.1.2.4 Collection **mfa**

###### 2.1.2.4.1 **mfa** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>mfa</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#ac7a68bf-ef02-4449-964e-455eda30c57b><span class="name-container">rocketfy</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.4.2 **mfa** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#3f5c4247-856e-446c-a725-8f58a980142b class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#300a4894-51a0-4b3e-8659-e56e22713e26 class="margin-0">db_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a00dfcb5-a5c8-42b7-8dd0-a593ce5fe4db class="margin-0">otp_code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cbfc29dd-63d1-4206-8ea2-b1374e4eb2d4 class="margin-0">current_otp</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#db2049a6-3b79-443b-b94b-a9f1e2345e42 class="margin-0">created_date</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#524c3ce8-ad75-45d2-9f57-2d0788151942 class="margin-0">expired_date</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#600c5ac1-a91c-4666-b71e-e55d53825171 class="margin-0">attempts</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#51ccd951-a0e4-40ad-bfbd-4b54a1c55def class="margin-0">uuid_transaction_used</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#23a7eca1-9a27-4777-bf04-fc1d75569e15 class="margin-0">uuid</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5fbdc751-57d9-4a75-b62a-befef74caf5b class="margin-0">channel_notification</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4e066d2e-8463-42ec-a0d9-db7bb59314dd class="margin-5">type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3c6c3813-73ee-43f7-b004-bf8bf749d61d class="margin-5">email</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#09ae9346-568b-4e8f-a9ef-8c50cedae969 class="margin-5">sms</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7e6367e6-e318-49ce-aa8e-eb7e6caf64b1 class="margin-0">user_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5fbee9b6-21c9-4853-bc10-82d0d384865e class="margin-0">claim_date</a></td><td class="no-break-word">date</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f5802ce0-9007-463d-971b-1d73b56297b5 class="margin-0">claimed</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#64c3d6d3-a5d6-4659-9cac-13b91cee5304 class="margin-0">service_response_email</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0ad149d4-d333-49e0-aa6f-35e12d3cd38d class="margin-5">accepted</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#921f9f9c-8258-454e-b7ec-c89faadf8bb4 class="margin-10">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4b117a36-0bda-4766-8f15-8ac37f075797 class="margin-5">ehlo</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cf77d85c-e1bd-4ba4-acc5-0e0b323615c0 class="margin-10">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1b4ccf16-bfe3-4b07-8e32-cf1d1036c2f1 class="margin-5">envelope</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2f6dc0fb-399a-4a12-a485-4bfad5c32fad class="margin-10">from</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6f8f5aee-07e1-46eb-b86e-0184f669b0ea class="margin-10">to</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#499c7327-698a-4d70-9081-555acb302fd6 class="margin-15">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#91e21270-6cde-458b-bee7-85ecfb248dc2 class="margin-5">envelopeTime</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8a2bf9f3-4e3d-43f6-bc8e-7af1e2a10e47 class="margin-5">messageId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#46d29565-0b9d-4b3f-b06c-cf32df1d8395 class="margin-5">messageSize</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9854f1a6-1b40-4e96-b400-42be4bbc7da3 class="margin-5">messageTime</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#55bc20ac-0374-4f38-abbf-c9991bce7871 class="margin-5">rejected</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#015a4902-fd4f-47ee-ab27-2e69062f4398 class="margin-5">response</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3bdd2086-4ca7-44e9-8d4a-1098eb9f498e class="margin-0">service_response_sms</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b67e3710-4f64-4972-993d-1534f6192dfd class="margin-5">$metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c3378038-f104-441f-9489-cba1d6b2b929 class="margin-10">attempts</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b914cb3a-a018-4b3b-8b18-87b5265a982b class="margin-10">cfId</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#958f5e14-bdb6-4cd1-9dda-71570a007630 class="margin-10">extendedRequestId</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#299c08d0-da64-4b4d-a57f-29c53e80d530 class="margin-10">httpStatusCode</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ba6fb3c7-3df5-4e88-a10b-dcd249f6338b class="margin-10">requestId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#da58fd1b-921d-4d56-9a04-be8ad683491a class="margin-10">totalRetryDelay</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4f3a8ff0-212b-4c05-9995-cc9531d84ead class="margin-5">MessageId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="3f5c4247-856e-446c-a725-8f58a980142b"></a>

###### 2.1.2.4.2.1 Field **\_id**

###### 2.1.2.4.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="300a4894-51a0-4b3e-8659-e56e22713e26"></a>

###### 2.1.2.4.2.2 Field **db\_name**

###### 2.1.2.4.2.2.1 **db\_name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>db_name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>uniformesurban_1080540989</td></tr></tbody></table>

### <a id="a00dfcb5-a5c8-42b7-8dd0-a593ce5fe4db"></a>

###### 2.1.2.4.2.3 Field **otp\_code**

###### 2.1.2.4.2.3.1 **otp\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>otp_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>508136</td></tr></tbody></table>

### <a id="cbfc29dd-63d1-4206-8ea2-b1374e4eb2d4"></a>

###### 2.1.2.4.2.4 Field **current\_otp**

###### 2.1.2.4.2.4.1 **current\_otp** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>current_otp</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="db2049a6-3b79-443b-b94b-a9f1e2345e42"></a>

###### 2.1.2.4.2.5 Field **created\_date**

###### 2.1.2.4.2.5.1 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="524c3ce8-ad75-45d2-9f57-2d0788151942"></a>

###### 2.1.2.4.2.6 Field **expired\_date**

###### 2.1.2.4.2.6.1 **expired\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>expired_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="600c5ac1-a91c-4666-b71e-e55d53825171"></a>

###### 2.1.2.4.2.7 Field **attempts**

###### 2.1.2.4.2.7.1 **attempts** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>attempts</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>17</td></tr></tbody></table>

### <a id="51ccd951-a0e4-40ad-bfbd-4b54a1c55def"></a>

###### 2.1.2.4.2.8 Field **uuid\_transaction\_used**

###### 2.1.2.4.2.8.1 **uuid\_transaction\_used** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>uuid_transaction_used</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="23a7eca1-9a27-4777-bf04-fc1d75569e15"></a>

###### 2.1.2.4.2.9 Field **uuid**

###### 2.1.2.4.2.9.1 **uuid** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>uuid</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>e9052f73-da6e-4116-ae2b-480fd68a2a27</td></tr></tbody></table>

### <a id="5fbdc751-57d9-4a75-b62a-befef74caf5b"></a>

###### 2.1.2.4.2.10 Field **channel\_notification**

###### 2.1.2.4.2.10.1 **channel\_notification** Tree Diagram

![Hackolade image](Modulo-admin/image19.png?raw=true)

###### 2.1.2.4.2.10.2 **channel\_notification** Hierarchy

Parent field: **mfa**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#4e066d2e-8463-42ec-a0d9-db7bb59314dd class="margin-NaN">type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3c6c3813-73ee-43f7-b004-bf8bf749d61d class="margin-NaN">email</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#09ae9346-568b-4e8f-a9ef-8c50cedae969 class="margin-NaN">sms</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.10.3 **channel\_notification** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>channel_notification</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="4e066d2e-8463-42ec-a0d9-db7bb59314dd"></a>

###### 2.1.2.4.2.11 Field **type**

###### 2.1.2.4.2.11.1 **type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>email</td></tr></tbody></table>

### <a id="3c6c3813-73ee-43f7-b004-bf8bf749d61d"></a>

###### 2.1.2.4.2.12 Field **email**

###### 2.1.2.4.2.12.1 **email** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>email</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>uni.med.urban@gmail.com</td></tr></tbody></table>

### <a id="09ae9346-568b-4e8f-a9ef-8c50cedae969"></a>

###### 2.1.2.4.2.13 Field **sms**

###### 2.1.2.4.2.13.1 **sms** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>sms</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>573132771854</td></tr></tbody></table>

### <a id="7e6367e6-e318-49ce-aa8e-eb7e6caf64b1"></a>

###### 2.1.2.4.2.14 Field **user\_id**

###### 2.1.2.4.2.14.1 **user\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>user_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#635abd72-5aab-496e-a47e-31cf5060165e>users</a></td></tr><tr><td>Foreign field</td><td><a href=#7ded5fdf-322e-4b41-b104-4dda07c2c04c>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr></tbody></table>

### <a id="5fbee9b6-21c9-4853-bc10-82d0d384865e"></a>

###### 2.1.2.4.2.15 Field **claim\_date**

###### 2.1.2.4.2.15.1 **claim\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>claim_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="f5802ce0-9007-463d-971b-1d73b56297b5"></a>

###### 2.1.2.4.2.16 Field **claimed**

###### 2.1.2.4.2.16.1 **claimed** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>claimed</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="64c3d6d3-a5d6-4659-9cac-13b91cee5304"></a>

###### 2.1.2.4.2.17 Field **service\_response\_email**

###### 2.1.2.4.2.17.1 **service\_response\_email** Tree Diagram

![Hackolade image](Modulo-admin/image20.png?raw=true)

###### 2.1.2.4.2.17.2 **service\_response\_email** Hierarchy

Parent field: **mfa**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#0ad149d4-d333-49e0-aa6f-35e12d3cd38d class="margin-NaN">accepted</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4b117a36-0bda-4766-8f15-8ac37f075797 class="margin-NaN">ehlo</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1b4ccf16-bfe3-4b07-8e32-cf1d1036c2f1 class="margin-NaN">envelope</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#91e21270-6cde-458b-bee7-85ecfb248dc2 class="margin-NaN">envelopeTime</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8a2bf9f3-4e3d-43f6-bc8e-7af1e2a10e47 class="margin-NaN">messageId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#46d29565-0b9d-4b3f-b06c-cf32df1d8395 class="margin-NaN">messageSize</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9854f1a6-1b40-4e96-b400-42be4bbc7da3 class="margin-NaN">messageTime</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#55bc20ac-0374-4f38-abbf-c9991bce7871 class="margin-NaN">rejected</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#015a4902-fd4f-47ee-ab27-2e69062f4398 class="margin-NaN">response</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.17.3 **service\_response\_email** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>service_response_email</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="0ad149d4-d333-49e0-aa6f-35e12d3cd38d"></a>

###### 2.1.2.4.2.18 Field **accepted**

###### 2.1.2.4.2.18.1 **accepted** Tree Diagram

![Hackolade image](Modulo-admin/image21.png?raw=true)

###### 2.1.2.4.2.18.2 **accepted** Hierarchy

Parent field: **service\_response\_email**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#921f9f9c-8258-454e-b7ec-c89faadf8bb4 class="margin-NaN">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.18.3 **accepted** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>accepted</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="921f9f9c-8258-454e-b7ec-c89faadf8bb4"></a>

###### 2.1.2.4.2.19 Field **\[0\]**

###### 2.1.2.4.2.19.1 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Sample</td><td>luistalero1984@hotmail.com</td></tr></tbody></table>

### <a id="4b117a36-0bda-4766-8f15-8ac37f075797"></a>

###### 2.1.2.4.2.20 Field **ehlo**

###### 2.1.2.4.2.20.1 **ehlo** Tree Diagram

![Hackolade image](Modulo-admin/image22.png?raw=true)

###### 2.1.2.4.2.20.2 **ehlo** Hierarchy

Parent field: **service\_response\_email**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#cf77d85c-e1bd-4ba4-acc5-0e0b323615c0 class="margin-NaN">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.20.3 **ehlo** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>ehlo</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="cf77d85c-e1bd-4ba4-acc5-0e0b323615c0"></a>

###### 2.1.2.4.2.21 Field **\[0\]**

###### 2.1.2.4.2.21.1 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Sample</td><td>8BITMIME</td></tr></tbody></table>

### <a id="1b4ccf16-bfe3-4b07-8e32-cf1d1036c2f1"></a>

###### 2.1.2.4.2.22 Field **envelope**

###### 2.1.2.4.2.22.1 **envelope** Tree Diagram

![Hackolade image](Modulo-admin/image23.png?raw=true)

###### 2.1.2.4.2.22.2 **envelope** Hierarchy

Parent field: **service\_response\_email**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#2f6dc0fb-399a-4a12-a485-4bfad5c32fad class="margin-NaN">from</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6f8f5aee-07e1-46eb-b86e-0184f669b0ea class="margin-NaN">to</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.22.3 **envelope** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>envelope</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="2f6dc0fb-399a-4a12-a485-4bfad5c32fad"></a>

###### 2.1.2.4.2.23 Field **from**

###### 2.1.2.4.2.23.1 **from** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>from</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>no-reply@rocketfy.co</td></tr></tbody></table>

### <a id="6f8f5aee-07e1-46eb-b86e-0184f669b0ea"></a>

###### 2.1.2.4.2.24 Field **to**

###### 2.1.2.4.2.24.1 **to** Tree Diagram

![Hackolade image](Modulo-admin/image24.png?raw=true)

###### 2.1.2.4.2.24.2 **to** Hierarchy

Parent field: **envelope**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#499c7327-698a-4d70-9081-555acb302fd6 class="margin-NaN">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.24.3 **to** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>to</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="499c7327-698a-4d70-9081-555acb302fd6"></a>

###### 2.1.2.4.2.25 Field **\[0\]**

###### 2.1.2.4.2.25.1 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Sample</td><td>luistalero1984@hotmail.com</td></tr></tbody></table>

### <a id="91e21270-6cde-458b-bee7-85ecfb248dc2"></a>

###### 2.1.2.4.2.26 Field **envelopeTime**

###### 2.1.2.4.2.26.1 **envelopeTime** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>envelopeTime</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>101</td></tr></tbody></table>

### <a id="8a2bf9f3-4e3d-43f6-bc8e-7af1e2a10e47"></a>

###### 2.1.2.4.2.27 Field **messageId**

###### 2.1.2.4.2.27.1 **messageId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>messageId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>&lt;6234b8cf-0d55-1e9d-64e2-d7970e265dc2@rocketfy.co&gt;</td></tr></tbody></table>

### <a id="46d29565-0b9d-4b3f-b06c-cf32df1d8395"></a>

###### 2.1.2.4.2.28 Field **messageSize**

###### 2.1.2.4.2.28.1 **messageSize** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>messageSize</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>14368</td></tr></tbody></table>

### <a id="9854f1a6-1b40-4e96-b400-42be4bbc7da3"></a>

###### 2.1.2.4.2.29 Field **messageTime**

###### 2.1.2.4.2.29.1 **messageTime** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>messageTime</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1054</td></tr></tbody></table>

### <a id="55bc20ac-0374-4f38-abbf-c9991bce7871"></a>

###### 2.1.2.4.2.30 Field **rejected**

###### 2.1.2.4.2.30.1 **rejected** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>rejected</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="015a4902-fd4f-47ee-ab27-2e69062f4398"></a>

###### 2.1.2.4.2.31 Field **response**

###### 2.1.2.4.2.31.1 **response** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>response</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>250 Ok 01000193322dd0e9-5dbe8a5f-e0f1-42e8-92fc-3eb098389426-000000</td></tr></tbody></table>

### <a id="3bdd2086-4ca7-44e9-8d4a-1098eb9f498e"></a>

###### 2.1.2.4.2.32 Field **service\_response\_sms**

###### 2.1.2.4.2.32.1 **service\_response\_sms** Tree Diagram

![Hackolade image](Modulo-admin/image25.png?raw=true)

###### 2.1.2.4.2.32.2 **service\_response\_sms** Hierarchy

Parent field: **mfa**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#b67e3710-4f64-4972-993d-1534f6192dfd class="margin-NaN">$metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4f3a8ff0-212b-4c05-9995-cc9531d84ead class="margin-NaN">MessageId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.32.3 **service\_response\_sms** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>service_response_sms</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="b67e3710-4f64-4972-993d-1534f6192dfd"></a>

###### 2.1.2.4.2.33 Field **$metadata**

###### 2.1.2.4.2.33.1 **$metadata** Tree Diagram

![Hackolade image](Modulo-admin/image26.png?raw=true)

###### 2.1.2.4.2.33.2 **$metadata** Hierarchy

Parent field: **service\_response\_sms**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#c3378038-f104-441f-9489-cba1d6b2b929 class="margin-NaN">attempts</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b914cb3a-a018-4b3b-8b18-87b5265a982b class="margin-NaN">cfId</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#958f5e14-bdb6-4cd1-9dda-71570a007630 class="margin-NaN">extendedRequestId</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#299c08d0-da64-4b4d-a57f-29c53e80d530 class="margin-NaN">httpStatusCode</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ba6fb3c7-3df5-4e88-a10b-dcd249f6338b class="margin-NaN">requestId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#da58fd1b-921d-4d56-9a04-be8ad683491a class="margin-NaN">totalRetryDelay</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.4.2.33.3 **$metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>$metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="c3378038-f104-441f-9489-cba1d6b2b929"></a>

###### 2.1.2.4.2.34 Field **attempts**

###### 2.1.2.4.2.34.1 **attempts** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>attempts</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1</td></tr></tbody></table>

### <a id="b914cb3a-a018-4b3b-8b18-87b5265a982b"></a>

###### 2.1.2.4.2.35 Field **cfId**

###### 2.1.2.4.2.35.1 **cfId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cfId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="958f5e14-bdb6-4cd1-9dda-71570a007630"></a>

###### 2.1.2.4.2.36 Field **extendedRequestId**

###### 2.1.2.4.2.36.1 **extendedRequestId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>extendedRequestId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="299c08d0-da64-4b4d-a57f-29c53e80d530"></a>

###### 2.1.2.4.2.37 Field **httpStatusCode**

###### 2.1.2.4.2.37.1 **httpStatusCode** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>httpStatusCode</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>200</td></tr></tbody></table>

### <a id="ba6fb3c7-3df5-4e88-a10b-dcd249f6338b"></a>

###### 2.1.2.4.2.38 Field **requestId**

###### 2.1.2.4.2.38.1 **requestId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>requestId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>14c54ddc-eca7-529a-a5a1-2ddfd6b423bc</td></tr></tbody></table>

### <a id="da58fd1b-921d-4d56-9a04-be8ad683491a"></a>

###### 2.1.2.4.2.39 Field **totalRetryDelay**

###### 2.1.2.4.2.39.1 **totalRetryDelay** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>totalRetryDelay</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="4f3a8ff0-212b-4c05-9995-cc9531d84ead"></a>

###### 2.1.2.4.2.40 Field **MessageId**

###### 2.1.2.4.2.40.1 **MessageId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>MessageId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>e6b80935-c567-5f3e-a3ad-6936ff74ee18</td></tr></tbody></table>

###### 2.1.2.4.3 **mfa** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">uuid_-1</td><td class="table-column-property">user_id_-1_current_otp_-1_otp_code_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">uuid_-1</td><td class="table-column-indexes">user_id_-1_current_otp_-1_otp_code_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">uuid('descending')</td><td class="table-column-indexes">user_id('descending'), current_otp('descending'), otp_code('descending')</td></tr><tr><td>Unique</td><td class="table-column-indexes"></td><td class="table-column-indexes">true</td><td class="table-column-indexes"></td></tr></tbody></table>

### <a id="2620e329-587f-4ad6-936b-0cf39da379f0"></a>

##### 2.1.2.5 Collection **user\_sessions**

###### 2.1.2.5.1 **user\_sessions** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>user_sessions</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#ac7a68bf-ef02-4449-964e-455eda30c57b><span class="name-container">rocketfy</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.5.2 **user\_sessions** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#a5e4f573-d4e7-4ef6-a71b-77d374fbd3c7 class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#806bf5c1-c446-465f-b5af-39716670d810 class="margin-0">browser</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f6dc88fd-20dd-4ede-9a4e-5a4d3aaa6237 class="margin-0">dbname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8b8045e1-13bb-42ec-92c4-0b99d3afc064 class="margin-0">email</a></td><td class="no-break-word">string</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#241cd450-e276-489c-ad2e-c94aa07982f9 class="margin-0">created_at</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4060db7c-37e6-4f18-b540-770b90aeda78 class="margin-0">last_connection</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8d93eaed-47fe-494d-803b-dc383a2d69db class="margin-0">expire_at</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9026304c-b3ca-47d5-bb16-be7c31cb5d86 class="margin-0">identifier</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1f2a10ac-ec5d-45bf-819d-01d45e887379 class="margin-0">is_active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#be385cd0-5896-4593-9394-d09ff995512a class="margin-0">fingerprint</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ceb07ea3-1ff4-4e77-b49a-bdd660a08437 class="margin-0">ip</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#81d423cc-58f8-4657-9214-afd6cf9a7f19 class="margin-0">metaadmin_user</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c1ea5caf-310a-4462-aaca-5099d9a2a908 class="margin-5">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1432b1eb-578e-4de1-b871-d750c005f0eb class="margin-5">email</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5fc78f56-679b-4ec0-825b-b58ff5d7b107 class="margin-0">session_id</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5ef2bbe1-3453-4715-bf43-8d2c3abdb309 class="margin-0">using_super</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="a5e4f573-d4e7-4ef6-a71b-77d374fbd3c7"></a>

###### 2.1.2.5.2.1 Field **\_id**

###### 2.1.2.5.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="806bf5c1-c446-465f-b5af-39716670d810"></a>

###### 2.1.2.5.2.2 Field **browser**

###### 2.1.2.5.2.2.1 **browser** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>browser</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>"Chromium";v="130", "Google Chrome";v="130", "Not?A_Brand";v="99"</td></tr></tbody></table>

### <a id="f6dc88fd-20dd-4ede-9a4e-5a4d3aaa6237"></a>

###### 2.1.2.5.2.3 Field **dbname**

###### 2.1.2.5.2.3.1 **dbname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dbname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>belladamas_288071226</td></tr></tbody></table>

### <a id="8b8045e1-13bb-42ec-92c4-0b99d3afc064"></a>

###### 2.1.2.5.2.4 Field **email**

###### 2.1.2.5.2.4.1 **email** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>email</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#635abd72-5aab-496e-a47e-31cf5060165e>users</a></td></tr><tr><td>Foreign field</td><td><a href=#cd4547b7-f02b-4317-b8fc-23d68be8c71a>user</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr><tr><td>Sample</td><td>contacto.belladamas@gmail.com</td></tr></tbody></table>

### <a id="241cd450-e276-489c-ad2e-c94aa07982f9"></a>

###### 2.1.2.5.2.5 Field **created\_at**

###### 2.1.2.5.2.5.1 **created\_at** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_at</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4060db7c-37e6-4f18-b540-770b90aeda78"></a>

###### 2.1.2.5.2.6 Field **last\_connection**

###### 2.1.2.5.2.6.1 **last\_connection** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>last_connection</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8d93eaed-47fe-494d-803b-dc383a2d69db"></a>

###### 2.1.2.5.2.7 Field **expire\_at**

###### 2.1.2.5.2.7.1 **expire\_at** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>expire_at</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="9026304c-b3ca-47d5-bb16-be7c31cb5d86"></a>

###### 2.1.2.5.2.8 Field **identifier**

###### 2.1.2.5.2.8.1 **identifier** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>identifier</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>96be8f5b-1da2-4588-a135-e84ea7e10a98</td></tr></tbody></table>

### <a id="1f2a10ac-ec5d-45bf-819d-01d45e887379"></a>

###### 2.1.2.5.2.9 Field **is\_active**

###### 2.1.2.5.2.9.1 **is\_active** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>is_active</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="be385cd0-5896-4593-9394-d09ff995512a"></a>

###### 2.1.2.5.2.10 Field **fingerprint**

###### 2.1.2.5.2.10.1 **fingerprint** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fingerprint</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ceb07ea3-1ff4-4e77-b49a-bdd660a08437"></a>

###### 2.1.2.5.2.11 Field **ip**

###### 2.1.2.5.2.11.1 **ip** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>ip</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>181.59.3.152</td></tr></tbody></table>

### <a id="81d423cc-58f8-4657-9214-afd6cf9a7f19"></a>

###### 2.1.2.5.2.12 Field **metaadmin\_user**

###### 2.1.2.5.2.12.1 **metaadmin\_user** Tree Diagram

![Hackolade image](Modulo-admin/image27.png?raw=true)

###### 2.1.2.5.2.12.2 **metaadmin\_user** Hierarchy

Parent field: **user\_sessions**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#c1ea5caf-310a-4462-aaca-5099d9a2a908 class="margin-NaN">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1432b1eb-578e-4de1-b871-d750c005f0eb class="margin-NaN">email</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.5.2.12.3 **metaadmin\_user** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metaadmin_user</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="c1ea5caf-310a-4462-aaca-5099d9a2a908"></a>

###### 2.1.2.5.2.13 Field **\_id**

###### 2.1.2.5.2.13.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="1432b1eb-578e-4de1-b871-d750c005f0eb"></a>

###### 2.1.2.5.2.14 Field **email**

###### 2.1.2.5.2.14.1 **email** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>email</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>luis.ruiz@rocketfy.co</td></tr></tbody></table>

### <a id="5fc78f56-679b-4ec0-825b-b58ff5d7b107"></a>

###### 2.1.2.5.2.15 Field **session\_id**

###### 2.1.2.5.2.15.1 **session\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>session_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5ef2bbe1-3453-4715-bf43-8d2c3abdb309"></a>

###### 2.1.2.5.2.16 Field **using\_super**

###### 2.1.2.5.2.16.1 **using\_super** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>using_super</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

###### 2.1.2.5.3 **user\_sessions** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">identifier_-1</td><td class="table-column-property">identifier_1_is_active_1_expire_at_1</td><td class="table-column-property">identifier_1_expire_at_1</td><td class="table-column-property">using_super_-1_ip_-1_date_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">identifier_-1</td><td class="table-column-indexes">identifier_1_is_active_1_expire_at_1</td><td class="table-column-indexes">identifier_1_expire_at_1</td><td class="table-column-indexes">using_super_-1_ip_-1_date_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">identifier('descending')</td><td class="table-column-indexes">identifier('ascending'), is_active('ascending'), expire_at('ascending')</td><td class="table-column-indexes">identifier('ascending'), expire_at('ascending')</td><td class="table-column-indexes">using_super('descending'), ip('descending')</td></tr></tbody></table>

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">using_super_-1_session_id_-1_date_-1</td><td class="table-column-property">ip_-1</td><td class="table-column-property">dbname_-1</td><td class="table-column-property">email_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">using_super_-1_session_id_-1_date_-1</td><td class="table-column-indexes">ip_-1</td><td class="table-column-indexes">dbname_-1</td><td class="table-column-indexes">email_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">using_super('descending'), session_id('descending')</td><td class="table-column-indexes">ip('descending')</td><td class="table-column-indexes">dbname('descending')</td><td class="table-column-indexes">email('descending')</td></tr></tbody></table>

### <a id="b3cf6f21-4a4d-4a9d-afec-691df5296b74"></a>

##### 2.1.2.6 Collection **customers**

###### 2.1.2.6.1 **customers** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>customers</td></tr><tr><td>Technical name</td><td>Tiendas111</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Description</td><td><div class="docs-markdown"><p>En esta colección se almacenan todos los registros de las tiendas registradas en la plataforma. Cada tienda posee un campo único denominado dbname, el cual se encarga de vincular los datos de la tienda con el resto de los recursos relacionados (órdenes, productos, billetera, etc.) a través del campo establishment_identifier. De esta forma, se garantiza la consistencia y la trazabilidad de la información en todo el sistema.</p></div></td></tr><tr><td>Database</td><td><a href=#ac7a68bf-ef02-4449-964e-455eda30c57b><span class="name-container">rocketfy</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.6.2 **customers** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#bd0c7b13-73ce-421c-9eea-7225ef09517d class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk, dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0a0281b7-ce1c-4ba4-837e-f2fffb953b81 class="margin-0">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3dbc25d1-c48c-414d-9b2a-5561ead11571 class="margin-0">email</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#533c52dd-40ce-42c3-8fe6-4f30a4f36a6c class="margin-0">phone</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#578ccb91-e9a7-4d1b-8b75-d7e25f92141c class="margin-0">metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e8049db5-55f0-4440-961d-2d8bb381de9b class="margin-5">accept_time</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#24578803-ac99-4d66-9749-c4e30c46ed03 class="margin-5">hostname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dd4cdfcb-1c9f-4248-8d41-838fef28cd79 class="margin-5">platform</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a61ada41-02d1-4e81-9c37-785f8deba3eb class="margin-5">networkInterfaces</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dadd4c11-a8a9-4118-97bf-a7bed071f449 class="margin-10">Ethernet</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7a58c210-f326-4e33-9152-a47df2e24e2e class="margin-15">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#39eec03b-b479-470d-a743-b3188d66d6e4 class="margin-20">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a31e6c2c-5c59-47b0-bf8c-d33bf33b94df class="margin-20">netmask</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#eb0bf9aa-4341-4d0b-bca4-101a7a6872ea class="margin-20">family</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c42d3066-3911-4b38-88a2-19ebb1c24872 class="margin-20">mac</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9d13738d-1d3e-41d8-a2aa-9b46a6721163 class="margin-20">internal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a6461361-195f-41ab-8bcf-32aeab869f35 class="margin-20">cidr</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4e783b83-2b2b-4b35-b267-03c4bc586580 class="margin-20">scopeid</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d012b67c-76d0-4dee-88c6-110d66f81ed0 class="margin-10">Wi-Fi</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#66a78cc9-b87b-430b-8c3f-3aaad8a6bd3d class="margin-15">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#401fe6a2-8810-41ca-bb39-61b77aa2699a class="margin-20">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a2520eab-7c3f-4a1e-b6ae-ff47150d544b class="margin-20">netmask</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a1a43e78-0d07-4d18-9a48-f8e895f62b49 class="margin-20">family</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#89d39931-77dd-4f86-bdce-ee7675903819 class="margin-20">mac</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#40f84e21-6c7c-4874-ab4f-321890f4db27 class="margin-20">internal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8610f961-a930-4a84-8386-4c4f0d6ba8e7 class="margin-20">cidr</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#75d8ed04-5f12-4bb7-994c-d2a3726a3cd4 class="margin-20">scopeid</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#016d6e5d-edae-4551-bbd5-3f5331fd771c class="margin-10">Loopback&nbsp;Pseudo-Interface&nbsp;1</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f26f4d7d-9485-4011-91e7-e36cf3d0ced6 class="margin-15">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1dd4c85f-ab96-4c42-93f0-f203d4e65dcf class="margin-20">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5b4e4567-c03d-48d0-bacf-ea4b00b0beb7 class="margin-20">netmask</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f44e62ee-3391-40c6-91d3-ad09228c2575 class="margin-20">family</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3f0870aa-a7ae-49dc-8e17-334aeed8259c class="margin-20">mac</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#48edaca5-4277-4410-8f2d-e4616e216ee5 class="margin-20">internal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b8f70560-bdfe-42e6-9030-d1f1b82fbb83 class="margin-20">cidr</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#876c7290-665e-4efd-994a-7da94003d030 class="margin-20">scopeid</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e4de0482-6385-4263-86f8-dd63e43472b7 class="margin-5">from</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4f180122-33dc-48bf-a6b6-9f7ba03de397 class="margin-0">pageId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#075e0e77-aa2a-4a97-9b16-8527a6a301b5 class="margin-0">dbname</a></td><td class="no-break-word">string</td><td>true</td><td>dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fc0106a4-8aac-4949-81d7-7beac5a871ee class="margin-0">plan</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d3494168-962d-4053-95ef-be1b87bef5ad class="margin-0">country</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#60c4fc06-c1e5-4e13-a57d-d80860251e3c class="margin-0">test</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#669ab6f8-aa63-4a96-9968-8d0038758e27 class="margin-0">actived</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#806f4211-7177-4027-8e43-3bf6dfc177bf class="margin-0">exp</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#79a0fd2e-aba0-42d6-8e55-bd650740d54d class="margin-0">created_time</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7c99bb40-d870-49f2-8d20-991ddf8b525d class="margin-0">created_date</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#629f8752-3943-4a5b-922c-d39341a9b566 class="margin-5">dateFormat</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8d0e1411-a046-4fb7-a1e8-6b5cb6cd93cf class="margin-5">hourFormat</a></td><td class="no-break-word">time</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1534e79e-749d-40da-b570-26f99901350a class="margin-5">toDate</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1a030393-71ab-4f8e-9606-a30129798290 class="margin-0">host_asterisk</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4d93927a-7b63-4042-992c-5b612f2fc2ff class="margin-0">user_asterisk</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#62ee6211-5788-438c-889d-05d25b22082c class="margin-0">pass_asterisk</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#81375e3a-cc40-4b58-8b91-ddd7a7e8cf0f class="margin-0">visible</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d4740070-924c-4771-89b8-1dd56da3e0ff class="margin-0">slug</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#710dd299-485b-4404-9dc0-e87ae62277d3 class="margin-0">sender</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9db343c7-8d26-4913-a0f0-58c0493d0194 class="margin-5">date</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6b7e5c4e-86dc-4d66-9fed-4100520f4550 class="margin-5">shippings_count</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5f632bf7-602a-4f2a-94f5-c2d96b288649 class="margin-0">updated_date</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#50e63181-64a8-47cd-8539-426a50bc2c33 class="margin-5">created_sender</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#665c900d-9da1-4788-ad98-6d81fd3a12f5 class="margin-0">cohortMigrated3</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a7661303-b597-4cfd-ae33-40f14aedce4e class="margin-0">blocked_balance</a></td><td class="no-break-word">double</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3da5e79c-318b-4b33-8de3-87f61bab3b1e class="margin-0">rocketfy_leads</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9c3a10ad-1721-41b4-88a2-c14897bd0364 class="margin-0">rocketfy_shipping</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#97afedf2-957e-4e7a-86b6-a8acffdb5358 class="margin-0">cohortsMigration</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5c92feb8-86f1-4503-9fa2-a2248048ea03 class="margin-0">billing</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ff61076b-609c-4155-9087-1fc08091cc41 class="margin-5">document_type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d21ed2e2-391f-449d-9c92-52fb442a47dd class="margin-5">document</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ff4a17a7-40c4-4aa5-9440-e0773270c3e0 class="margin-5">document_evidence</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#233a9839-e626-4aca-801c-4b44d3b391b6 class="margin-10">fieldname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3e326ce7-8d08-40eb-ba28-2b7215201aa4 class="margin-10">originalname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fab3ec82-9955-4e22-a798-847bb56d1bc5 class="margin-10">encoding</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b4ed41e2-f443-43f4-ac1b-1354268cc5a3 class="margin-10">mimetype</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#794f7eb7-5c67-4895-9d00-96d53970ca9c class="margin-10">size</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a44db370-8a9c-4eb4-a560-4764bf3f9537 class="margin-10">bucket</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6b1637b5-0012-43ab-908c-d0c0ac8ccb28 class="margin-10">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#905de79b-f056-4745-b60d-326e5b9d8122 class="margin-10">acl</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#88f6c5f5-fd68-4f62-8f71-3afb543722d0 class="margin-10">contentType</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4146ca86-d2b9-4298-9f8a-c6134d25f3ad class="margin-10">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ba428a6c-c270-41e1-868a-d4890da71fd5 class="margin-10">storageClass</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ddfa4b8e-641c-446c-b822-c5f4e9882e21 class="margin-10">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#704eada4-b37d-42db-ad0c-cc880e9e0344 class="margin-10">metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cfb1495b-cd71-454b-a6b6-2427517f83f8 class="margin-15">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e5936b54-9f10-43d5-b33c-ed1c6684f423 class="margin-15">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#52c541c1-9df1-429a-b80f-89be465d3726 class="margin-10">location</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#30a235ec-a4de-4d94-9794-43fdb7df1bac class="margin-10">etag</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1fd5289c-1eae-4658-9a66-b6d22376b851 class="margin-10">versionId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f9977bbc-99e3-4e9c-ac3a-fde5c288aab1 class="margin-5">corporate_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4a21cfa0-9600-4fad-ba07-6bbeeda9506b class="margin-0">warehouse</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dca80109-1078-4a80-9d81-37d51026a72e class="margin-5">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#86ec2b78-af9d-48ba-aae1-bb02c5e1c0ae class="margin-5">status</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#65cd47f3-9177-4826-b555-73257d3163e5 class="margin-5">old_warehouses</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#45f55e4d-2c8b-4526-89e2-d763aadc95dd class="margin-5">products_counter</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7bb867ba-71f7-455d-bf0b-d930e9271e42 class="margin-5">has_shared_products</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b338b217-c391-49a0-bd18-635eb4a5290a class="margin-0">refferal_settings</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#143d676a-ad55-4079-a2ea-62a73bbf87f1 class="margin-5">goal</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f8e6c364-0cdd-4f54-b302-4054e7d2df03 class="margin-5">goal_type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8a1d8afa-af26-449c-adf4-d0dc0dcedd1b class="margin-5">reward</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#82507e81-f753-49f0-99a1-45119f9c52c9 class="margin-5">custom_commission</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#767edf2d-4d05-454b-b6bc-063d29811505 class="margin-10">rkf_charge_percent</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2230f7b0-4e1e-49e8-b3f4-02c6a51621df class="margin-10">constant_fee</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4641d717-f0f3-4391-9b07-9159f3376d50 class="margin-0">balance_advance</a></td><td class="no-break-word">double</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3fbfb2ca-f410-4e55-a039-462429990db7 class="margin-0">publicAPI</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#24441eac-2560-4ad0-ac99-64d7b14fb5e0 class="margin-5">domain</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#51696356-9b85-4ee7-ba82-d8d5c6076b7a class="margin-0">woocommerce</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4182142b-91e4-4981-bb09-558ea9005baf class="margin-5">app_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#25878061-abef-4b96-9b3c-19f2517d5872 class="margin-5">scope</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#68963e64-3bbf-4879-83aa-76d732afc1d3 class="margin-5">user_id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6a4b8c1b-09ac-4b44-8d8e-214a22298727 class="margin-5">return_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a8583ad4-3d41-46e2-931b-d9eed0cb880f class="margin-5">callback_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4694e091-bc38-4137-ba04-7d125be7d8fd class="margin-5">query_string</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#851fc900-9e73-494e-87e5-d4b98d418ff8 class="margin-5">domain</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#474e190a-b7e5-4959-b146-bb9f830c752a class="margin-5">auth_wc_api</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0233604c-b224-4245-a1a2-972b90760edc class="margin-0">custom_servientrega</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7a005ea7-a8b6-4c18-98e2-89ae62295dac class="margin-5">user</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#65b7deea-191f-4b1e-9e03-6023203adcdf class="margin-5">pwd</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ca3fd0eb-6e5b-4bb1-9ffe-0f4235e37741 class="margin-5">billing_code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#755c34e7-0842-490d-86e7-348cda5de769 class="margin-5">nom_cargue</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d988ec66-37ed-4db6-ad16-f8d056c1215b class="margin-5">id_product</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7eef7303-2483-4b51-b780-eb25a32b6a59 class="margin-5">init_weight</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#729099c8-b7d3-4994-9201-f227a04e5279 class="margin-0">required_billing_validation</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#51accfe9-f955-4641-975a-41a2dae0977d class="margin-0">questions</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d99c48d9-c926-4654-905d-bc6d1f2fd262 class="margin-5">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#51c64186-f2f0-4118-ba90-941aa33d0f81 class="margin-10">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b481090a-8912-43cf-bed8-8fdfcd197f9e class="margin-10">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8ff854ad-f063-4626-9818-c0172c6f5ea7 class="margin-10">answer</a></td><td class="no-break-word">array,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d7fd1e86-f706-46f6-b457-9409c5d28922 class="margin-15">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0e848cbf-21ac-4f3e-807c-b64bc5e275e1 class="margin-20">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dfd6c32b-dde9-4642-ad64-1cad14e68bde class="margin-0">migrate_quick_wd</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cd708260-06fc-49e5-8738-ac4ea82d6558 class="margin-0">migrated_contapyme</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#79852520-51c9-433f-a9c1-5c7d6969c386 class="margin-0">gifts</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#10199e0d-ef08-4b76-af58-8fdcd5e35526 class="margin-5">shippings</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3899cc15-95a1-4883-9cf1-dd75b8c603b6 class="margin-10">quantity</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9e482c10-19c3-4279-b98d-a8e7f8a5f1a2 class="margin-0">dropshipper</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a7cc1ebc-a063-4772-bbc7-b091b8b5e1f4 class="margin-5">date_created</a></td><td class="no-break-word">integer64</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bfdf7a0b-bc72-40ef-8332-6b12d5d4720f class="margin-5">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a19f8584-1a63-49d5-b1d2-75f3cf6887ee class="margin-0">last_connection_date</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e4821998-227d-40ae-8122-43f650499d9f class="margin-5">format</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#02ad87e9-007e-4d2e-ae63-dacedfcbf303 class="margin-5">unix</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6a2f4e8b-31e8-4c24-a4d5-cd5f08af13d0 class="margin-0">ban</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4b2c4e8b-418c-4e4b-8195-6d1e0f1488bf class="margin-5">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#58d9c996-7e5b-4f6c-a6b0-291f7227d004 class="margin-0">store_information</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ecd2e523-70a7-41bf-a3f2-9c43a7482e46 class="margin-5">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#882fe286-f1db-4213-8bc4-ecbbcd57f983 class="margin-5">logo</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0e420044-b26f-4f83-9c7b-bc60095f9657 class="margin-5">banner</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c07c9532-7398-43af-8fa0-99ae183b1814 class="margin-0">blocked</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#44e11908-94e0-45f2-8ec8-90a38d953d9b class="margin-0">enable_fast_withdraw</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ad8c1938-405f-4c46-8171-ea4602c585f8 class="margin-0">indicative</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#51603a27-2cd0-456c-a559-8390d671d939 class="margin-0">country_ref</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#278aebdc-1328-491a-992e-5cc535fe2351 class="margin-5">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0bfcc634-5cbc-4c3a-9433-35fcc9aea915 class="margin-5">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6eec492b-95f5-41b7-ac47-fd59340c1069 class="margin-5">iso2</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8f55c86b-d2b6-4787-9187-4157f4b1356b class="margin-5">iso3</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b125d10c-ce6a-4c3f-9b17-023785f2ad9d class="margin-5">flag_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#632b3e7a-b883-4a9b-8fe3-021ab1539d6e class="margin-5">phone_code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fe09c27d-fd89-43ef-b533-a618c9b78ff1 class="margin-0">currency_ref</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#393586e1-a4b0-4dad-99b3-1e3b1056c839 class="margin-5">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#53f6561f-2b59-46ce-be5e-9a43b98612df class="margin-5">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d4d1a2d7-1a7e-4787-9bdf-3661f435fe75 class="margin-5">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#37127af4-3d9f-49c4-a7d7-fef6e6804cf2 class="margin-5">htmlSymbol</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#27f19d90-3a00-48ba-9602-1e2aada4081f class="margin-0">scoringWarehouseReputation</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#76b6aacf-f733-4478-b64c-64826dfa542d class="margin-5">averageChatResponse</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0ed08e5a-a900-4adf-9421-5cefd89159c6 class="margin-5">averageChatResponseScore</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a3908030-8492-4730-88f3-508195e2306a class="margin-5">averageGuideTime</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2f4c6e0b-16c9-421f-8a12-c818b462b5ea class="margin-5">averageGuideTimeScore</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7685cf25-4ee4-4715-9acc-130b2db5a593 class="margin-5">cancellationRate</a></td><td class="no-break-word">double</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5c271aec-eea5-4b2a-b1ac-bc5d329409e1 class="margin-5">cancellationRateScore</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#feaf16a1-c4a1-4c8c-9ab9-3ddb77c973cd class="margin-5">final_score</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#11607121-01e2-450f-823a-c4cb8a0a3015 class="margin-0">subscription</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6f07ae76-f095-4c98-83fc-9b19125a2582 class="margin-5">plan</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0fc77799-7de0-4fe1-a99b-a1d7b8ca9ed2 class="margin-5">remainingShipments</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5fc88677-54ef-4754-bed0-6db89ec36b05 class="margin-5">expiresAt</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8401f164-3cf9-4b0a-bd46-bbe6f7ef4514 class="margin-5">isActive</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d7908ca5-f32e-48d0-b488-8a0117ac0f9b class="margin-5">paymentMethodId</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fc0c485a-9b45-4fe8-a77f-eabbcbafcd5a class="margin-0"></a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="bd0c7b13-73ce-421c-9eea-7225ef09517d"></a>

###### 2.1.2.6.2.1 Field **\_id**

###### 2.1.2.6.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="0a0281b7-ce1c-4ba4-837e-f2fffb953b81"></a>

###### 2.1.2.6.2.2 Field **name**

###### 2.1.2.6.2.2.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>test two drop</td></tr></tbody></table>

### <a id="3dbc25d1-c48c-414d-9b2a-5561ead11571"></a>

###### 2.1.2.6.2.3 Field **email**

###### 2.1.2.6.2.3.1 **email** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>email</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>testtwo@test.co</td></tr></tbody></table>

### <a id="533c52dd-40ce-42c3-8fe6-4f30a4f36a6c"></a>

###### 2.1.2.6.2.4 Field **phone**

###### 2.1.2.6.2.4.1 **phone** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>phone</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="578ccb91-e9a7-4d1b-8b75-d7e25f92141c"></a>

###### 2.1.2.6.2.5 Field **metadata**

###### 2.1.2.6.2.5.1 **metadata** Tree Diagram

![Hackolade image](Modulo-admin/image28.png?raw=true)

###### 2.1.2.6.2.5.2 **metadata** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#e8049db5-55f0-4440-961d-2d8bb381de9b class="margin-NaN">accept_time</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#24578803-ac99-4d66-9749-c4e30c46ed03 class="margin-NaN">hostname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dd4cdfcb-1c9f-4248-8d41-838fef28cd79 class="margin-NaN">platform</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a61ada41-02d1-4e81-9c37-785f8deba3eb class="margin-NaN">networkInterfaces</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e4de0482-6385-4263-86f8-dd63e43472b7 class="margin-NaN">from</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.5.3 **metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="e8049db5-55f0-4440-961d-2d8bb381de9b"></a>

###### 2.1.2.6.2.6 Field **accept\_time**

###### 2.1.2.6.2.6.1 **accept\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>accept_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1603230393</td></tr></tbody></table>

### <a id="24578803-ac99-4d66-9749-c4e30c46ed03"></a>

###### 2.1.2.6.2.7 Field **hostname**

###### 2.1.2.6.2.7.1 **hostname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>hostname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>DESKTOP-SSC8H1H</td></tr></tbody></table>

### <a id="dd4cdfcb-1c9f-4248-8d41-838fef28cd79"></a>

###### 2.1.2.6.2.8 Field **platform**

###### 2.1.2.6.2.8.1 **platform** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>platform</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>win32</td></tr></tbody></table>

### <a id="a61ada41-02d1-4e81-9c37-785f8deba3eb"></a>

###### 2.1.2.6.2.9 Field **networkInterfaces**

###### 2.1.2.6.2.9.1 **networkInterfaces** Tree Diagram

![Hackolade image](Modulo-admin/image29.png?raw=true)

###### 2.1.2.6.2.9.2 **networkInterfaces** Hierarchy

Parent field: **metadata**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#dadd4c11-a8a9-4118-97bf-a7bed071f449 class="margin-NaN">Ethernet</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d012b67c-76d0-4dee-88c6-110d66f81ed0 class="margin-NaN">Wi-Fi</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#016d6e5d-edae-4551-bbd5-3f5331fd771c class="margin-NaN">Loopback&nbsp;Pseudo-Interface&nbsp;1</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.9.3 **networkInterfaces** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>networkInterfaces</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="dadd4c11-a8a9-4118-97bf-a7bed071f449"></a>

###### 2.1.2.6.2.10 Field **Ethernet**

###### 2.1.2.6.2.10.1 **Ethernet** Tree Diagram

![Hackolade image](Modulo-admin/image30.png?raw=true)

###### 2.1.2.6.2.10.2 **Ethernet** Hierarchy

Parent field: **networkInterfaces**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#7a58c210-f326-4e33-9152-a47df2e24e2e class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.10.3 **Ethernet** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Ethernet</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="7a58c210-f326-4e33-9152-a47df2e24e2e"></a>

###### 2.1.2.6.2.11 Field **\[0\]**

###### 2.1.2.6.2.11.1 **\[0\]** Tree Diagram

![Hackolade image](Modulo-admin/image31.png?raw=true)

###### 2.1.2.6.2.11.2 **\[0\]** Hierarchy

Parent field: **Ethernet**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#39eec03b-b479-470d-a743-b3188d66d6e4 class="margin-NaN">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a31e6c2c-5c59-47b0-bf8c-d33bf33b94df class="margin-NaN">netmask</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#eb0bf9aa-4341-4d0b-bca4-101a7a6872ea class="margin-NaN">family</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c42d3066-3911-4b38-88a2-19ebb1c24872 class="margin-NaN">mac</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9d13738d-1d3e-41d8-a2aa-9b46a6721163 class="margin-NaN">internal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a6461361-195f-41ab-8bcf-32aeab869f35 class="margin-NaN">cidr</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4e783b83-2b2b-4b35-b267-03c4bc586580 class="margin-NaN">scopeid</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.11.3 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="39eec03b-b479-470d-a743-b3188d66d6e4"></a>

###### 2.1.2.6.2.12 Field **address**

###### 2.1.2.6.2.12.1 **address** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>address</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>172.27.233.245</td></tr></tbody></table>

### <a id="a31e6c2c-5c59-47b0-bf8c-d33bf33b94df"></a>

###### 2.1.2.6.2.13 Field **netmask**

###### 2.1.2.6.2.13.1 **netmask** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>netmask</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>255.255.248.0</td></tr></tbody></table>

### <a id="eb0bf9aa-4341-4d0b-bca4-101a7a6872ea"></a>

###### 2.1.2.6.2.14 Field **family**

###### 2.1.2.6.2.14.1 **family** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>family</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>IPv4</td></tr></tbody></table>

### <a id="c42d3066-3911-4b38-88a2-19ebb1c24872"></a>

###### 2.1.2.6.2.15 Field **mac**

###### 2.1.2.6.2.15.1 **mac** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mac</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>00:ff:dd:1f:32:99</td></tr></tbody></table>

### <a id="9d13738d-1d3e-41d8-a2aa-9b46a6721163"></a>

###### 2.1.2.6.2.16 Field **internal**

###### 2.1.2.6.2.16.1 **internal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>internal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="a6461361-195f-41ab-8bcf-32aeab869f35"></a>

###### 2.1.2.6.2.17 Field **cidr**

###### 2.1.2.6.2.17.1 **cidr** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cidr</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>172.27.233.245/21</td></tr></tbody></table>

### <a id="4e783b83-2b2b-4b35-b267-03c4bc586580"></a>

###### 2.1.2.6.2.18 Field **scopeid**

###### 2.1.2.6.2.18.1 **scopeid** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>scopeid</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>16</td></tr></tbody></table>

### <a id="d012b67c-76d0-4dee-88c6-110d66f81ed0"></a>

###### 2.1.2.6.2.19 Field **Wi-Fi**

###### 2.1.2.6.2.19.1 **Wi-Fi** Tree Diagram

![Hackolade image](Modulo-admin/image32.png?raw=true)

###### 2.1.2.6.2.19.2 **Wi-Fi** Hierarchy

Parent field: **networkInterfaces**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#66a78cc9-b87b-430b-8c3f-3aaad8a6bd3d class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.19.3 **Wi-Fi** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Wi-Fi</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="66a78cc9-b87b-430b-8c3f-3aaad8a6bd3d"></a>

###### 2.1.2.6.2.20 Field **\[0\]**

###### 2.1.2.6.2.20.1 **\[0\]** Tree Diagram

![Hackolade image](Modulo-admin/image33.png?raw=true)

###### 2.1.2.6.2.20.2 **\[0\]** Hierarchy

Parent field: **Wi-Fi**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#401fe6a2-8810-41ca-bb39-61b77aa2699a class="margin-NaN">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a2520eab-7c3f-4a1e-b6ae-ff47150d544b class="margin-NaN">netmask</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a1a43e78-0d07-4d18-9a48-f8e895f62b49 class="margin-NaN">family</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#89d39931-77dd-4f86-bdce-ee7675903819 class="margin-NaN">mac</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#40f84e21-6c7c-4874-ab4f-321890f4db27 class="margin-NaN">internal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8610f961-a930-4a84-8386-4c4f0d6ba8e7 class="margin-NaN">cidr</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#75d8ed04-5f12-4bb7-994c-d2a3726a3cd4 class="margin-NaN">scopeid</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.20.3 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="401fe6a2-8810-41ca-bb39-61b77aa2699a"></a>

###### 2.1.2.6.2.21 Field **address**

###### 2.1.2.6.2.21.1 **address** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>address</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>192.168.1.43</td></tr></tbody></table>

### <a id="a2520eab-7c3f-4a1e-b6ae-ff47150d544b"></a>

###### 2.1.2.6.2.22 Field **netmask**

###### 2.1.2.6.2.22.1 **netmask** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>netmask</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>255.255.255.0</td></tr></tbody></table>

### <a id="a1a43e78-0d07-4d18-9a48-f8e895f62b49"></a>

###### 2.1.2.6.2.23 Field **family**

###### 2.1.2.6.2.23.1 **family** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>family</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>IPv4</td></tr></tbody></table>

### <a id="89d39931-77dd-4f86-bdce-ee7675903819"></a>

###### 2.1.2.6.2.24 Field **mac**

###### 2.1.2.6.2.24.1 **mac** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mac</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>a0:51:0b:15:8f:ec</td></tr></tbody></table>

### <a id="40f84e21-6c7c-4874-ab4f-321890f4db27"></a>

###### 2.1.2.6.2.25 Field **internal**

###### 2.1.2.6.2.25.1 **internal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>internal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="8610f961-a930-4a84-8386-4c4f0d6ba8e7"></a>

###### 2.1.2.6.2.26 Field **cidr**

###### 2.1.2.6.2.26.1 **cidr** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cidr</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>192.168.1.43/24</td></tr></tbody></table>

### <a id="75d8ed04-5f12-4bb7-994c-d2a3726a3cd4"></a>

###### 2.1.2.6.2.27 Field **scopeid**

###### 2.1.2.6.2.27.1 **scopeid** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>scopeid</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>10</td></tr></tbody></table>

### <a id="016d6e5d-edae-4551-bbd5-3f5331fd771c"></a>

###### 2.1.2.6.2.28 Field **Loopback Pseudo-Interface 1**

###### 2.1.2.6.2.28.1 **Loopback Pseudo-Interface 1** Tree Diagram

![Hackolade image](Modulo-admin/image34.png?raw=true)

###### 2.1.2.6.2.28.2 **Loopback Pseudo-Interface 1** Hierarchy

Parent field: **networkInterfaces**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#f26f4d7d-9485-4011-91e7-e36cf3d0ced6 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.28.3 **Loopback Pseudo-Interface 1** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Loopback Pseudo-Interface 1</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="f26f4d7d-9485-4011-91e7-e36cf3d0ced6"></a>

###### 2.1.2.6.2.29 Field **\[0\]**

###### 2.1.2.6.2.29.1 **\[0\]** Tree Diagram

![Hackolade image](Modulo-admin/image35.png?raw=true)

###### 2.1.2.6.2.29.2 **\[0\]** Hierarchy

Parent field: **Loopback Pseudo-Interface 1**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#1dd4c85f-ab96-4c42-93f0-f203d4e65dcf class="margin-NaN">address</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5b4e4567-c03d-48d0-bacf-ea4b00b0beb7 class="margin-NaN">netmask</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f44e62ee-3391-40c6-91d3-ad09228c2575 class="margin-NaN">family</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3f0870aa-a7ae-49dc-8e17-334aeed8259c class="margin-NaN">mac</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#48edaca5-4277-4410-8f2d-e4616e216ee5 class="margin-NaN">internal</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b8f70560-bdfe-42e6-9030-d1f1b82fbb83 class="margin-NaN">cidr</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#876c7290-665e-4efd-994a-7da94003d030 class="margin-NaN">scopeid</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.29.3 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="1dd4c85f-ab96-4c42-93f0-f203d4e65dcf"></a>

###### 2.1.2.6.2.30 Field **address**

###### 2.1.2.6.2.30.1 **address** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>address</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>127.0.0.1</td></tr></tbody></table>

### <a id="5b4e4567-c03d-48d0-bacf-ea4b00b0beb7"></a>

###### 2.1.2.6.2.31 Field **netmask**

###### 2.1.2.6.2.31.1 **netmask** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>netmask</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>255.0.0.0</td></tr></tbody></table>

### <a id="f44e62ee-3391-40c6-91d3-ad09228c2575"></a>

###### 2.1.2.6.2.32 Field **family**

###### 2.1.2.6.2.32.1 **family** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>family</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>IPv4</td></tr></tbody></table>

### <a id="3f0870aa-a7ae-49dc-8e17-334aeed8259c"></a>

###### 2.1.2.6.2.33 Field **mac**

###### 2.1.2.6.2.33.1 **mac** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mac</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>00:00:00:00:00:00</td></tr></tbody></table>

### <a id="48edaca5-4277-4410-8f2d-e4616e216ee5"></a>

###### 2.1.2.6.2.34 Field **internal**

###### 2.1.2.6.2.34.1 **internal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>internal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="b8f70560-bdfe-42e6-9030-d1f1b82fbb83"></a>

###### 2.1.2.6.2.35 Field **cidr**

###### 2.1.2.6.2.35.1 **cidr** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cidr</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>127.0.0.1/8</td></tr></tbody></table>

### <a id="876c7290-665e-4efd-994a-7da94003d030"></a>

###### 2.1.2.6.2.36 Field **scopeid**

###### 2.1.2.6.2.36.1 **scopeid** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>scopeid</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="e4de0482-6385-4263-86f8-dd63e43472b7"></a>

###### 2.1.2.6.2.37 Field **from**

###### 2.1.2.6.2.37.1 **from** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>from</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>organico</td></tr></tbody></table>

### <a id="4f180122-33dc-48bf-a6b6-9f7ba03de397"></a>

###### 2.1.2.6.2.38 Field **pageId**

###### 2.1.2.6.2.38.1 **pageId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>pageId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>247456575848438</td></tr></tbody></table>

### <a id="075e0e77-aa2a-4a97-9b16-8527a6a301b5"></a>

###### 2.1.2.6.2.39 Field **dbname**

###### 2.1.2.6.2.39.1 **dbname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dbname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>testtwodrop_804079258</td></tr></tbody></table>

### <a id="fc0106a4-8aac-4949-81d7-7beac5a871ee"></a>

###### 2.1.2.6.2.40 Field **plan**

###### 2.1.2.6.2.40.1 **plan** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>plan</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>pro</td></tr></tbody></table>

### <a id="d3494168-962d-4053-95ef-be1b87bef5ad"></a>

###### 2.1.2.6.2.41 Field **country**

###### 2.1.2.6.2.41.1 **country** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>COL</td></tr></tbody></table>

### <a id="60c4fc06-c1e5-4e13-a57d-d80860251e3c"></a>

###### 2.1.2.6.2.42 Field **test**

###### 2.1.2.6.2.42.1 **test** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>test</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="669ab6f8-aa63-4a96-9968-8d0038758e27"></a>

###### 2.1.2.6.2.43 Field **actived**

###### 2.1.2.6.2.43.1 **actived** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>actived</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="806f4211-7177-4027-8e43-3bf6dfc177bf"></a>

###### 2.1.2.6.2.44 Field **exp**

###### 2.1.2.6.2.44.1 **exp** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>exp</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1604526393</td></tr></tbody></table>

### <a id="79a0fd2e-aba0-42d6-8e55-bd650740d54d"></a>

###### 2.1.2.6.2.45 Field **created\_time**

###### 2.1.2.6.2.45.1 **created\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1603230393</td></tr></tbody></table>

### <a id="7c99bb40-d870-49f2-8d20-991ddf8b525d"></a>

###### 2.1.2.6.2.46 Field **created\_date**

###### 2.1.2.6.2.46.1 **created\_date** Tree Diagram

![Hackolade image](Modulo-admin/image36.png?raw=true)

###### 2.1.2.6.2.46.2 **created\_date** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#629f8752-3943-4a5b-922c-d39341a9b566 class="margin-NaN">dateFormat</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8d0e1411-a046-4fb7-a1e8-6b5cb6cd93cf class="margin-NaN">hourFormat</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1534e79e-749d-40da-b570-26f99901350a class="margin-NaN">toDate</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.46.3 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="629f8752-3943-4a5b-922c-d39341a9b566"></a>

###### 2.1.2.6.2.47 Field **dateFormat**

###### 2.1.2.6.2.47.1 **dateFormat** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dateFormat</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>ISODate("2020-10-20")</td></tr></tbody></table>

### <a id="8d0e1411-a046-4fb7-a1e8-6b5cb6cd93cf"></a>

###### 2.1.2.6.2.48 Field **hourFormat**

###### 2.1.2.6.2.48.1 **hourFormat** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>hourFormat</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Format</td><td>time</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>16:46:33</td></tr></tbody></table>

### <a id="1534e79e-749d-40da-b570-26f99901350a"></a>

###### 2.1.2.6.2.49 Field **toDate**

###### 2.1.2.6.2.49.1 **toDate** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>toDate</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>ISODate("2020-10-20T16:46:33-05:00")</td></tr></tbody></table>

### <a id="1a030393-71ab-4f8e-9606-a30129798290"></a>

###### 2.1.2.6.2.50 Field **host\_asterisk**

###### 2.1.2.6.2.50.1 **host\_asterisk** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>host_asterisk</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4d93927a-7b63-4042-992c-5b612f2fc2ff"></a>

###### 2.1.2.6.2.51 Field **user\_asterisk**

###### 2.1.2.6.2.51.1 **user\_asterisk** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>user_asterisk</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="62ee6211-5788-438c-889d-05d25b22082c"></a>

###### 2.1.2.6.2.52 Field **pass\_asterisk**

###### 2.1.2.6.2.52.1 **pass\_asterisk** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>pass_asterisk</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="81375e3a-cc40-4b58-8b91-ddd7a7e8cf0f"></a>

###### 2.1.2.6.2.53 Field **visible**

###### 2.1.2.6.2.53.1 **visible** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>visible</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="d4740070-924c-4771-89b8-1dd56da3e0ff"></a>

###### 2.1.2.6.2.54 Field **slug**

###### 2.1.2.6.2.54.1 **slug** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>slug</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>testtwodrop2</td></tr></tbody></table>

### <a id="710dd299-485b-4404-9dc0-e87ae62277d3"></a>

###### 2.1.2.6.2.55 Field **sender**

###### 2.1.2.6.2.55.1 **sender** Tree Diagram

![Hackolade image](Modulo-admin/image37.png?raw=true)

###### 2.1.2.6.2.55.2 **sender** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#9db343c7-8d26-4913-a0f0-58c0493d0194 class="margin-NaN">date</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6b7e5c4e-86dc-4d66-9fed-4100520f4550 class="margin-NaN">shippings_count</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.55.3 **sender** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>sender</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="9db343c7-8d26-4913-a0f0-58c0493d0194"></a>

###### 2.1.2.6.2.56 Field **date**

###### 2.1.2.6.2.56.1 **date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1605713844</td></tr></tbody></table>

### <a id="6b7e5c4e-86dc-4d66-9fed-4100520f4550"></a>

###### 2.1.2.6.2.57 Field **shippings\_count**

###### 2.1.2.6.2.57.1 **shippings\_count** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shippings_count</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>370</td></tr></tbody></table>

### <a id="5f632bf7-602a-4f2a-94f5-c2d96b288649"></a>

###### 2.1.2.6.2.58 Field **updated\_date**

###### 2.1.2.6.2.58.1 **updated\_date** Tree Diagram

![Hackolade image](Modulo-admin/image38.png?raw=true)

###### 2.1.2.6.2.58.2 **updated\_date** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#50e63181-64a8-47cd-8539-426a50bc2c33 class="margin-NaN">created_sender</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.58.3 **updated\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>updated_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="50e63181-64a8-47cd-8539-426a50bc2c33"></a>

###### 2.1.2.6.2.59 Field **created\_sender**

###### 2.1.2.6.2.59.1 **created\_sender** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_sender</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1605713844</td></tr></tbody></table>

### <a id="665c900d-9da1-4788-ad98-6d81fd3a12f5"></a>

###### 2.1.2.6.2.60 Field **cohortMigrated3**

###### 2.1.2.6.2.60.1 **cohortMigrated3** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cohortMigrated3</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="a7661303-b597-4cfd-ae33-40f14aedce4e"></a>

###### 2.1.2.6.2.61 Field **blocked\_balance**

###### 2.1.2.6.2.61.1 **blocked\_balance** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>blocked_balance</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>4772129.24744489</td></tr></tbody></table>

### <a id="3da5e79c-318b-4b33-8de3-87f61bab3b1e"></a>

###### 2.1.2.6.2.62 Field **rocketfy\_leads**

###### 2.1.2.6.2.62.1 **rocketfy\_leads** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>rocketfy_leads</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="9c3a10ad-1721-41b4-88a2-c14897bd0364"></a>

###### 2.1.2.6.2.63 Field **rocketfy\_shipping**

###### 2.1.2.6.2.63.1 **rocketfy\_shipping** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>rocketfy_shipping</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="97afedf2-957e-4e7a-86b6-a8acffdb5358"></a>

###### 2.1.2.6.2.64 Field **cohortsMigration**

###### 2.1.2.6.2.64.1 **cohortsMigration** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cohortsMigration</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="5c92feb8-86f1-4503-9fa2-a2248048ea03"></a>

###### 2.1.2.6.2.65 Field **billing**

###### 2.1.2.6.2.65.1 **billing** Tree Diagram

![Hackolade image](Modulo-admin/image39.png?raw=true)

###### 2.1.2.6.2.65.2 **billing** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#ff61076b-609c-4155-9087-1fc08091cc41 class="margin-NaN">document_type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d21ed2e2-391f-449d-9c92-52fb442a47dd class="margin-NaN">document</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ff4a17a7-40c4-4aa5-9440-e0773270c3e0 class="margin-NaN">document_evidence</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f9977bbc-99e3-4e9c-ac3a-fde5c288aab1 class="margin-NaN">corporate_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.65.3 **billing** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>billing</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="ff61076b-609c-4155-9087-1fc08091cc41"></a>

###### 2.1.2.6.2.66 Field **document\_type**

###### 2.1.2.6.2.66.1 **document\_type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>document_type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>CC</td></tr></tbody></table>

### <a id="d21ed2e2-391f-449d-9c92-52fb442a47dd"></a>

###### 2.1.2.6.2.67 Field **document**

###### 2.1.2.6.2.67.1 **document** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>document</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1036676072</td></tr></tbody></table>

### <a id="ff4a17a7-40c4-4aa5-9440-e0773270c3e0"></a>

###### 2.1.2.6.2.68 Field **document\_evidence**

###### 2.1.2.6.2.68.1 **document\_evidence** Tree Diagram

![Hackolade image](Modulo-admin/image40.png?raw=true)

###### 2.1.2.6.2.68.2 **document\_evidence** Hierarchy

Parent field: **billing**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#233a9839-e626-4aca-801c-4b44d3b391b6 class="margin-NaN">fieldname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3e326ce7-8d08-40eb-ba28-2b7215201aa4 class="margin-NaN">originalname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fab3ec82-9955-4e22-a798-847bb56d1bc5 class="margin-NaN">encoding</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b4ed41e2-f443-43f4-ac1b-1354268cc5a3 class="margin-NaN">mimetype</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#794f7eb7-5c67-4895-9d00-96d53970ca9c class="margin-NaN">size</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a44db370-8a9c-4eb4-a560-4764bf3f9537 class="margin-NaN">bucket</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6b1637b5-0012-43ab-908c-d0c0ac8ccb28 class="margin-NaN">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#905de79b-f056-4745-b60d-326e5b9d8122 class="margin-NaN">acl</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#88f6c5f5-fd68-4f62-8f71-3afb543722d0 class="margin-NaN">contentType</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4146ca86-d2b9-4298-9f8a-c6134d25f3ad class="margin-NaN">contentDisposition</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ba428a6c-c270-41e1-868a-d4890da71fd5 class="margin-NaN">storageClass</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ddfa4b8e-641c-446c-b822-c5f4e9882e21 class="margin-NaN">serverSideEncryption</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#704eada4-b37d-42db-ad0c-cc880e9e0344 class="margin-NaN">metadata</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#52c541c1-9df1-429a-b80f-89be465d3726 class="margin-NaN">location</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#30a235ec-a4de-4d94-9794-43fdb7df1bac class="margin-NaN">etag</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1fd5289c-1eae-4658-9a66-b6d22376b851 class="margin-NaN">versionId</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.68.3 **document\_evidence** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>document_evidence</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="233a9839-e626-4aca-801c-4b44d3b391b6"></a>

###### 2.1.2.6.2.69 Field **fieldname**

###### 2.1.2.6.2.69.1 **fieldname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="3e326ce7-8d08-40eb-ba28-2b7215201aa4"></a>

###### 2.1.2.6.2.70 Field **originalname**

###### 2.1.2.6.2.70.1 **originalname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>originalname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>WhatsApp Image 2021-05-13 at 2.11.05 PM.jpeg</td></tr></tbody></table>

### <a id="fab3ec82-9955-4e22-a798-847bb56d1bc5"></a>

###### 2.1.2.6.2.71 Field **encoding**

###### 2.1.2.6.2.71.1 **encoding** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>encoding</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>7bit</td></tr></tbody></table>

### <a id="b4ed41e2-f443-43f4-ac1b-1354268cc5a3"></a>

###### 2.1.2.6.2.72 Field **mimetype**

###### 2.1.2.6.2.72.1 **mimetype** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>mimetype</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="794f7eb7-5c67-4895-9d00-96d53970ca9c"></a>

###### 2.1.2.6.2.73 Field **size**

###### 2.1.2.6.2.73.1 **size** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>size</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>54187</td></tr></tbody></table>

### <a id="a44db370-8a9c-4eb4-a560-4764bf3f9537"></a>

###### 2.1.2.6.2.74 Field **bucket**

###### 2.1.2.6.2.74.1 **bucket** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>bucket</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>shopping-rocketfy-uploads</td></tr></tbody></table>

### <a id="6b1637b5-0012-43ab-908c-d0c0ac8ccb28"></a>

###### 2.1.2.6.2.75 Field **key**

###### 2.1.2.6.2.75.1 **key** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>key</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>WhatsApp Image 2021-05-13 at 2.11.05 PM.jpeg</td></tr></tbody></table>

### <a id="905de79b-f056-4745-b60d-326e5b9d8122"></a>

###### 2.1.2.6.2.76 Field **acl**

###### 2.1.2.6.2.76.1 **acl** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>acl</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>public-read</td></tr></tbody></table>

### <a id="88f6c5f5-fd68-4f62-8f71-3afb543722d0"></a>

###### 2.1.2.6.2.77 Field **contentType**

###### 2.1.2.6.2.77.1 **contentType** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentType</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="4146ca86-d2b9-4298-9f8a-c6134d25f3ad"></a>

###### 2.1.2.6.2.78 Field **contentDisposition**

###### 2.1.2.6.2.78.1 **contentDisposition** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>contentDisposition</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ba428a6c-c270-41e1-868a-d4890da71fd5"></a>

###### 2.1.2.6.2.79 Field **storageClass**

###### 2.1.2.6.2.79.1 **storageClass** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>storageClass</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>STANDARD</td></tr></tbody></table>

### <a id="ddfa4b8e-641c-446c-b822-c5f4e9882e21"></a>

###### 2.1.2.6.2.80 Field **serverSideEncryption**

###### 2.1.2.6.2.80.1 **serverSideEncryption** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>serverSideEncryption</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="704eada4-b37d-42db-ad0c-cc880e9e0344"></a>

###### 2.1.2.6.2.81 Field **metadata**

###### 2.1.2.6.2.81.1 **metadata** Tree Diagram

![Hackolade image](Modulo-admin/image41.png?raw=true)

###### 2.1.2.6.2.81.2 **metadata** Hierarchy

Parent field: **document\_evidence**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#cfb1495b-cd71-454b-a6b6-2427517f83f8 class="margin-NaN">fieldName</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e5936b54-9f10-43d5-b33c-ed1c6684f423 class="margin-NaN">Content-Type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.81.3 **metadata** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>metadata</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="cfb1495b-cd71-454b-a6b6-2427517f83f8"></a>

###### 2.1.2.6.2.82 Field **fieldName**

###### 2.1.2.6.2.82.1 **fieldName** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fieldName</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="e5936b54-9f10-43d5-b33c-ed1c6684f423"></a>

###### 2.1.2.6.2.83 Field **Content-Type**

###### 2.1.2.6.2.83.1 **Content-Type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>Content-Type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image/jpeg</td></tr></tbody></table>

### <a id="52c541c1-9df1-429a-b80f-89be465d3726"></a>

###### 2.1.2.6.2.84 Field **location**

###### 2.1.2.6.2.84.1 **location** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>location</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://shopping-rocketfy-uploads.s3.amazonaws.com/WhatsApp%20Image%202021-05-13%20at%202.11.05%20PM.jpeg</td></tr></tbody></table>

### <a id="30a235ec-a4de-4d94-9794-43fdb7df1bac"></a>

###### 2.1.2.6.2.85 Field **etag**

###### 2.1.2.6.2.85.1 **etag** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>etag</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>"27ab062edb3d65c172f6f4f5517545a5"</td></tr></tbody></table>

### <a id="1fd5289c-1eae-4658-9a66-b6d22376b851"></a>

###### 2.1.2.6.2.86 Field **versionId**

###### 2.1.2.6.2.86.1 **versionId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>versionId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>ww6gGdpZn1oU1KnEFHxtyYzRJK7ITsPv</td></tr></tbody></table>

### <a id="f9977bbc-99e3-4e9c-ac3a-fde5c288aab1"></a>

###### 2.1.2.6.2.87 Field **corporate\_name**

###### 2.1.2.6.2.87.1 **corporate\_name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>corporate_name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>JUAN PABLO GUTIERREZ VARGAS</td></tr></tbody></table>

### <a id="4a21cfa0-9600-4fad-ba07-6bbeeda9506b"></a>

###### 2.1.2.6.2.88 Field **warehouse**

###### 2.1.2.6.2.88.1 **warehouse** Tree Diagram

![Hackolade image](Modulo-admin/image42.png?raw=true)

###### 2.1.2.6.2.88.2 **warehouse** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#dca80109-1078-4a80-9d81-37d51026a72e class="margin-NaN">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#86ec2b78-af9d-48ba-aae1-bb02c5e1c0ae class="margin-NaN">status</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#65cd47f3-9177-4826-b555-73257d3163e5 class="margin-NaN">old_warehouses</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#45f55e4d-2c8b-4526-89e2-d763aadc95dd class="margin-NaN">products_counter</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7bb867ba-71f7-455d-bf0b-d930e9271e42 class="margin-NaN">has_shared_products</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.88.3 **warehouse** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>warehouse</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="dca80109-1078-4a80-9d81-37d51026a72e"></a>

###### 2.1.2.6.2.89 Field **active**

###### 2.1.2.6.2.89.1 **active** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>active</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="86ec2b78-af9d-48ba-aae1-bb02c5e1c0ae"></a>

###### 2.1.2.6.2.90 Field **status**

###### 2.1.2.6.2.90.1 **status** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>status</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>rejected</td></tr></tbody></table>

### <a id="65cd47f3-9177-4826-b555-73257d3163e5"></a>

###### 2.1.2.6.2.91 Field **old\_warehouses**

###### 2.1.2.6.2.91.1 **old\_warehouses** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>old_warehouses</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="45f55e4d-2c8b-4526-89e2-d763aadc95dd"></a>

###### 2.1.2.6.2.92 Field **products\_counter**

###### 2.1.2.6.2.92.1 **products\_counter** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>products_counter</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="7bb867ba-71f7-455d-bf0b-d930e9271e42"></a>

###### 2.1.2.6.2.93 Field **has\_shared\_products**

###### 2.1.2.6.2.93.1 **has\_shared\_products** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>has_shared_products</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="b338b217-c391-49a0-bd18-635eb4a5290a"></a>

###### 2.1.2.6.2.94 Field **refferal\_settings**

###### 2.1.2.6.2.94.1 **refferal\_settings** Tree Diagram

![Hackolade image](Modulo-admin/image43.png?raw=true)

###### 2.1.2.6.2.94.2 **refferal\_settings** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#143d676a-ad55-4079-a2ea-62a73bbf87f1 class="margin-NaN">goal</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f8e6c364-0cdd-4f54-b302-4054e7d2df03 class="margin-NaN">goal_type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8a1d8afa-af26-449c-adf4-d0dc0dcedd1b class="margin-NaN">reward</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#82507e81-f753-49f0-99a1-45119f9c52c9 class="margin-NaN">custom_commission</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.94.3 **refferal\_settings** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>refferal_settings</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="143d676a-ad55-4079-a2ea-62a73bbf87f1"></a>

###### 2.1.2.6.2.95 Field **goal**

###### 2.1.2.6.2.95.1 **goal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>goal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>100</td></tr></tbody></table>

### <a id="f8e6c364-0cdd-4f54-b302-4054e7d2df03"></a>

###### 2.1.2.6.2.96 Field **goal\_type**

###### 2.1.2.6.2.96.1 **goal\_type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>goal_type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>orders</td></tr></tbody></table>

### <a id="8a1d8afa-af26-449c-adf4-d0dc0dcedd1b"></a>

###### 2.1.2.6.2.97 Field **reward**

###### 2.1.2.6.2.97.1 **reward** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>reward</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>500</td></tr></tbody></table>

### <a id="82507e81-f753-49f0-99a1-45119f9c52c9"></a>

###### 2.1.2.6.2.98 Field **custom\_commission**

###### 2.1.2.6.2.98.1 **custom\_commission** Tree Diagram

![Hackolade image](Modulo-admin/image44.png?raw=true)

###### 2.1.2.6.2.98.2 **custom\_commission** Hierarchy

Parent field: **refferal\_settings**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#767edf2d-4d05-454b-b6bc-063d29811505 class="margin-NaN">rkf_charge_percent</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2230f7b0-4e1e-49e8-b3f4-02c6a51621df class="margin-NaN">constant_fee</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.98.3 **custom\_commission** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>custom_commission</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="767edf2d-4d05-454b-b6bc-063d29811505"></a>

###### 2.1.2.6.2.99 Field **rkf\_charge\_percent**

###### 2.1.2.6.2.99.1 **rkf\_charge\_percent** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>rkf_charge_percent</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="2230f7b0-4e1e-49e8-b3f4-02c6a51621df"></a>

###### 2.1.2.6.2.100 Field **constant\_fee**

###### 2.1.2.6.2.100.1 **constant\_fee** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>constant_fee</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="4641d717-f0f3-4391-9b07-9159f3376d50"></a>

###### 2.1.2.6.2.101 Field **balance\_advance**

###### 2.1.2.6.2.101.1 **balance\_advance** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>balance_advance</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="3fbfb2ca-f410-4e55-a039-462429990db7"></a>

###### 2.1.2.6.2.102 Field **publicAPI**

###### 2.1.2.6.2.102.1 **publicAPI** Tree Diagram

![Hackolade image](Modulo-admin/image45.png?raw=true)

###### 2.1.2.6.2.102.2 **publicAPI** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#24441eac-2560-4ad0-ac99-64d7b14fb5e0 class="margin-NaN">domain</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.102.3 **publicAPI** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>publicAPI</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="24441eac-2560-4ad0-ac99-64d7b14fb5e0"></a>

###### 2.1.2.6.2.103 Field **domain**

###### 2.1.2.6.2.103.1 **domain** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>domain</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://test.co</td></tr></tbody></table>

### <a id="51696356-9b85-4ee7-ba82-d8d5c6076b7a"></a>

###### 2.1.2.6.2.104 Field **woocommerce**

###### 2.1.2.6.2.104.1 **woocommerce** Tree Diagram

![Hackolade image](Modulo-admin/image46.png?raw=true)

###### 2.1.2.6.2.104.2 **woocommerce** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#4182142b-91e4-4981-bb09-558ea9005baf class="margin-NaN">app_name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#25878061-abef-4b96-9b3c-19f2517d5872 class="margin-NaN">scope</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#68963e64-3bbf-4879-83aa-76d732afc1d3 class="margin-NaN">user_id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6a4b8c1b-09ac-4b44-8d8e-214a22298727 class="margin-NaN">return_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a8583ad4-3d41-46e2-931b-d9eed0cb880f class="margin-NaN">callback_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4694e091-bc38-4137-ba04-7d125be7d8fd class="margin-NaN">query_string</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#851fc900-9e73-494e-87e5-d4b98d418ff8 class="margin-NaN">domain</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#474e190a-b7e5-4959-b146-bb9f830c752a class="margin-NaN">auth_wc_api</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.104.3 **woocommerce** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>woocommerce</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="4182142b-91e4-4981-bb09-558ea9005baf"></a>

###### 2.1.2.6.2.105 Field **app\_name**

###### 2.1.2.6.2.105.1 **app\_name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>app_name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Rocketfy</td></tr></tbody></table>

### <a id="25878061-abef-4b96-9b3c-19f2517d5872"></a>

###### 2.1.2.6.2.106 Field **scope**

###### 2.1.2.6.2.106.1 **scope** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>scope</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>read_write</td></tr></tbody></table>

### <a id="68963e64-3bbf-4879-83aa-76d732afc1d3"></a>

###### 2.1.2.6.2.107 Field **user\_id**

###### 2.1.2.6.2.107.1 **user\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>user_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>5f8f5ab9d4240339c4281f5f</td></tr></tbody></table>

### <a id="6a4b8c1b-09ac-4b44-8d8e-214a22298727"></a>

###### 2.1.2.6.2.108 Field **return\_url**

###### 2.1.2.6.2.108.1 **return\_url** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>return_url</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://app.rocketfy.co/orders/pending</td></tr></tbody></table>

### <a id="a8583ad4-3d41-46e2-931b-d9eed0cb880f"></a>

###### 2.1.2.6.2.109 Field **callback\_url**

###### 2.1.2.6.2.109.1 **callback\_url** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>callback_url</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://rest.rocketfy.co/api/wc/hookauthwoocommerce</td></tr></tbody></table>

### <a id="4694e091-bc38-4137-ba04-7d125be7d8fd"></a>

###### 2.1.2.6.2.110 Field **query\_string**

###### 2.1.2.6.2.110.1 **query\_string** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>query_string</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://renechardon.com/wc-auth/v1/authorize?app_name=Rocketfy&amp;scope=read_write&amp;user_id=5f8f5ab9d4240339c4281f5f&amp;return_url=https%3A%2F%2Fapp.rocketfy.co%2Forders%2Fpending&amp;callback_url=https%3A%2F%2Frest.rocketfy.co%2Fapi%2Fwc%2Fhookauthwoocommerce</td></tr></tbody></table>

### <a id="851fc900-9e73-494e-87e5-d4b98d418ff8"></a>

###### 2.1.2.6.2.111 Field **domain**

###### 2.1.2.6.2.111.1 **domain** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>domain</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://renechardon.com</td></tr></tbody></table>

### <a id="474e190a-b7e5-4959-b146-bb9f830c752a"></a>

###### 2.1.2.6.2.112 Field **auth\_wc\_api**

###### 2.1.2.6.2.112.1 **auth\_wc\_api** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>auth_wc_api</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="0233604c-b224-4245-a1a2-972b90760edc"></a>

###### 2.1.2.6.2.113 Field **custom\_servientrega**

###### 2.1.2.6.2.113.1 **custom\_servientrega** Tree Diagram

![Hackolade image](Modulo-admin/image47.png?raw=true)

###### 2.1.2.6.2.113.2 **custom\_servientrega** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#7a005ea7-a8b6-4c18-98e2-89ae62295dac class="margin-NaN">user</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#65b7deea-191f-4b1e-9e03-6023203adcdf class="margin-NaN">pwd</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ca3fd0eb-6e5b-4bb1-9ffe-0f4235e37741 class="margin-NaN">billing_code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#755c34e7-0842-490d-86e7-348cda5de769 class="margin-NaN">nom_cargue</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d988ec66-37ed-4db6-ad16-f8d056c1215b class="margin-NaN">id_product</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7eef7303-2483-4b51-b780-eb25a32b6a59 class="margin-NaN">init_weight</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.113.3 **custom\_servientrega** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>custom_servientrega</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="7a005ea7-a8b6-4c18-98e2-89ae62295dac"></a>

###### 2.1.2.6.2.114 Field **user**

###### 2.1.2.6.2.114.1 **user** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>user</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>901195703</td></tr></tbody></table>

### <a id="65b7deea-191f-4b1e-9e03-6023203adcdf"></a>

###### 2.1.2.6.2.115 Field **pwd**

###### 2.1.2.6.2.115.1 **pwd** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>pwd</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>BpSUh12jBIipnUY/8yu2pQ==</td></tr></tbody></table>

### <a id="ca3fd0eb-6e5b-4bb1-9ffe-0f4235e37741"></a>

###### 2.1.2.6.2.116 Field **billing\_code**

###### 2.1.2.6.2.116.1 **billing\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>billing_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>SER123726</td></tr></tbody></table>

### <a id="755c34e7-0842-490d-86e7-348cda5de769"></a>

###### 2.1.2.6.2.117 Field **nom\_cargue**

###### 2.1.2.6.2.117.1 **nom\_cargue** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>nom_cargue</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Industrial</td></tr></tbody></table>

### <a id="d988ec66-37ed-4db6-ad16-f8d056c1215b"></a>

###### 2.1.2.6.2.118 Field **id\_product**

###### 2.1.2.6.2.118.1 **id\_product** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id_product</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6</td></tr></tbody></table>

### <a id="7eef7303-2483-4b51-b780-eb25a32b6a59"></a>

###### 2.1.2.6.2.119 Field **init\_weight**

###### 2.1.2.6.2.119.1 **init\_weight** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>init_weight</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>2000</td></tr></tbody></table>

### <a id="729099c8-b7d3-4994-9201-f227a04e5279"></a>

###### 2.1.2.6.2.120 Field **required\_billing\_validation**

###### 2.1.2.6.2.120.1 **required\_billing\_validation** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>required_billing_validation</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="51accfe9-f955-4641-975a-41a2dae0977d"></a>

###### 2.1.2.6.2.121 Field **questions**

###### 2.1.2.6.2.121.1 **questions** Tree Diagram

![Hackolade image](Modulo-admin/image48.png?raw=true)

###### 2.1.2.6.2.121.2 **questions** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#d99c48d9-c926-4654-905d-bc6d1f2fd262 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.121.3 **questions** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>questions</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="d99c48d9-c926-4654-905d-bc6d1f2fd262"></a>

###### 2.1.2.6.2.122 Field **\[0\]**

###### 2.1.2.6.2.122.1 **\[0\]** Tree Diagram

![Hackolade image](Modulo-admin/image49.png?raw=true)

###### 2.1.2.6.2.122.2 **\[0\]** Hierarchy

Parent field: **questions**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#51c64186-f2f0-4118-ba90-941aa33d0f81 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b481090a-8912-43cf-bed8-8fdfcd197f9e class="margin-NaN">key</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8ff854ad-f063-4626-9818-c0172c6f5ea7 class="margin-NaN">answer</a></td><td class="no-break-word">array,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.122.3 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="51c64186-f2f0-4118-ba90-941aa33d0f81"></a>

###### 2.1.2.6.2.123 Field **name**

###### 2.1.2.6.2.123.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>¿En qué necesita ayuda?</td></tr></tbody></table>

### <a id="b481090a-8912-43cf-bed8-8fdfcd197f9e"></a>

###### 2.1.2.6.2.124 Field **key**

###### 2.1.2.6.2.124.1 **key** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>key</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>need_help</td></tr></tbody></table>

### <a id="8ff854ad-f063-4626-9818-c0172c6f5ea7"></a>

###### 2.1.2.6.2.125 Field **answer**

###### 2.1.2.6.2.125.1 **answer** Tree Diagram

![Hackolade image](Modulo-admin/image50.png?raw=true)

###### 2.1.2.6.2.125.2 **answer** Hierarchy

Parent field: **\[0\]**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#d7fd1e86-f706-46f6-b457-9409c5d28922 class="margin-NaN">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.125.3 **answer** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>answer</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (array,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="d7fd1e86-f706-46f6-b457-9409c5d28922"></a>

###### 2.1.2.6.2.126 Field **items**

###### 2.1.2.6.2.126.1 **items** Tree Diagram

![Hackolade image](Modulo-admin/image51.png?raw=true)

###### 2.1.2.6.2.126.2 **items** Hierarchy

Parent field: **answer**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#0e848cbf-21ac-4f3e-807c-b64bc5e275e1 class="margin-NaN">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.126.3 **items** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="0e848cbf-21ac-4f3e-807c-b64bc5e275e1"></a>

###### 2.1.2.6.2.127 Field **\[0\]**

###### 2.1.2.6.2.127.1 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr></tbody></table>

### <a id="dfd6c32b-dde9-4642-ad64-1cad14e68bde"></a>

###### 2.1.2.6.2.128 Field **migrate\_quick\_wd**

###### 2.1.2.6.2.128.1 **migrate\_quick\_wd** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>migrate_quick_wd</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="cd708260-06fc-49e5-8738-ac4ea82d6558"></a>

###### 2.1.2.6.2.129 Field **migrated\_contapyme**

###### 2.1.2.6.2.129.1 **migrated\_contapyme** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>migrated_contapyme</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="79852520-51c9-433f-a9c1-5c7d6969c386"></a>

###### 2.1.2.6.2.130 Field **gifts**

###### 2.1.2.6.2.130.1 **gifts** Tree Diagram

![Hackolade image](Modulo-admin/image52.png?raw=true)

###### 2.1.2.6.2.130.2 **gifts** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#10199e0d-ef08-4b76-af58-8fdcd5e35526 class="margin-NaN">shippings</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.130.3 **gifts** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>gifts</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="10199e0d-ef08-4b76-af58-8fdcd5e35526"></a>

###### 2.1.2.6.2.131 Field **shippings**

###### 2.1.2.6.2.131.1 **shippings** Tree Diagram

![Hackolade image](Modulo-admin/image53.png?raw=true)

###### 2.1.2.6.2.131.2 **shippings** Hierarchy

Parent field: **gifts**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#3899cc15-95a1-4883-9cf1-dd75b8c603b6 class="margin-NaN">quantity</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.131.3 **shippings** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shippings</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="3899cc15-95a1-4883-9cf1-dd75b8c603b6"></a>

###### 2.1.2.6.2.132 Field **quantity**

###### 2.1.2.6.2.132.1 **quantity** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>quantity</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="9e482c10-19c3-4279-b98d-a8e7f8a5f1a2"></a>

###### 2.1.2.6.2.133 Field **dropshipper**

###### 2.1.2.6.2.133.1 **dropshipper** Tree Diagram

![Hackolade image](Modulo-admin/image54.png?raw=true)

###### 2.1.2.6.2.133.2 **dropshipper** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#a7cc1ebc-a063-4772-bbc7-b091b8b5e1f4 class="margin-NaN">date_created</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bfdf7a0b-bc72-40ef-8332-6b12d5d4720f class="margin-NaN">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.133.3 **dropshipper** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dropshipper</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="a7cc1ebc-a063-4772-bbc7-b091b8b5e1f4"></a>

###### 2.1.2.6.2.134 Field **date\_created**

###### 2.1.2.6.2.134.1 **date\_created** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>date_created</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer64</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1632411667000</td></tr></tbody></table>

### <a id="bfdf7a0b-bc72-40ef-8332-6b12d5d4720f"></a>

###### 2.1.2.6.2.135 Field **active**

###### 2.1.2.6.2.135.1 **active** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>active</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="a19f8584-1a63-49d5-b1d2-75f3cf6887ee"></a>

###### 2.1.2.6.2.136 Field **last\_connection\_date**

###### 2.1.2.6.2.136.1 **last\_connection\_date** Tree Diagram

![Hackolade image](Modulo-admin/image55.png?raw=true)

###### 2.1.2.6.2.136.2 **last\_connection\_date** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#e4821998-227d-40ae-8122-43f650499d9f class="margin-NaN">format</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#02ad87e9-007e-4d2e-ae63-dacedfcbf303 class="margin-NaN">unix</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.136.3 **last\_connection\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>last_connection_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="e4821998-227d-40ae-8122-43f650499d9f"></a>

###### 2.1.2.6.2.137 Field **format**

###### 2.1.2.6.2.137.1 **format** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>format</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>31/03/2025 20:43</td></tr></tbody></table>

### <a id="02ad87e9-007e-4d2e-ae63-dacedfcbf303"></a>

###### 2.1.2.6.2.138 Field **unix**

###### 2.1.2.6.2.138.1 **unix** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>unix</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1743453783</td></tr></tbody></table>

### <a id="6a2f4e8b-31e8-4c24-a4d5-cd5f08af13d0"></a>

###### 2.1.2.6.2.139 Field **ban**

###### 2.1.2.6.2.139.1 **ban** Tree Diagram

![Hackolade image](Modulo-admin/image56.png?raw=true)

###### 2.1.2.6.2.139.2 **ban** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#4b2c4e8b-418c-4e4b-8195-6d1e0f1488bf class="margin-NaN">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.139.3 **ban** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>ban</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="4b2c4e8b-418c-4e4b-8195-6d1e0f1488bf"></a>

###### 2.1.2.6.2.140 Field **\[0\]**

###### 2.1.2.6.2.140.1 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Sample</td><td>shippings</td></tr></tbody></table>

### <a id="58d9c996-7e5b-4f6c-a6b0-291f7227d004"></a>

###### 2.1.2.6.2.141 Field **store\_information**

###### 2.1.2.6.2.141.1 **store\_information** Tree Diagram

![Hackolade image](Modulo-admin/image57.png?raw=true)

###### 2.1.2.6.2.141.2 **store\_information** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#ecd2e523-70a7-41bf-a3f2-9c43a7482e46 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#882fe286-f1db-4213-8bc4-ecbbcd57f983 class="margin-NaN">logo</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0e420044-b26f-4f83-9c7b-bc60095f9657 class="margin-NaN">banner</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.141.3 **store\_information** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>store_information</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="ecd2e523-70a7-41bf-a3f2-9c43a7482e46"></a>

###### 2.1.2.6.2.142 Field **name**

###### 2.1.2.6.2.142.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>test two drop 2</td></tr></tbody></table>

### <a id="882fe286-f1db-4213-8bc4-ecbbcd57f983"></a>

###### 2.1.2.6.2.143 Field **logo**

###### 2.1.2.6.2.143.1 **logo** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>logo</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://shopping-rocketfy-uploads.s3.amazonaws.com/testtwodrop_804079258_121642999_10221463163479893_6069666320517077970_n44.jpg</td></tr></tbody></table>

### <a id="0e420044-b26f-4f83-9c7b-bc60095f9657"></a>

###### 2.1.2.6.2.144 Field **banner**

###### 2.1.2.6.2.144.1 **banner** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>banner</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://shopping-rocketfy-uploads.s3.amazonaws.com/testtwodrop_804079258_image%20%281%29.png</td></tr></tbody></table>

### <a id="c07c9532-7398-43af-8fa0-99ae183b1814"></a>

###### 2.1.2.6.2.145 Field **blocked**

###### 2.1.2.6.2.145.1 **blocked** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>blocked</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="44e11908-94e0-45f2-8ec8-90a38d953d9b"></a>

###### 2.1.2.6.2.146 Field **enable\_fast\_withdraw**

###### 2.1.2.6.2.146.1 **enable\_fast\_withdraw** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>enable_fast_withdraw</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="ad8c1938-405f-4c46-8171-ea4602c585f8"></a>

###### 2.1.2.6.2.147 Field **indicative**

###### 2.1.2.6.2.147.1 **indicative** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>indicative</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>57</td></tr></tbody></table>

### <a id="51603a27-2cd0-456c-a559-8390d671d939"></a>

###### 2.1.2.6.2.148 Field **country\_ref**

###### 2.1.2.6.2.148.1 **country\_ref** Tree Diagram

![Hackolade image](Modulo-admin/image58.png?raw=true)

###### 2.1.2.6.2.148.2 **country\_ref** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#278aebdc-1328-491a-992e-5cc535fe2351 class="margin-NaN">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0bfcc634-5cbc-4c3a-9433-35fcc9aea915 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6eec492b-95f5-41b7-ac47-fd59340c1069 class="margin-NaN">iso2</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8f55c86b-d2b6-4787-9187-4157f4b1356b class="margin-NaN">iso3</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b125d10c-ce6a-4c3f-9b17-023785f2ad9d class="margin-NaN">flag_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#632b3e7a-b883-4a9b-8fe3-021ab1539d6e class="margin-NaN">phone_code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.148.3 **country\_ref** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country_ref</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="278aebdc-1328-491a-992e-5cc535fe2351"></a>

###### 2.1.2.6.2.149 Field **\_id**

###### 2.1.2.6.2.149.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="0bfcc634-5cbc-4c3a-9433-35fcc9aea915"></a>

###### 2.1.2.6.2.150 Field **name**

###### 2.1.2.6.2.150.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Colombia</td></tr></tbody></table>

### <a id="6eec492b-95f5-41b7-ac47-fd59340c1069"></a>

###### 2.1.2.6.2.151 Field **iso2**

###### 2.1.2.6.2.151.1 **iso2** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>iso2</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>CO</td></tr></tbody></table>

### <a id="8f55c86b-d2b6-4787-9187-4157f4b1356b"></a>

###### 2.1.2.6.2.152 Field **iso3**

###### 2.1.2.6.2.152.1 **iso3** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>iso3</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>COL</td></tr></tbody></table>

### <a id="b125d10c-ce6a-4c3f-9b17-023785f2ad9d"></a>

###### 2.1.2.6.2.153 Field **flag\_url**

###### 2.1.2.6.2.153.1 **flag\_url** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>flag_url</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://www.geonames.org/flags/x/co.gif</td></tr></tbody></table>

### <a id="632b3e7a-b883-4a9b-8fe3-021ab1539d6e"></a>

###### 2.1.2.6.2.154 Field **phone\_code**

###### 2.1.2.6.2.154.1 **phone\_code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>phone_code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>57</td></tr></tbody></table>

### <a id="fe09c27d-fd89-43ef-b533-a618c9b78ff1"></a>

###### 2.1.2.6.2.155 Field **currency\_ref**

###### 2.1.2.6.2.155.1 **currency\_ref** Tree Diagram

![Hackolade image](Modulo-admin/image59.png?raw=true)

###### 2.1.2.6.2.155.2 **currency\_ref** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#393586e1-a4b0-4dad-99b3-1e3b1056c839 class="margin-NaN">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#53f6561f-2b59-46ce-be5e-9a43b98612df class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d4d1a2d7-1a7e-4787-9bdf-3661f435fe75 class="margin-NaN">code</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#37127af4-3d9f-49c4-a7d7-fef6e6804cf2 class="margin-NaN">htmlSymbol</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.155.3 **currency\_ref** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>currency_ref</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="393586e1-a4b0-4dad-99b3-1e3b1056c839"></a>

###### 2.1.2.6.2.156 Field **\_id**

###### 2.1.2.6.2.156.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="53f6561f-2b59-46ce-be5e-9a43b98612df"></a>

###### 2.1.2.6.2.157 Field **name**

###### 2.1.2.6.2.157.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Peso Colombiano</td></tr></tbody></table>

### <a id="d4d1a2d7-1a7e-4787-9bdf-3661f435fe75"></a>

###### 2.1.2.6.2.158 Field **code**

###### 2.1.2.6.2.158.1 **code** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>code</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>COP</td></tr></tbody></table>

### <a id="37127af4-3d9f-49c4-a7d7-fef6e6804cf2"></a>

###### 2.1.2.6.2.159 Field **htmlSymbol**

###### 2.1.2.6.2.159.1 **htmlSymbol** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>htmlSymbol</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>&amp;#36;</td></tr></tbody></table>

### <a id="27f19d90-3a00-48ba-9602-1e2aada4081f"></a>

###### 2.1.2.6.2.160 Field **scoringWarehouseReputation**

###### 2.1.2.6.2.160.1 **scoringWarehouseReputation** Tree Diagram

![Hackolade image](Modulo-admin/image60.png?raw=true)

###### 2.1.2.6.2.160.2 **scoringWarehouseReputation** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#76b6aacf-f733-4478-b64c-64826dfa542d class="margin-NaN">averageChatResponse</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0ed08e5a-a900-4adf-9421-5cefd89159c6 class="margin-NaN">averageChatResponseScore</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a3908030-8492-4730-88f3-508195e2306a class="margin-NaN">averageGuideTime</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2f4c6e0b-16c9-421f-8a12-c818b462b5ea class="margin-NaN">averageGuideTimeScore</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7685cf25-4ee4-4715-9acc-130b2db5a593 class="margin-NaN">cancellationRate</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5c271aec-eea5-4b2a-b1ac-bc5d329409e1 class="margin-NaN">cancellationRateScore</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#feaf16a1-c4a1-4c8c-9ab9-3ddb77c973cd class="margin-NaN">final_score</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.160.3 **scoringWarehouseReputation** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>scoringWarehouseReputation</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="76b6aacf-f733-4478-b64c-64826dfa542d"></a>

###### 2.1.2.6.2.161 Field **averageChatResponse**

###### 2.1.2.6.2.161.1 **averageChatResponse** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>averageChatResponse</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="0ed08e5a-a900-4adf-9421-5cefd89159c6"></a>

###### 2.1.2.6.2.162 Field **averageChatResponseScore**

###### 2.1.2.6.2.162.1 **averageChatResponseScore** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>averageChatResponseScore</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="a3908030-8492-4730-88f3-508195e2306a"></a>

###### 2.1.2.6.2.163 Field **averageGuideTime**

###### 2.1.2.6.2.163.1 **averageGuideTime** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>averageGuideTime</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="2f4c6e0b-16c9-421f-8a12-c818b462b5ea"></a>

###### 2.1.2.6.2.164 Field **averageGuideTimeScore**

###### 2.1.2.6.2.164.1 **averageGuideTimeScore** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>averageGuideTimeScore</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="7685cf25-4ee4-4715-9acc-130b2db5a593"></a>

###### 2.1.2.6.2.165 Field **cancellationRate**

###### 2.1.2.6.2.165.1 **cancellationRate** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cancellationRate</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>11.11</td></tr></tbody></table>

### <a id="5c271aec-eea5-4b2a-b1ac-bc5d329409e1"></a>

###### 2.1.2.6.2.166 Field **cancellationRateScore**

###### 2.1.2.6.2.166.1 **cancellationRateScore** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>cancellationRateScore</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>3</td></tr></tbody></table>

### <a id="feaf16a1-c4a1-4c8c-9ab9-3ddb77c973cd"></a>

###### 2.1.2.6.2.167 Field **final\_score**

###### 2.1.2.6.2.167.1 **final\_score** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>final_score</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1</td></tr></tbody></table>

### <a id="11607121-01e2-450f-823a-c4cb8a0a3015"></a>

###### 2.1.2.6.2.168 Field **subscription**

###### 2.1.2.6.2.168.1 **subscription** Tree Diagram

![Hackolade image](Modulo-admin/image61.png?raw=true)

###### 2.1.2.6.2.168.2 **subscription** Hierarchy

Parent field: **customers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#6f07ae76-f095-4c98-83fc-9b19125a2582 class="margin-NaN">plan</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0fc77799-7de0-4fe1-a99b-a1d7b8ca9ed2 class="margin-NaN">remainingShipments</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5fc88677-54ef-4754-bed0-6db89ec36b05 class="margin-NaN">expiresAt</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8401f164-3cf9-4b0a-bd46-bbe6f7ef4514 class="margin-NaN">isActive</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d7908ca5-f32e-48d0-b488-8a0117ac0f9b class="margin-NaN">paymentMethodId</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.6.2.168.3 **subscription** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>subscription</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="6f07ae76-f095-4c98-83fc-9b19125a2582"></a>

###### 2.1.2.6.2.169 Field **plan**

###### 2.1.2.6.2.169.1 **plan** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>plan</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>free</td></tr></tbody></table>

### <a id="0fc77799-7de0-4fe1-a99b-a1d7b8ca9ed2"></a>

###### 2.1.2.6.2.170 Field **remainingShipments**

###### 2.1.2.6.2.170.1 **remainingShipments** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>remainingShipments</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>15</td></tr></tbody></table>

### <a id="5fc88677-54ef-4754-bed0-6db89ec36b05"></a>

###### 2.1.2.6.2.171 Field **expiresAt**

###### 2.1.2.6.2.171.1 **expiresAt** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>expiresAt</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8401f164-3cf9-4b0a-bd46-bbe6f7ef4514"></a>

###### 2.1.2.6.2.172 Field **isActive**

###### 2.1.2.6.2.172.1 **isActive** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>isActive</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="d7908ca5-f32e-48d0-b488-8a0117ac0f9b"></a>

###### 2.1.2.6.2.173 Field **paymentMethodId**

###### 2.1.2.6.2.173.1 **paymentMethodId** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>paymentMethodId</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="fc0c485a-9b45-4fe8-a77f-eabbcbafcd5a"></a>

###### 2.1.2.6.2.174 Field

###### 2.1.2.6.2.174.1 properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr></tbody></table>

###### 2.1.2.6.3 **customers** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">dbname_1</td><td class="table-column-property">wallet_-1</td><td class="table-column-property">billing_-1</td><td class="table-column-property">slug_-1</td><td class="table-column-property">warehouse.has_shared_products_-1_last_connection_date.unix_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">dbname_1</td><td class="table-column-indexes">wallet_-1</td><td class="table-column-indexes">billing_-1</td><td class="table-column-indexes">slug_-1</td><td class="table-column-indexes">warehouse.has_shared_products_-1_last_connection_date.unix_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">dbname('ascending')</td><td class="table-column-indexes"></td><td class="table-column-indexes">billing('descending')</td><td class="table-column-indexes">slug('descending')</td><td class="table-column-indexes">has_shared_products('descending'), unix('descending')</td></tr></tbody></table>

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">domain_-1</td><td class="table-column-property">_id_</td><td class="table-column-property">email_-1</td><td class="table-column-property">country_ref.iso3_-1</td><td class="table-column-property">warehouse.has_shared_products_1_warehouse.only_my_stores_1_last_connection_date.unix_1_scoring.horas_despacho_1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">domain_-1</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">email_-1</td><td class="table-column-indexes">country_ref.iso3_-1</td><td class="table-column-indexes">warehouse.has_shared_products_1_warehouse.only_my_stores_1_last_connection_date.unix_1_scoring.horas_despacho_1</td></tr><tr><td>Key</td><td class="table-column-indexes"></td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">email('descending')</td><td class="table-column-indexes">iso3('descending')</td><td class="table-column-indexes">has_shared_products('ascending'), unix('ascending')</td></tr></tbody></table>

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">warehouse.verified_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">warehouse.verified_-1</td></tr></tbody></table>

### <a id="relationships"></a>

## 3\. Relationships

### <a id="9be71d53-344d-4713-aff2-0adee88bf92e"></a>

### 3.33 Relationship **customers-users**

#### 3.33.1 **customers-users** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#b3cf6f21-4a4d-4a9d-afec-691df5296b74>customers</a></td><td><a href=#bd0c7b13-73ce-421c-9eea-7225ef09517d>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-admin/image126.png?raw=true)![Hackolade image](Modulo-admin/image127.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#635abd72-5aab-496e-a47e-31cf5060165e>users</a></td><td><a href=#dbff98ec-351a-4317-826d-3b6365572297>client_id</a></td></tr></tbody></table>

#### 3.33.2 **customers-users** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>customers-users</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#b3cf6f21-4a4d-4a9d-afec-691df5296b74>customers</a></td></tr><tr><td>Parent field</td><td><a href=#bd0c7b13-73ce-421c-9eea-7225ef09517d>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#635abd72-5aab-496e-a47e-31cf5060165e>users</a></td></tr><tr><td>Child field</td><td><a href=#dbff98ec-351a-4317-826d-3b6365572297>client_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="5016ed4d-34f1-40c7-805f-580b326b0d00"></a>

### 3.34 Relationship **users-mfa**

#### 3.34.1 **users-mfa** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#635abd72-5aab-496e-a47e-31cf5060165e>users</a></td><td><a href=#7ded5fdf-322e-4b41-b104-4dda07c2c04c>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-admin/image128.png?raw=true)![Hackolade image](Modulo-admin/image129.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#9dfd6d06-1625-47c9-806c-ff10078f8786>mfa</a></td><td><a href=#7e6367e6-e318-49ce-aa8e-eb7e6caf64b1>user_id</a></td></tr></tbody></table>

#### 3.34.2 **users-mfa** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>users-mfa</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#635abd72-5aab-496e-a47e-31cf5060165e>users</a></td></tr><tr><td>Parent field</td><td><a href=#7ded5fdf-322e-4b41-b104-4dda07c2c04c>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#9dfd6d06-1625-47c9-806c-ff10078f8786>mfa</a></td></tr><tr><td>Child field</td><td><a href=#7e6367e6-e318-49ce-aa8e-eb7e6caf64b1>user_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="792ea2f7-b783-41e2-af95-410ff3dea258"></a>

### 3.35 Relationship **users-user\_sessions**

#### 3.35.1 **users-user\_sessions** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#635abd72-5aab-496e-a47e-31cf5060165e>users</a></td><td><a href=#cd4547b7-f02b-4317-b8fc-23d68be8c71a>user</a></td></tr></tbody></table>

![Hackolade image](Modulo-admin/image130.png?raw=true)![Hackolade image](Modulo-admin/image131.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#2620e329-587f-4ad6-936b-0cf39da379f0>user_sessions</a></td><td><a href=#8b8045e1-13bb-42ec-92c4-0b99d3afc064>email</a></td></tr></tbody></table>

#### 3.35.2 **users-user\_sessions** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>users-user_sessions</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#635abd72-5aab-496e-a47e-31cf5060165e>users</a></td></tr><tr><td>Parent field</td><td><a href=#cd4547b7-f02b-4317-b8fc-23d68be8c71a>user</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#2620e329-587f-4ad6-936b-0cf39da379f0>user_sessions</a></td></tr><tr><td>Child field</td><td><a href=#8b8045e1-13bb-42ec-92c4-0b99d3afc064>email</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="61b45523-079f-46eb-ac68-e6c79a716afb"></a>

### 3.36 Relationship **customers-user\_sticker\_guide**

#### 3.36.1 **customers-user\_sticker\_guide** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#b3cf6f21-4a4d-4a9d-afec-691df5296b74>customers</a></td><td><a href=#075e0e77-aa2a-4a97-9b16-8527a6a301b5>dbname</a></td></tr></tbody></table>

![Hackolade image](Modulo-admin/image132.png?raw=true)![Hackolade image](Modulo-admin/image133.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#a2628771-9510-48ad-b4bb-3461c7ac2da1>users_sticker_guide</a></td><td><a href=#51e20567-a0f4-4234-9832-f69555196f67>db_name</a></td></tr></tbody></table>

#### 3.36.2 **customers-user\_sticker\_guide** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>customers-user_sticker_guide</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#b3cf6f21-4a4d-4a9d-afec-691df5296b74>customers</a></td></tr><tr><td>Parent field</td><td><a href=#075e0e77-aa2a-4a97-9b16-8527a6a301b5>dbname</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#a2628771-9510-48ad-b4bb-3461c7ac2da1>users_sticker_guide</a></td></tr><tr><td>Child field</td><td><a href=#51e20567-a0f4-4234-9832-f69555196f67>db_name</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="94e62133-7c1f-4ee7-ab8d-f07c6a0bd4e6"></a>

### 3.37 Relationship **customers-metrics\_use**

#### 3.37.1 **customers-metrics\_use** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#b3cf6f21-4a4d-4a9d-afec-691df5296b74>customers</a></td><td><a href=#bd0c7b13-73ce-421c-9eea-7225ef09517d>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-admin/image134.png?raw=true)![Hackolade image](Modulo-admin/image135.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#e35d3b15-e7a0-46d4-b3e6-523b15c328fd>metrics_use</a></td><td><a href=#0de701c3-d53d-4d23-ac25-33f614aa0d78>store_id</a></td></tr></tbody></table>

#### 3.37.2 **customers-metrics\_use** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>customers-metrics_use</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#b3cf6f21-4a4d-4a9d-afec-691df5296b74>customers</a></td></tr><tr><td>Parent field</td><td><a href=#bd0c7b13-73ce-421c-9eea-7225ef09517d>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#e35d3b15-e7a0-46d4-b3e6-523b15c328fd>metrics_use</a></td></tr><tr><td>Child field</td><td><a href=#0de701c3-d53d-4d23-ac25-33f614aa0d78>store_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="edges"></a>