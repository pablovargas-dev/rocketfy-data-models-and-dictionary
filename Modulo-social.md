     

### <a id="documentation-body"></a>

![Hackolade image](Modulo-social/image1.png?raw=true)

MongoDB Physical Model
----------------------

#### Schema for:

##### Model name: Modelo Ecosistema social

Author: Rocketfy Development Team

Version: 1.0

### <a id="contents"></a>

*   [Table of Contents](#contents)
*   [1\. Model](#model)
*   [2\. Databases](#containers)
    *   [2.1 rocketfy\_social](#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030)
        
        [2.1.2. Collections](#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030-children)
        
        [2.1.2.1 attachments](#3110b6c4-7738-4437-af77-997a0209eab2)
        
        [2.1.2.2 comments](#ca600bb1-368f-4995-9f04-74124feafdba)
        
        [2.1.2.3 courses](#355ab62e-d043-4d61-9433-ae9b23082712)
        
        [2.1.2.4 courses\_categories](#970d314e-cca9-4f99-9df5-3f07c6b8f4b0)
        
        [2.1.2.5 courses\_items](#151d5e73-3715-46a7-9623-3da0faef42fb)
        
        [2.1.2.6 courses\_students](#1964526e-5e24-4114-b088-9fe56c59d7ee)
        
        [2.1.2.7 courses\_views](#53d4250e-9e5f-4b9c-a1f4-fa8275a8fa76)
        
        [2.1.2.8 groups](#08c8e91b-103d-4e25-a982-6753a9d346f4)
        
        [2.1.2.9 members](#28890b55-1cc0-4ee8-b160-64d122d7afe7)
        
        [2.1.2.10 posts](#58d2c416-c138-420d-a88c-16430c02938e)
        
        [2.1.2.11 profiles](#b1686cab-180b-4cc8-9833-91106170efab)
        
        [2.1.2.12 reaction\_types](#db9fa34e-f9da-48e5-8654-548ffee6bae5)
        
        [2.1.2.13 reactions](#a5364c7f-449f-44f2-bae5-2422737da3c0)
        
        [2.1.2.14 refferals\_monthly\_transactions](#0a36268a-2d4b-4f7f-96e9-a34870e54fac)
        
        [2.1.2.15 refferals](#4361851d-09df-4aa8-889f-74e8bccdb9a7)
        
*   [3\. Relationships](#relationships)
    *   [3.17 profiles-posts](#95f5b3a8-9a6f-4219-8590-6ed26b98ac2a)
    *   [3.18 profiles-groups](#cfdb43c2-ddbd-4807-a5a0-b12a395236fe)
    *   [3.19 profiles-members](#5b828669-6ed2-4a23-a6d0-dfa012257b38)
    *   [3.20 posts-comments](#79f2c3b1-16a4-4fc4-8ef1-66f7c1f0e2c5)
    *   [3.21 posts-attachments](#4e2b75bb-2ca5-4f03-93f9-517e5561936b)
    *   [3.22 posts-reactions](#24c550d9-1a24-4ffb-8094-085ef9201721)
    *   [3.23 reactions-reaction\_types](#3153f34e-075d-4ef6-9409-d15cf5135202)
    *   [3.24 profiles-courses](#74a0bfef-cd5c-49d4-a46a-5be153e4a719)
    *   [3.25 courses-courses\_students](#ed505039-0467-406c-b97c-8f4551fb7901)
    *   [3.26 courses-courses\_items](#cad9180e-04d9-4ae1-9fae-ead72349be1b)
    *   [3.27 courses\_categories-courses](#e96ac9f6-0d6f-4b8f-9ef5-92e90659f20b)
    *   [3.28 groups-members](#b10c7d77-9e4d-4fd2-bc42-9e8accedf905)
    *   [3.29 profiles-refferals](#25bc313e-138a-488a-a303-41ba1a513281)
    *   [3.30 refferals-monthly\_transactions](#dc0a24e9-09bd-4b6c-a813-e27aa1cb3db3)

### <a id="model"></a>

## 1\. Model

### 1.1 Model **Rocketfy**

#### 1.1.1 **Rocketfy** Entity Relationship Diagram

![Hackolade image](Modulo-social/image2.png?raw=true)

#### 1.1.2 **Rocketfy** Properties

##### 1.1.2.1 **Details** tab

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td><span>Model name</span></td><td>Rocketfy</td></tr><tr><td><span>Target</span></td><td>MongoDB</td></tr><tr><td><span>DB version</span></td><td>v8.0</td></tr><tr><td><span>Lineage capture</span></td><td></td></tr></tbody></table>

##### 1.1.2.2 **Options** tab

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

#### 1.1.3 **Rocketfy** DB Definitions

### <a id="containers"></a>

## 2\. Databases

### <a id="80bb28e2-9999-4f53-8f5d-0b7ba2dfe030"></a>

### 2.1 Database **rocketfy\_social**

#### 2.1.1 **rocketfy\_social** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Database name</td><td>rocketfy_social</td></tr><tr><td>Activated</td><td>true</td></tr></tbody></table>

### <a id="80bb28e2-9999-4f53-8f5d-0b7ba2dfe030-children"></a>

#### 2.1.2 **rocketfy\_social** Collections

### <a id="3110b6c4-7738-4437-af77-997a0209eab2"></a>

##### 2.1.2.1 Collection **attachments**

###### 2.1.2.1.1 **attachments** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>attachments</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030><span class="name-container">rocketfy_social</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.1.2 **attachments** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#d8072669-3fb3-4291-8a51-c4a9250e4893 class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#52509f75-3879-41ee-afba-71c9ce9f41da class="margin-0">profile_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#084d9535-3623-45d8-b887-d7eabfc8a8b3 class="margin-0">post_id</a></td><td class="no-break-word">objectId,null</td><td>false</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c1a2a080-1e7f-4a91-9085-895209ee2b1e class="margin-0">created_date</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#af1490ad-b379-4e46-8d3f-a8d140e27970 class="margin-0">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2a41f4d4-f0f6-4f2c-97cd-b1f4a9404e1f class="margin-0">type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b79395e2-3840-4769-9ed6-1f41b792e12f class="margin-0">link</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#39771556-2e21-4088-90c7-e347f3ca203f class="margin-0">size</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5439124f-dd76-4dce-983d-46be99d581e6 class="margin-0">format</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7ffd8e7c-b069-488f-88f4-ece19c84268e class="margin-0">slug</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#17397248-1e9a-4035-aad8-49e6f7ff241b class="margin-0">thumbnail</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#14c9cd85-97e9-42fb-b85d-e04b16a3044f class="margin-0">downloadable</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="d8072669-3fb3-4291-8a51-c4a9250e4893"></a>

###### 2.1.2.1.2.1 Field **\_id**

###### 2.1.2.1.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="52509f75-3879-41ee-afba-71c9ce9f41da"></a>

###### 2.1.2.1.2.2 Field **profile\_id**

###### 2.1.2.1.2.2.1 **profile\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>profile_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="084d9535-3623-45d8-b887-d7eabfc8a8b3"></a>

###### 2.1.2.1.2.3 Field **post\_id**

###### 2.1.2.1.2.3.1 **post\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>post_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (objectId,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#58d2c416-c138-420d-a88c-16430c02938e>posts</a></td></tr><tr><td>Foreign field</td><td><a href=#122bb9a0-92b3-40dc-8bf7-2b6933e208fe>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c1a2a080-1e7f-4a91-9085-895209ee2b1e"></a>

###### 2.1.2.1.2.4 Field **created\_date**

###### 2.1.2.1.2.4.1 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1742050712</td></tr></tbody></table>

### <a id="af1490ad-b379-4e46-8d3f-a8d140e27970"></a>

###### 2.1.2.1.2.5 Field **name**

###### 2.1.2.1.2.5.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>lionfootwear_1163591564_images_bota cat 016 sin puntera ocre.jpg</td></tr></tbody></table>

### <a id="2a41f4d4-f0f6-4f2c-97cd-b1f4a9404e1f"></a>

###### 2.1.2.1.2.6 Field **type**

###### 2.1.2.1.2.6.1 **type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>image</td></tr></tbody></table>

### <a id="b79395e2-3840-4769-9ed6-1f41b792e12f"></a>

###### 2.1.2.1.2.7 Field **link**

###### 2.1.2.1.2.7.1 **link** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>link</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://shopping-rocketfy-uploads.s3.amazonaws.com/1658435870279-660981726-lionfootwear_1163591564_images_bota%20cat%20016%20sin%20puntera%20ocre.jpg</td></tr></tbody></table>

### <a id="39771556-2e21-4088-90c7-e347f3ca203f"></a>

###### 2.1.2.1.2.8 Field **size**

###### 2.1.2.1.2.8.1 **size** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>size</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>6704689</td></tr></tbody></table>

### <a id="5439124f-dd76-4dce-983d-46be99d581e6"></a>

###### 2.1.2.1.2.9 Field **format**

###### 2.1.2.1.2.9.1 **format** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>format</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>jpeg</td></tr></tbody></table>

### <a id="7ffd8e7c-b069-488f-88f4-ece19c84268e"></a>

###### 2.1.2.1.2.10 Field **slug**

###### 2.1.2.1.2.10.1 **slug** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>slug</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1658435870279-660981726-lionfootwear_1163591564_images_bota cat 016 sin puntera ocre.jpg</td></tr></tbody></table>

### <a id="17397248-1e9a-4035-aad8-49e6f7ff241b"></a>

###### 2.1.2.1.2.11 Field **thumbnail**

###### 2.1.2.1.2.11.1 **thumbnail** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>thumbnail</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="14c9cd85-97e9-42fb-b85d-e04b16a3044f"></a>

###### 2.1.2.1.2.12 Field **downloadable**

###### 2.1.2.1.2.12.1 **downloadable** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>downloadable</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

###### 2.1.2.1.3 **attachments** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">post_id_1</td><td class="table-column-property">profile_id_1</td><td class="table-column-property">slug_1</td><td class="table-column-property">link_1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">post_id_1</td><td class="table-column-indexes">profile_id_1</td><td class="table-column-indexes">slug_1</td><td class="table-column-indexes">link_1</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">post_id('ascending')</td><td class="table-column-indexes">profile_id('ascending')</td><td class="table-column-indexes">slug('ascending')</td><td class="table-column-indexes">link('ascending')</td></tr></tbody></table>

### <a id="ca600bb1-368f-4995-9f04-74124feafdba"></a>

##### 2.1.2.2 Collection **comments**

###### 2.1.2.2.1 **comments** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>comments</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030><span class="name-container">rocketfy_social</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.2.2 **comments** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#4b187726-6aac-4e93-b3cc-826d404b0647 class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#03cf0b93-3817-41da-9ec5-0fd37e6e0e8a class="margin-0">post_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3d2f2b20-b1ad-4d0f-9663-ffb6a23493d2 class="margin-0">profile_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#28b28fdc-2c11-4fa1-b7b0-c912dbe4830c class="margin-0">type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9998fad8-0b87-47a5-82fa-cdf5e880e920 class="margin-0">text</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#89571fdd-e774-4833-9708-8cf9d38703cc class="margin-0">created_date</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a3452714-11a7-4b03-8c8a-eb0a9347ece1 class="margin-5">unix</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cedf9806-2413-4323-aff6-08b03fcbd3e9 class="margin-5">iso</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4890bd3b-849e-4fd5-9d1e-da924c7ce342 class="margin-5">utc</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b03bc171-7689-42f5-9fbb-79dfe619884d class="margin-5">format</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#dce0f2fd-b7d8-43ba-8025-87f5c56b3ea3 class="margin-0">comment_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="4b187726-6aac-4e93-b3cc-826d404b0647"></a>

###### 2.1.2.2.2.1 Field **\_id**

###### 2.1.2.2.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="03cf0b93-3817-41da-9ec5-0fd37e6e0e8a"></a>

###### 2.1.2.2.2.2 Field **post\_id**

###### 2.1.2.2.2.2.1 **post\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>post_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#58d2c416-c138-420d-a88c-16430c02938e>posts</a></td></tr><tr><td>Foreign field</td><td><a href=#122bb9a0-92b3-40dc-8bf7-2b6933e208fe>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr></tbody></table>

### <a id="3d2f2b20-b1ad-4d0f-9663-ffb6a23493d2"></a>

###### 2.1.2.2.2.3 Field **profile\_id**

###### 2.1.2.2.2.3.1 **profile\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>profile_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="28b28fdc-2c11-4fa1-b7b0-c912dbe4830c"></a>

###### 2.1.2.2.2.4 Field **type**

###### 2.1.2.2.2.4.1 **type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>comment</td></tr></tbody></table>

### <a id="9998fad8-0b87-47a5-82fa-cdf5e880e920"></a>

###### 2.1.2.2.2.5 Field **text**

###### 2.1.2.2.2.5.1 **text** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>text</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Marelvi Store 3223940027</td></tr></tbody></table>

### <a id="89571fdd-e774-4833-9708-8cf9d38703cc"></a>

###### 2.1.2.2.2.6 Field **created\_date**

###### 2.1.2.2.2.6.1 **created\_date** Tree Diagram

![Hackolade image](Modulo-social/image3.png?raw=true)

###### 2.1.2.2.2.6.2 **created\_date** Hierarchy

Parent field: **comments**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#a3452714-11a7-4b03-8c8a-eb0a9347ece1 class="margin-NaN">unix</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cedf9806-2413-4323-aff6-08b03fcbd3e9 class="margin-NaN">iso</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4890bd3b-849e-4fd5-9d1e-da924c7ce342 class="margin-NaN">utc</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b03bc171-7689-42f5-9fbb-79dfe619884d class="margin-NaN">format</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.2.2.6.3 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="a3452714-11a7-4b03-8c8a-eb0a9347ece1"></a>

###### 2.1.2.2.2.7 Field **unix**

###### 2.1.2.2.2.7.1 **unix** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>unix</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1731023053</td></tr></tbody></table>

### <a id="cedf9806-2413-4323-aff6-08b03fcbd3e9"></a>

###### 2.1.2.2.2.8 Field **iso**

###### 2.1.2.2.2.8.1 **iso** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>iso</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>ISODate("2024-11-07T23:44:13.022Z")</td></tr></tbody></table>

### <a id="4890bd3b-849e-4fd5-9d1e-da924c7ce342"></a>

###### 2.1.2.2.2.9 Field **utc**

###### 2.1.2.2.2.9.1 **utc** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>utc</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>-05:00</td></tr></tbody></table>

### <a id="b03bc171-7689-42f5-9fbb-79dfe619884d"></a>

###### 2.1.2.2.2.10 Field **format**

###### 2.1.2.2.2.10.1 **format** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>format</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>07/11/2024 6:44 PM PM</td></tr></tbody></table>

### <a id="dce0f2fd-b7d8-43ba-8025-87f5c56b3ea3"></a>

###### 2.1.2.2.2.11 Field **comment\_id**

###### 2.1.2.2.2.11.1 **comment\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>comment_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

###### 2.1.2.2.3 **comments** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">profile_id_1</td><td class="table-column-property">post_id_1</td><td class="table-column-property">comment_id_1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">profile_id_1</td><td class="table-column-indexes">post_id_1</td><td class="table-column-indexes">comment_id_1</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">profile_id('ascending')</td><td class="table-column-indexes">post_id('ascending')</td><td class="table-column-indexes">comment_id('ascending')</td></tr></tbody></table>

### <a id="355ab62e-d043-4d61-9433-ae9b23082712"></a>

##### 2.1.2.3 Collection **courses**

###### 2.1.2.3.1 **courses** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>courses</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030><span class="name-container">rocketfy_social</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.3.2 **courses** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#4195246a-4b17-4a90-b080-4e352748326b class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk, dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#57160f7b-2fdb-42c2-a1a0-24249a35f1e4 class="margin-0">owner_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4e25e115-4be6-489d-a5de-1ec3d1a1370b class="margin-0">image_pic</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0291a5fa-544b-496b-90ee-1beb3ce33cd9 class="margin-0">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#76824457-b569-4126-98f0-131dfbab5295 class="margin-0">description</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#58525d9f-bd43-476f-a282-0159f36ebf4a class="margin-0">verified</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#745eebd9-902d-4f02-be3b-9695ad63f422 class="margin-0">category_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#da7a6bca-645e-4332-aee7-151c843880ed class="margin-0">items</a></td><td class="no-break-word">array</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2b401302-8ad0-43b2-ba02-a56633695e57 class="margin-5">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#990ac316-e437-490d-b8a9-6c705d99b748 class="margin-0">created_date</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="4195246a-4b17-4a90-b080-4e352748326b"></a>

###### 2.1.2.3.2.1 Field **\_id**

###### 2.1.2.3.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="57160f7b-2fdb-42c2-a1a0-24249a35f1e4"></a>

###### 2.1.2.3.2.2 Field **owner\_id**

###### 2.1.2.3.2.2.1 **owner\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>owner_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#b1686cab-180b-4cc8-9833-91106170efab>profiles</a></td></tr><tr><td>Foreign field</td><td><a href=#d37fb002-9140-4232-8c0a-96b4a4b4a0d8>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr></tbody></table>

### <a id="4e25e115-4be6-489d-a5de-1ec3d1a1370b"></a>

###### 2.1.2.3.2.3 Field **image\_pic**

###### 2.1.2.3.2.3.1 **image\_pic** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>image_pic</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://shopping-rocketfy-uploads.s3.amazonaws.com/1739316090694-245958661-trendread_696246621_images_1000135433.jpg</td></tr></tbody></table>

### <a id="0291a5fa-544b-496b-90ee-1beb3ce33cd9"></a>

###### 2.1.2.3.2.4 Field **name**

###### 2.1.2.3.2.4.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Diplomado Ecommerce en Dropshipping</td></tr></tbody></table>

### <a id="76824457-b569-4126-98f0-131dfbab5295"></a>

###### 2.1.2.3.2.5 Field **description**

###### 2.1.2.3.2.5.1 **description** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>description</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>¡Lanza tu propia tienda online sin necesidad de inventario y con baja inversión!</td></tr></tbody></table>

### <a id="58525d9f-bd43-476f-a282-0159f36ebf4a"></a>

###### 2.1.2.3.2.6 Field **verified**

###### 2.1.2.3.2.6.1 **verified** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>verified</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="745eebd9-902d-4f02-be3b-9695ad63f422"></a>

###### 2.1.2.3.2.7 Field **category\_id**

###### 2.1.2.3.2.7.1 **category\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>category_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#970d314e-cca9-4f99-9df5-3f07c6b8f4b0>courses_categories</a></td></tr><tr><td>Foreign field</td><td><a href=#a27601ea-81a8-47d2-bb61-5da3e02bf920>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr></tbody></table>

### <a id="da7a6bca-645e-4332-aee7-151c843880ed"></a>

###### 2.1.2.3.2.8 Field **items**

###### 2.1.2.3.2.8.1 **items** Tree Diagram

![Hackolade image](Modulo-social/image4.png?raw=true)

###### 2.1.2.3.2.8.2 **items** Hierarchy

Parent field: **courses**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#2b401302-8ad0-43b2-ba02-a56633695e57 class="margin-NaN">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.3.2.8.3 **items** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>items</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="2b401302-8ad0-43b2-ba02-a56633695e57"></a>

###### 2.1.2.3.2.9 Field **\[0\]**

###### 2.1.2.3.2.9.1 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr></tbody></table>

### <a id="990ac316-e437-490d-b8a9-6c705d99b748"></a>

###### 2.1.2.3.2.10 Field **created\_date**

###### 2.1.2.3.2.10.1 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1739316245</td></tr></tbody></table>

###### 2.1.2.3.3 **courses** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td></tr></tbody></table>

### <a id="970d314e-cca9-4f99-9df5-3f07c6b8f4b0"></a>

##### 2.1.2.4 Collection **courses\_categories**

###### 2.1.2.4.1 **courses\_categories** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>courses_categories</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030><span class="name-container">rocketfy_social</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.4.2 **courses\_categories** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#a27601ea-81a8-47d2-bb61-5da3e02bf920 class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk, dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#20843b6f-e70c-41a5-b13e-49ea391989a8 class="margin-0">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a0be6cef-4e56-4d49-930b-2e986017a46a class="margin-0">created_date</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="a27601ea-81a8-47d2-bb61-5da3e02bf920"></a>

###### 2.1.2.4.2.1 Field **\_id**

###### 2.1.2.4.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="20843b6f-e70c-41a5-b13e-49ea391989a8"></a>

###### 2.1.2.4.2.2 Field **name**

###### 2.1.2.4.2.2.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Básico</td></tr></tbody></table>

### <a id="a0be6cef-4e56-4d49-930b-2e986017a46a"></a>

###### 2.1.2.4.2.3 Field **created\_date**

###### 2.1.2.4.2.3.1 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1675787525</td></tr></tbody></table>

###### 2.1.2.4.3 **courses\_categories** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td></tr></tbody></table>

### <a id="151d5e73-3715-46a7-9623-3da0faef42fb"></a>

##### 2.1.2.5 Collection **courses\_items**

###### 2.1.2.5.1 **courses\_items** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>courses_items</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030><span class="name-container">rocketfy_social</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.5.2 **courses\_items** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#83567e3d-b299-4976-8d21-8e99f49032fd class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#36ad5f3a-c27d-408c-b09c-81397029440f class="margin-0">course_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ba776edb-585b-427f-8e96-aa2c5955441f class="margin-0">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#05c9aecd-58c9-4289-922a-3f6b354ec539 class="margin-0">description</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a8dad0b7-56a2-4734-a90a-8d3e95241b72 class="margin-0">youtube_url</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#00d7d0da-fd17-484b-bd5d-bf0672ba7f6a class="margin-0">created_date</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="83567e3d-b299-4976-8d21-8e99f49032fd"></a>

###### 2.1.2.5.2.1 Field **\_id**

###### 2.1.2.5.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="36ad5f3a-c27d-408c-b09c-81397029440f"></a>

###### 2.1.2.5.2.2 Field **course\_id**

###### 2.1.2.5.2.2.1 **course\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>course_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#355ab62e-d043-4d61-9433-ae9b23082712>courses</a></td></tr><tr><td>Foreign field</td><td><a href=#4195246a-4b17-4a90-b080-4e352748326b>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr></tbody></table>

### <a id="ba776edb-585b-427f-8e96-aa2c5955441f"></a>

###### 2.1.2.5.2.3 Field **name**

###### 2.1.2.5.2.3.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>crea tus paginas de ventas</td></tr></tbody></table>

### <a id="05c9aecd-58c9-4289-922a-3f6b354ec539"></a>

###### 2.1.2.5.2.4 Field **description**

###### 2.1.2.5.2.4.1 **description** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>description</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Crea las páginas de ventas en Facebook e Instagram</td></tr></tbody></table>

### <a id="a8dad0b7-56a2-4734-a90a-8d3e95241b72"></a>

###### 2.1.2.5.2.5 Field **youtube\_url**

###### 2.1.2.5.2.5.1 **youtube\_url** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>youtube_url</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://www.youtube.com/watch?v=6RGhdc8Blx0&amp;t=6s</td></tr></tbody></table>

### <a id="00d7d0da-fd17-484b-bd5d-bf0672ba7f6a"></a>

###### 2.1.2.5.2.6 Field **created\_date**

###### 2.1.2.5.2.6.1 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1734795717</td></tr></tbody></table>

###### 2.1.2.5.3 **courses\_items** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td></tr></tbody></table>

### <a id="1964526e-5e24-4114-b088-9fe56c59d7ee"></a>

##### 2.1.2.6 Collection **courses\_students**

###### 2.1.2.6.1 **courses\_students** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>courses_students</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030><span class="name-container">rocketfy_social</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.6.2 **courses\_students** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#66c3e485-d6b4-4455-b67a-890703e5fa8d class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7aa49001-1307-4f72-bf08-36b54c4f7442 class="margin-0">profile_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#804ea9fe-8408-46b0-864b-5e3f9c9c1f19 class="margin-0">course_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d2a79baf-0eef-476c-80b6-fc20b54ac4a4 class="margin-0">taking</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4e296eb6-7c07-4f93-949f-f71d7000e83f class="margin-0">created_date</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="66c3e485-d6b4-4455-b67a-890703e5fa8d"></a>

###### 2.1.2.6.2.1 Field **\_id**

###### 2.1.2.6.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="7aa49001-1307-4f72-bf08-36b54c4f7442"></a>

###### 2.1.2.6.2.2 Field **profile\_id**

###### 2.1.2.6.2.2.1 **profile\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>profile_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="804ea9fe-8408-46b0-864b-5e3f9c9c1f19"></a>

###### 2.1.2.6.2.3 Field **course\_id**

###### 2.1.2.6.2.3.1 **course\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>course_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#355ab62e-d043-4d61-9433-ae9b23082712>courses</a></td></tr><tr><td>Foreign field</td><td><a href=#4195246a-4b17-4a90-b080-4e352748326b>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr></tbody></table>

### <a id="d2a79baf-0eef-476c-80b6-fc20b54ac4a4"></a>

###### 2.1.2.6.2.4 Field **taking**

###### 2.1.2.6.2.4.1 **taking** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>taking</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="4e296eb6-7c07-4f93-949f-f71d7000e83f"></a>

###### 2.1.2.6.2.5 Field **created\_date**

###### 2.1.2.6.2.5.1 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1712818348</td></tr></tbody></table>

###### 2.1.2.6.3 **courses\_students** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td></tr></tbody></table>

### <a id="53d4250e-9e5f-4b9c-a1f4-fa8275a8fa76"></a>

##### 2.1.2.7 Collection **courses\_views**

###### 2.1.2.7.1 **courses\_views** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>courses_views</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030><span class="name-container">rocketfy_social</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.7.2 **courses\_views** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#f0a20619-7ae6-43fe-b74a-f63abb403f0c class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bfa68cf8-68d8-4846-84ee-56673398dcf1 class="margin-0">profile_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#94fe88c4-affd-4a4c-b899-4f3fa5885055 class="margin-0">course_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#52d48b5b-2f6d-43c7-89db-013ea744cc84 class="margin-0">item_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#be4b8c8e-4c2c-4bf4-a402-97dcfe9f4ba7 class="margin-0">created_date</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="f0a20619-7ae6-43fe-b74a-f63abb403f0c"></a>

###### 2.1.2.7.2.1 Field **\_id**

###### 2.1.2.7.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="bfa68cf8-68d8-4846-84ee-56673398dcf1"></a>

###### 2.1.2.7.2.2 Field **profile\_id**

###### 2.1.2.7.2.2.1 **profile\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>profile_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="94fe88c4-affd-4a4c-b899-4f3fa5885055"></a>

###### 2.1.2.7.2.3 Field **course\_id**

###### 2.1.2.7.2.3.1 **course\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>course_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="52d48b5b-2f6d-43c7-89db-013ea744cc84"></a>

###### 2.1.2.7.2.4 Field **item\_id**

###### 2.1.2.7.2.4.1 **item\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>item_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="be4b8c8e-4c2c-4bf4-a402-97dcfe9f4ba7"></a>

###### 2.1.2.7.2.5 Field **created\_date**

###### 2.1.2.7.2.5.1 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1727549692</td></tr></tbody></table>

###### 2.1.2.7.3 **courses\_views** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">item_id_1</td><td class="table-column-property">course_id_1_profile_id_1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">item_id_1</td><td class="table-column-indexes">course_id_1_profile_id_1</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">item_id('ascending')</td><td class="table-column-indexes">course_id('ascending'), profile_id('ascending')</td></tr></tbody></table>

### <a id="08c8e91b-103d-4e25-a982-6753a9d346f4"></a>

##### 2.1.2.8 Collection **groups**

###### 2.1.2.8.1 **groups** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>groups</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030><span class="name-container">rocketfy_social</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.8.2 **groups** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#1b95761a-aab4-45c2-b5a1-d56dd6fe65bf class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk, dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#90f589fb-1f59-400d-abc1-ff2d67f6104d class="margin-0">owner_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8909604a-3308-46c6-8366-bbe524ad46fd class="margin-0">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#46682aca-04c3-4ed4-ac6d-2ad5e4388c8a class="margin-0">type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#151706c7-8bd5-4c26-a66c-5b97c8d371e3 class="margin-0">visibility</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c2e6c074-c513-47f8-8518-1b4d0f8bd42f class="margin-0">country</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a0216484-0865-4fcd-a1aa-df77121e68e4 class="margin-0">profile_pic</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e50a274d-d0fa-4e87-a02a-3219733be167 class="margin-0">banner_pic</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e281b3ab-e55d-4d1e-964a-294de54ce1cb class="margin-0">created_date</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#da974a72-6466-4ac4-a354-9b691cfd3910 class="margin-5">unix</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9fde2ac8-3642-4727-913a-fe4f17d456d4 class="margin-5">iso</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6f06130d-4f9f-44ff-808a-fa12d9522896 class="margin-5">utc</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#22597da9-e473-4f9a-a761-b9fb4c167fb9 class="margin-5">format</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bb27a46f-ea6a-42cc-a758-9c978b1d7e82 class="margin-0">description</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#982c3d97-c6ec-4144-8908-0498ec49d6b6 class="margin-0">verified</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1c393ca5-21cc-4cdc-a5c4-79f700f3f714 class="margin-5">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#11912a41-f682-45c4-8a77-39d00b4b3037 class="margin-5">date</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f7830604-b5f9-4400-8d9d-cd61095fa182 class="margin-5">benefits_limit</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#de7464ce-e156-492b-9ef9-23ce4a18dfcf class="margin-5">list_position</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8787139b-30a7-413c-90b7-da194f4a1d7d class="margin-5">verified</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c2fb96fa-a01e-491f-8c24-23c0e182faea class="margin-10">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#50b8607a-eeb3-4d31-a3b8-be87ad29c33d class="margin-10">date</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0f973815-40a9-4157-881f-f1e196cff6c3 class="margin-0">benefits_limit</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d1e236ae-b1d0-46e4-9550-fc74748c9a87 class="margin-0">list_position</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#46e97c90-0955-4acc-adfe-317eb31b74ae class="margin-0">whatsapp_link</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="1b95761a-aab4-45c2-b5a1-d56dd6fe65bf"></a>

###### 2.1.2.8.2.1 Field **\_id**

###### 2.1.2.8.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="90f589fb-1f59-400d-abc1-ff2d67f6104d"></a>

###### 2.1.2.8.2.2 Field **owner\_id**

###### 2.1.2.8.2.2.1 **owner\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>owner_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#b1686cab-180b-4cc8-9833-91106170efab>profiles</a></td></tr><tr><td>Foreign field</td><td><a href=#d37fb002-9140-4232-8c0a-96b4a4b4a0d8>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr></tbody></table>

### <a id="8909604a-3308-46c6-8366-bbe524ad46fd"></a>

###### 2.1.2.8.2.3 Field **name**

###### 2.1.2.8.2.3.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Mentes ExpertAds</td></tr></tbody></table>

### <a id="46682aca-04c3-4ed4-ac6d-2ad5e4388c8a"></a>

###### 2.1.2.8.2.4 Field **type**

###### 2.1.2.8.2.4.1 **type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Public</td></tr></tbody></table>

### <a id="151706c7-8bd5-4c26-a66c-5b97c8d371e3"></a>

###### 2.1.2.8.2.5 Field **visibility**

###### 2.1.2.8.2.5.1 **visibility** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>visibility</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="c2e6c074-c513-47f8-8518-1b4d0f8bd42f"></a>

###### 2.1.2.8.2.6 Field **country**

###### 2.1.2.8.2.6.1 **country** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>COL</td></tr></tbody></table>

### <a id="a0216484-0865-4fcd-a1aa-df77121e68e4"></a>

###### 2.1.2.8.2.7 Field **profile\_pic**

###### 2.1.2.8.2.7.1 **profile\_pic** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>profile_pic</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://shopping-rocketfy-uploads.s3.amazonaws.com/1741369547196-700207773-todocosas_1474948903_images_Imagen%20de%20WhatsApp%202025-03-07%20a%20las%2010.33.23_0abd2efb.jpg</td></tr></tbody></table>

### <a id="e50a274d-d0fa-4e87-a02a-3219733be167"></a>

###### 2.1.2.8.2.8 Field **banner\_pic**

###### 2.1.2.8.2.8.1 **banner\_pic** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>banner_pic</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://shopping-rocketfy-uploads.s3.amazonaws.com/1741369550575-529474638-todocosas_1474948903_images_Imagen%20de%20WhatsApp%202025-03-07%20a%20las%2010.33.10_b414a488.jpg</td></tr></tbody></table>

### <a id="e281b3ab-e55d-4d1e-964a-294de54ce1cb"></a>

###### 2.1.2.8.2.9 Field **created\_date**

###### 2.1.2.8.2.9.1 **created\_date** Tree Diagram

![Hackolade image](Modulo-social/image5.png?raw=true)

###### 2.1.2.8.2.9.2 **created\_date** Hierarchy

Parent field: **groups**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#da974a72-6466-4ac4-a354-9b691cfd3910 class="margin-NaN">unix</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9fde2ac8-3642-4727-913a-fe4f17d456d4 class="margin-NaN">iso</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6f06130d-4f9f-44ff-808a-fa12d9522896 class="margin-NaN">utc</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#22597da9-e473-4f9a-a761-b9fb4c167fb9 class="margin-NaN">format</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.8.2.9.3 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="da974a72-6466-4ac4-a354-9b691cfd3910"></a>

###### 2.1.2.8.2.10 Field **unix**

###### 2.1.2.8.2.10.1 **unix** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>unix</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1741369633</td></tr></tbody></table>

### <a id="9fde2ac8-3642-4727-913a-fe4f17d456d4"></a>

###### 2.1.2.8.2.11 Field **iso**

###### 2.1.2.8.2.11.1 **iso** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>iso</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>ISODate("2025-03-07T17:47:13.621Z")</td></tr></tbody></table>

### <a id="6f06130d-4f9f-44ff-808a-fa12d9522896"></a>

###### 2.1.2.8.2.12 Field **utc**

###### 2.1.2.8.2.12.1 **utc** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>utc</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>-05:00</td></tr></tbody></table>

### <a id="22597da9-e473-4f9a-a761-b9fb4c167fb9"></a>

###### 2.1.2.8.2.13 Field **format**

###### 2.1.2.8.2.13.1 **format** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>format</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>07/03/2025 12:47 PM PM</td></tr></tbody></table>

### <a id="bb27a46f-ea6a-42cc-a758-9c978b1d7e82"></a>

###### 2.1.2.8.2.14 Field **description**

###### 2.1.2.8.2.14.1 **description** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>description</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Mentes ExpertAds | La comunidad para dominar Meta Ads Estrategias, pruebas y escalado para maximizar resultados</td></tr></tbody></table>

### <a id="982c3d97-c6ec-4144-8908-0498ec49d6b6"></a>

###### 2.1.2.8.2.15 Field **verified**

###### 2.1.2.8.2.15.1 **verified** Tree Diagram

![Hackolade image](Modulo-social/image6.png?raw=true)

###### 2.1.2.8.2.15.2 **verified** Hierarchy

Parent field: **groups**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#1c393ca5-21cc-4cdc-a5c4-79f700f3f714 class="margin-NaN">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#11912a41-f682-45c4-8a77-39d00b4b3037 class="margin-NaN">date</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f7830604-b5f9-4400-8d9d-cd61095fa182 class="margin-NaN">benefits_limit</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#de7464ce-e156-492b-9ef9-23ce4a18dfcf class="margin-NaN">list_position</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8787139b-30a7-413c-90b7-da194f4a1d7d class="margin-NaN">verified</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.8.2.15.3 **verified** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>verified</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="1c393ca5-21cc-4cdc-a5c4-79f700f3f714"></a>

###### 2.1.2.8.2.16 Field **active**

###### 2.1.2.8.2.16.1 **active** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>active</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="11912a41-f682-45c4-8a77-39d00b4b3037"></a>

###### 2.1.2.8.2.17 Field **date**

###### 2.1.2.8.2.17.1 **date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="f7830604-b5f9-4400-8d9d-cd61095fa182"></a>

###### 2.1.2.8.2.18 Field **benefits\_limit**

###### 2.1.2.8.2.18.1 **benefits\_limit** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>benefits_limit</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>50</td></tr></tbody></table>

### <a id="de7464ce-e156-492b-9ef9-23ce4a18dfcf"></a>

###### 2.1.2.8.2.19 Field **list\_position**

###### 2.1.2.8.2.19.1 **list\_position** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>list_position</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="8787139b-30a7-413c-90b7-da194f4a1d7d"></a>

###### 2.1.2.8.2.20 Field **verified**

###### 2.1.2.8.2.20.1 **verified** Tree Diagram

![Hackolade image](Modulo-social/image7.png?raw=true)

###### 2.1.2.8.2.20.2 **verified** Hierarchy

Parent field: **verified**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#c2fb96fa-a01e-491f-8c24-23c0e182faea class="margin-NaN">active</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#50b8607a-eeb3-4d31-a3b8-be87ad29c33d class="margin-NaN">date</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.8.2.20.3 **verified** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>verified</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="c2fb96fa-a01e-491f-8c24-23c0e182faea"></a>

###### 2.1.2.8.2.21 Field **active**

###### 2.1.2.8.2.21.1 **active** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>active</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="50b8607a-eeb3-4d31-a3b8-be87ad29c33d"></a>

###### 2.1.2.8.2.22 Field **date**

###### 2.1.2.8.2.22.1 **date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="0f973815-40a9-4157-881f-f1e196cff6c3"></a>

###### 2.1.2.8.2.23 Field **benefits\_limit**

###### 2.1.2.8.2.23.1 **benefits\_limit** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>benefits_limit</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>250</td></tr></tbody></table>

### <a id="d1e236ae-b1d0-46e4-9550-fc74748c9a87"></a>

###### 2.1.2.8.2.24 Field **list\_position**

###### 2.1.2.8.2.24.1 **list\_position** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>list_position</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>15</td></tr></tbody></table>

### <a id="46e97c90-0955-4acc-adfe-317eb31b74ae"></a>

###### 2.1.2.8.2.25 Field **whatsapp\_link**

###### 2.1.2.8.2.25.1 **whatsapp\_link** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>whatsapp_link</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://chat.whatsapp.com/GCJhD4Gy1zT21P6Ok4mizI</td></tr></tbody></table>

###### 2.1.2.8.3 **groups** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">owner_id_1</td><td class="table-column-property">verified.active_1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">owner_id_1</td><td class="table-column-indexes">verified.active_1</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">owner_id('ascending')</td><td class="table-column-indexes">active('ascending')</td></tr></tbody></table>

### <a id="28890b55-1cc0-4ee8-b160-64d122d7afe7"></a>

##### 2.1.2.9 Collection **members**

###### 2.1.2.9.1 **members** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>members</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030><span class="name-container">rocketfy_social</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.9.2 **members** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#268cd457-6092-4c72-aefc-d44110f6d9be class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1002d0e2-2af8-4924-badf-560d7569cecf class="margin-0">profile_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b497a926-b01e-436f-9eef-15a2f5d60dac class="margin-0">group_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#12e89199-9f73-486b-a431-2ce67d1510e2 class="margin-0">created_date</a></td><td class="no-break-word">document,numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#848b1c16-4062-49f5-ac8c-95fc4eb24fd5 class="margin-5">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6f4effcc-77de-4a8e-bdd5-eb4ccb8a639d class="margin-10">format</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b74429f8-38b2-4835-b4e3-32f73f9a6912 class="margin-10">iso</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d083fbb8-0d96-41ca-8b48-e1f7fb4b922c class="margin-10">unix</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4b05a16b-185a-434d-a6a4-409c6a5c0eb6 class="margin-10">utc</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4f5e27a9-0e6f-4737-97cf-51280ecadc1a class="margin-0">status</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6cbb06e4-a1de-4f00-a6ee-3f0ffd43b617 class="margin-0">disabled_date</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#abd79307-303f-4587-83dd-996eeb778602 class="margin-0">from_verified_group</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="268cd457-6092-4c72-aefc-d44110f6d9be"></a>

###### 2.1.2.9.2.1 Field **\_id**

###### 2.1.2.9.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="1002d0e2-2af8-4924-badf-560d7569cecf"></a>

###### 2.1.2.9.2.2 Field **profile\_id**

###### 2.1.2.9.2.2.1 **profile\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>profile_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#b1686cab-180b-4cc8-9833-91106170efab>profiles</a></td></tr><tr><td>Foreign field</td><td><a href=#d37fb002-9140-4232-8c0a-96b4a4b4a0d8>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr></tbody></table>

### <a id="b497a926-b01e-436f-9eef-15a2f5d60dac"></a>

###### 2.1.2.9.2.3 Field **group\_id**

###### 2.1.2.9.2.3.1 **group\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>group_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#08c8e91b-103d-4e25-a982-6753a9d346f4>groups</a></td></tr><tr><td>Foreign field</td><td><a href=#1b95761a-aab4-45c2-b5a1-d56dd6fe65bf>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr></tbody></table>

### <a id="12e89199-9f73-486b-a431-2ce67d1510e2"></a>

###### 2.1.2.9.2.4 Field **created\_date**

###### 2.1.2.9.2.4.1 **created\_date** Tree Diagram

![Hackolade image](Modulo-social/image8.png?raw=true)

###### 2.1.2.9.2.4.2 **created\_date** Hierarchy

Parent field: **members**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#848b1c16-4062-49f5-ac8c-95fc4eb24fd5 class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.9.2.4.3 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (document,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="848b1c16-4062-49f5-ac8c-95fc4eb24fd5"></a>

###### 2.1.2.9.2.5 Field **properties**

###### 2.1.2.9.2.5.1 **properties** Tree Diagram

![Hackolade image](Modulo-social/image9.png?raw=true)

###### 2.1.2.9.2.5.2 **properties** Hierarchy

Parent field: **created\_date**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#6f4effcc-77de-4a8e-bdd5-eb4ccb8a639d class="margin-NaN">format</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b74429f8-38b2-4835-b4e3-32f73f9a6912 class="margin-NaN">iso</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d083fbb8-0d96-41ca-8b48-e1f7fb4b922c class="margin-NaN">unix</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4b05a16b-185a-434d-a6a4-409c6a5c0eb6 class="margin-NaN">utc</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.9.2.5.3 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="6f4effcc-77de-4a8e-bdd5-eb4ccb8a639d"></a>

###### 2.1.2.9.2.6 Field **format**

###### 2.1.2.9.2.6.1 **format** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>format</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="b74429f8-38b2-4835-b4e3-32f73f9a6912"></a>

###### 2.1.2.9.2.7 Field **iso**

###### 2.1.2.9.2.7.1 **iso** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>iso</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="d083fbb8-0d96-41ca-8b48-e1f7fb4b922c"></a>

###### 2.1.2.9.2.8 Field **unix**

###### 2.1.2.9.2.8.1 **unix** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>unix</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4b05a16b-185a-434d-a6a4-409c6a5c0eb6"></a>

###### 2.1.2.9.2.9 Field **utc**

###### 2.1.2.9.2.9.1 **utc** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>utc</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4f5e27a9-0e6f-4737-97cf-51280ecadc1a"></a>

###### 2.1.2.9.2.10 Field **status**

###### 2.1.2.9.2.10.1 **status** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>status</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>active</td></tr></tbody></table>

### <a id="6cbb06e4-a1de-4f00-a6ee-3f0ffd43b617"></a>

###### 2.1.2.9.2.11 Field **disabled\_date**

###### 2.1.2.9.2.11.1 **disabled\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>disabled_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1741017485</td></tr></tbody></table>

### <a id="abd79307-303f-4587-83dd-996eeb778602"></a>

###### 2.1.2.9.2.12 Field **from\_verified\_group**

###### 2.1.2.9.2.12.1 **from\_verified\_group** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>from_verified_group</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

###### 2.1.2.9.3 **members** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">profile_id_-1</td><td class="table-column-property">group_id_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">profile_id_-1</td><td class="table-column-indexes">group_id_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">profile_id('descending')</td><td class="table-column-indexes">group_id('descending')</td></tr></tbody></table>

### <a id="58d2c416-c138-420d-a88c-16430c02938e"></a>

##### 2.1.2.10 Collection **posts**

###### 2.1.2.10.1 **posts** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>posts</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030><span class="name-container">rocketfy_social</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.10.2 **posts** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#122bb9a0-92b3-40dc-8bf7-2b6933e208fe class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk, dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#066592ad-f65f-4992-bd5e-2ccbee2af4d3 class="margin-0">status</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8e3a9fe5-e03b-45fe-8c1d-68d293c5ca65 class="margin-0">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5c1e8614-c92d-41e3-a033-5151b08ebe13 class="margin-0">description</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#884b9c1b-fcbe-45bf-b913-5683d768a52a class="margin-0">type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3712b0ed-6546-40bb-b674-0b9827471b86 class="margin-0">visibility</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#013392f3-218c-46dc-a16f-2f0c601aad92 class="margin-0">profile_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ae6c235a-bef5-4d44-be93-e638bc088aaa class="margin-0">youtube_url</a></td><td class="no-break-word">null,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#21ed80e3-3d39-47d6-933a-427939b6b9ef class="margin-0">created_date</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#05960782-2bbd-4786-9491-2c107d98b69e class="margin-5">unix</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#adebfe19-c6b2-4bff-8540-c069fa2fd4ca class="margin-5">iso</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#feebb1a7-fedc-40fc-b486-91bb4571eedb class="margin-5">utc</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#00562e38-e089-4da3-a65d-d6a739633d54 class="margin-5">format</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9a4476a8-0221-4330-91db-e874b1bd4c9d class="margin-0">attachments</a></td><td class="no-break-word">null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ff307188-7943-441a-80e7-28358efe8e17 class="margin-0">url_id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#039d668b-d51e-46a8-a3e1-dc37b157e43b class="margin-0">isFromGroup</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9060bfa7-33e1-45d8-8457-ed28fe77e531 class="margin-0">group_id</a></td><td class="no-break-word">null,objectId</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4dab2a5b-d5c7-4bcb-98d9-6d6aca1686e3 class="margin-0">linked_product</a></td><td class="no-break-word">null,document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#98f3843e-14aa-41f0-82f9-8f4835706346 class="margin-5">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ffde27bf-3368-4265-b12d-a648bdfe5404 class="margin-10">country</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a0234d8e-b3c5-4456-99b4-776026daf49b class="margin-10">id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6a5f57e8-f4f9-43ad-8a4d-b9ddd94a0831 class="margin-10">image</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4ca575f2-3562-49a1-aaa3-4a0e7f0c7a80 class="margin-10">link</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c39a8fa4-9533-48d1-b71e-453fcdde0f36 class="margin-10">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a988c6df-828e-46da-86d1-2be2270e0d24 class="margin-10">price</a></td><td class="no-break-word">numeric,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4cb90229-dd1f-4470-ad25-042d8319ca92 class="margin-10">toBuy</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1eb4f7cc-214b-448e-9369-c1e22cedb37f class="margin-10">warehouse_price</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="122bb9a0-92b3-40dc-8bf7-2b6933e208fe"></a>

###### 2.1.2.10.2.1 Field **\_id**

###### 2.1.2.10.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="066592ad-f65f-4992-bd5e-2ccbee2af4d3"></a>

###### 2.1.2.10.2.2 Field **status**

###### 2.1.2.10.2.2.1 **status** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>status</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>active</td></tr></tbody></table>

### <a id="8e3a9fe5-e03b-45fe-8c1d-68d293c5ca65"></a>

###### 2.1.2.10.2.3 Field **name**

###### 2.1.2.10.2.3.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5c1e8614-c92d-41e3-a033-5151b08ebe13"></a>

###### 2.1.2.10.2.4 Field **description**

###### 2.1.2.10.2.4.1 **description** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>description</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>🚨🅰TENCIÓN🔥🚨 Barajador Automático De Cartas Juegos Póker Naipes Mezclador Dropshipping: $ 39.000 Precio Sugerido: $ 59.900 https://app.rocketfy.co/perfil/tiendatht/productos WhatsApp: 3006772610 ⭕ Mezcla bien tus cartas, libera tus manos. ⭕ Tamaño del producto: barajador de cartas: 20x13x10cm. ⭕ Max capacidad: 2 paquetes. ⭕ Rápido y fácil de usar. ⭕ Funciona con Baterías AA. ⭕ Buena calidad: barajador de cartas automático.</td></tr></tbody></table>

### <a id="884b9c1b-fcbe-45bf-b913-5683d768a52a"></a>

###### 2.1.2.10.2.5 Field **type**

###### 2.1.2.10.2.5.1 **type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>simple</td></tr></tbody></table>

### <a id="3712b0ed-6546-40bb-b674-0b9827471b86"></a>

###### 2.1.2.10.2.6 Field **visibility**

###### 2.1.2.10.2.6.1 **visibility** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>visibility</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>public</td></tr></tbody></table>

### <a id="013392f3-218c-46dc-a16f-2f0c601aad92"></a>

###### 2.1.2.10.2.7 Field **profile\_id**

###### 2.1.2.10.2.7.1 **profile\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>profile_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#b1686cab-180b-4cc8-9833-91106170efab>profiles</a></td></tr><tr><td>Foreign field</td><td><a href=#d37fb002-9140-4232-8c0a-96b4a4b4a0d8>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr></tbody></table>

### <a id="ae6c235a-bef5-4d44-be93-e638bc088aaa"></a>

###### 2.1.2.10.2.8 Field **youtube\_url**

###### 2.1.2.10.2.8.1 **youtube\_url** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>youtube_url</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="21ed80e3-3d39-47d6-933a-427939b6b9ef"></a>

###### 2.1.2.10.2.9 Field **created\_date**

###### 2.1.2.10.2.9.1 **created\_date** Tree Diagram

![Hackolade image](Modulo-social/image10.png?raw=true)

###### 2.1.2.10.2.9.2 **created\_date** Hierarchy

Parent field: **posts**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#05960782-2bbd-4786-9491-2c107d98b69e class="margin-NaN">unix</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#adebfe19-c6b2-4bff-8540-c069fa2fd4ca class="margin-NaN">iso</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#feebb1a7-fedc-40fc-b486-91bb4571eedb class="margin-NaN">utc</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#00562e38-e089-4da3-a65d-d6a739633d54 class="margin-NaN">format</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.10.2.9.3 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="05960782-2bbd-4786-9491-2c107d98b69e"></a>

###### 2.1.2.10.2.10 Field **unix**

###### 2.1.2.10.2.10.1 **unix** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>unix</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1742480735</td></tr></tbody></table>

### <a id="adebfe19-c6b2-4bff-8540-c069fa2fd4ca"></a>

###### 2.1.2.10.2.11 Field **iso**

###### 2.1.2.10.2.11.1 **iso** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>iso</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>ISODate("2023-02-08T17:49:51.344Z")</td></tr></tbody></table>

### <a id="feebb1a7-fedc-40fc-b486-91bb4571eedb"></a>

###### 2.1.2.10.2.12 Field **utc**

###### 2.1.2.10.2.12.1 **utc** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>utc</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>-05:00</td></tr></tbody></table>

### <a id="00562e38-e089-4da3-a65d-d6a739633d54"></a>

###### 2.1.2.10.2.13 Field **format**

###### 2.1.2.10.2.13.1 **format** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>format</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>08/02/2023 12:49 PM PM</td></tr></tbody></table>

### <a id="9a4476a8-0221-4330-91db-e874b1bd4c9d"></a>

###### 2.1.2.10.2.14 Field **attachments**

###### 2.1.2.10.2.14.1 **attachments** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>attachments</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ff307188-7943-441a-80e7-28358efe8e17"></a>

###### 2.1.2.10.2.15 Field **url\_id**

###### 2.1.2.10.2.15.1 **url\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>url_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>gbcBHdfrHAd6ZahFm815VR</td></tr></tbody></table>

### <a id="039d668b-d51e-46a8-a3e1-dc37b157e43b"></a>

###### 2.1.2.10.2.16 Field **isFromGroup**

###### 2.1.2.10.2.16.1 **isFromGroup** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>isFromGroup</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="9060bfa7-33e1-45d8-8457-ed28fe77e531"></a>

###### 2.1.2.10.2.17 Field **group\_id**

###### 2.1.2.10.2.17.1 **group\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>group_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,objectId)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4dab2a5b-d5c7-4bcb-98d9-6d6aca1686e3"></a>

###### 2.1.2.10.2.18 Field **linked\_product**

###### 2.1.2.10.2.18.1 **linked\_product** Tree Diagram

![Hackolade image](Modulo-social/image11.png?raw=true)

###### 2.1.2.10.2.18.2 **linked\_product** Hierarchy

Parent field: **posts**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#98f3843e-14aa-41f0-82f9-8f4835706346 class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.10.2.18.3 **linked\_product** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>linked_product</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,document)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="98f3843e-14aa-41f0-82f9-8f4835706346"></a>

###### 2.1.2.10.2.19 Field **properties**

###### 2.1.2.10.2.19.1 **properties** Tree Diagram

![Hackolade image](Modulo-social/image12.png?raw=true)

###### 2.1.2.10.2.19.2 **properties** Hierarchy

Parent field: **linked\_product**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#ffde27bf-3368-4265-b12d-a648bdfe5404 class="margin-NaN">country</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a0234d8e-b3c5-4456-99b4-776026daf49b class="margin-NaN">id</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6a5f57e8-f4f9-43ad-8a4d-b9ddd94a0831 class="margin-NaN">image</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4ca575f2-3562-49a1-aaa3-4a0e7f0c7a80 class="margin-NaN">link</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c39a8fa4-9533-48d1-b71e-453fcdde0f36 class="margin-NaN">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#a988c6df-828e-46da-86d1-2be2270e0d24 class="margin-NaN">price</a></td><td class="no-break-word">numeric,string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4cb90229-dd1f-4470-ad25-042d8319ca92 class="margin-NaN">toBuy</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1eb4f7cc-214b-448e-9369-c1e22cedb37f class="margin-NaN">warehouse_price</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.10.2.19.3 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="ffde27bf-3368-4265-b12d-a648bdfe5404"></a>

###### 2.1.2.10.2.20 Field **country**

###### 2.1.2.10.2.20.1 **country** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a0234d8e-b3c5-4456-99b4-776026daf49b"></a>

###### 2.1.2.10.2.21 Field **id**

###### 2.1.2.10.2.21.1 **id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="6a5f57e8-f4f9-43ad-8a4d-b9ddd94a0831"></a>

###### 2.1.2.10.2.22 Field **image**

###### 2.1.2.10.2.22.1 **image** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>image</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4ca575f2-3562-49a1-aaa3-4a0e7f0c7a80"></a>

###### 2.1.2.10.2.23 Field **link**

###### 2.1.2.10.2.23.1 **link** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>link</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c39a8fa4-9533-48d1-b71e-453fcdde0f36"></a>

###### 2.1.2.10.2.24 Field **name**

###### 2.1.2.10.2.24.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="a988c6df-828e-46da-86d1-2be2270e0d24"></a>

###### 2.1.2.10.2.25 Field **price**

###### 2.1.2.10.2.25.1 **price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="4cb90229-dd1f-4470-ad25-042d8319ca92"></a>

###### 2.1.2.10.2.26 Field **toBuy**

###### 2.1.2.10.2.26.1 **toBuy** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>toBuy</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="1eb4f7cc-214b-448e-9369-c1e22cedb37f"></a>

###### 2.1.2.10.2.27 Field **warehouse\_price**

###### 2.1.2.10.2.27.1 **warehouse\_price** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>warehouse_price</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

###### 2.1.2.10.3 **posts** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">isFromGroup_1</td><td class="table-column-property">profile_id_1</td><td class="table-column-property">status_1</td><td class="table-column-property">group_id_1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">isFromGroup_1</td><td class="table-column-indexes">profile_id_1</td><td class="table-column-indexes">status_1</td><td class="table-column-indexes">group_id_1</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">isFromGroup('ascending')</td><td class="table-column-indexes">profile_id('ascending')</td><td class="table-column-indexes">status('ascending')</td><td class="table-column-indexes">group_id('ascending')</td></tr></tbody></table>

### <a id="b1686cab-180b-4cc8-9833-91106170efab"></a>

##### 2.1.2.11 Collection **profiles**

###### 2.1.2.11.1 **profiles** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>profiles</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030><span class="name-container">rocketfy_social</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.11.2 **profiles** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#d37fb002-9140-4232-8c0a-96b4a4b4a0d8 class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk, dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c8cbd766-50f2-4ebb-bc37-430598fa1c5d class="margin-0">email</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#601360d6-40e8-4bf6-9153-1f947d9d6bc4 class="margin-0">fullname</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b57b9053-7f4e-4c7a-9234-757998e978d0 class="margin-0">lastname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8057675d-fd6c-4e5c-b8ef-e4e17246d13a class="margin-0">description</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#afe05268-8556-47ee-9d6a-774756a429db class="margin-0">profile_pic</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ada3da40-0c3e-4eae-9489-5276d2aa8521 class="margin-0">rol_id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8652be4d-e4e9-4fd3-a3e4-a3c6cbf608c9 class="margin-0">phone</a></td><td class="no-break-word">integer64</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1bcac5b5-bed8-41bd-bcc3-e9f9aba611e8 class="margin-0">utc</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bdfebaca-ed4c-4885-85ac-cb50eebe9c0a class="margin-0">country_id</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4e436acb-44ce-418f-abe3-c907a94a6433 class="margin-0">document</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1ed86b23-c769-4069-8fc5-1d75c287b02a class="margin-0">last_connection_date</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#4988683d-fdf9-4514-8770-c29be76febbb class="margin-0">dbname</a></td><td class="no-break-word">string</td><td>true</td><td>dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d2595172-03cd-45c5-99b9-bbb24f415f43 class="margin-0">slug</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#656b690e-f9fa-41ca-a79c-5d231fb8bc84 class="margin-0">can_publish</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c642d855-5e15-4dd0-818b-ecb1ac545303 class="margin-0">banner_pic</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f3375454-ec3c-4378-a50f-68e4630f36ab class="margin-0">custom_commission</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e6c7f7b5-adba-48c6-8436-4187acc88094 class="margin-5">constant_fee</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e50ffd84-ee27-4274-aaac-804740626572 class="margin-5">rkf_charge_percent</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#70e62bcc-4bd6-482e-bcca-b7b07062bd12 class="margin-5">updated_at</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#31014fe7-5424-4e93-81a6-898e9a5134ec class="margin-0">plan</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d481b6c4-da43-4e55-9927-71b0f28f89b3 class="margin-0">scoring</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6ada6797-21a4-4c80-b9cb-1f116e44588f class="margin-5">activated_months</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ab66f991-06cb-4cfe-93a1-abd21b61e9d2 class="margin-5">evaluadores</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#63fdc1cb-4c73-467d-9551-daaac909196d class="margin-5">final_score</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e0eecf92-fe1d-4ddd-a0f0-d55570afa50b class="margin-5">has_seller_ratings</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d6dcfdd4-ae2f-46cc-a0d0-65c9498beb85 class="margin-5">horas_despacho</a></td><td class="no-break-word">double</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e24095ac-3a88-4440-a2c4-c7322c36d158 class="margin-5">horas_despacho_score</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ca0f224e-f279-4aef-be81-5591c3f01369 class="margin-5">horas_genera_guia</a></td><td class="no-break-word">double</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1e08daf6-562a-41af-af12-04fe9fd3925b class="margin-5">horas_genera_guia_score</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5d7445a6-a52b-4a27-8297-bf2843fc0f5b class="margin-5">last_shipping_date</a></td><td class="no-break-word">date,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#35eaff2e-06ad-4b8a-bdba-a8c691b87ea5 class="margin-5">median_response_time</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#03b34316-7d6b-430e-88cc-ed36afd27a25 class="margin-5">median_response_time_score</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#59be9c4d-a2b3-4154-8d61-8b4ff4c6ddd1 class="margin-5">msgs_calificaciones_sellers</a></td><td class="no-break-word">null,array</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5b1b2cbf-9e5c-4465-adb5-7be6e615f138 class="margin-10">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e564871c-c167-41f5-8c11-1b23428d6fae class="margin-15">[0]</a></td><td class="no-break-word">array</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e5607e79-5b0a-4e8e-aa18-64576c3140ba class="margin-20">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1d8837c9-7026-4450-9eb4-f8704a75e18d class="margin-20">[1]</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#79f953af-5d64-4899-8611-166310ee4f60 class="margin-20">[2]</a></td><td class="no-break-word">date</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cdd544dd-eaa2-403f-a33f-b76883bddbc0 class="margin-5">over_100_shipments</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bb874883-bb94-4fca-94d3-a0122097fc3a class="margin-5">porc_respuesta</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#64a5eb17-41f5-4080-aeb5-f070f283297b class="margin-5">porc_respuesta_score</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ff33ff86-6c46-4d2f-8e6e-712727fb3049 class="margin-5">score</a></td><td class="no-break-word">double</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fa79af97-79f5-4006-ab20-6065e0f53927 class="margin-5">scoring_date</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f22d7f5c-0a4a-4357-83e2-74f76afa0543 class="margin-5">seller_rating</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c88b8997-bb67-424d-b646-bafdda8ba7a1 class="margin-5">seller_rating_score</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#74ca7de6-a1a6-4e1a-b882-11753af0ad2d class="margin-5">store_name</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3c372d5d-6aff-43fd-b43a-725c7540f4ef class="margin-5">total_conversations</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c6ab9759-7efb-4d9b-9948-1f9c9eb27b51 class="margin-5">total_evaluaciones</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3f26d043-07d0-4638-bbfc-64c82f1fdc6d class="margin-5">total_shippings_as_whose</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="d37fb002-9140-4232-8c0a-96b4a4b4a0d8"></a>

###### 2.1.2.11.2.1 Field **\_id**

###### 2.1.2.11.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="c8cbd766-50f2-4ebb-bc37-430598fa1c5d"></a>

###### 2.1.2.11.2.2 Field **email**

###### 2.1.2.11.2.2.1 **email** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>email</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>fashionmodacolombiana1@gmail.com</td></tr></tbody></table>

### <a id="601360d6-40e8-4bf6-9153-1f947d9d6bc4"></a>

###### 2.1.2.11.2.3 Field **fullname**

###### 2.1.2.11.2.3.1 **fullname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fullname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="b57b9053-7f4e-4c7a-9234-757998e978d0"></a>

###### 2.1.2.11.2.4 Field **lastname**

###### 2.1.2.11.2.4.1 **lastname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>lastname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8057675d-fd6c-4e5c-b8ef-e4e17246d13a"></a>

###### 2.1.2.11.2.5 Field **description**

###### 2.1.2.11.2.5.1 **description** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>description</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="afe05268-8556-47ee-9d6a-774756a429db"></a>

###### 2.1.2.11.2.6 Field **profile\_pic**

###### 2.1.2.11.2.6.1 **profile\_pic** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>profile_pic</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://s3-uploads.rocketfy.co/zapatosmujer_1509203294_inbound3182977139202825656.png</td></tr></tbody></table>

### <a id="ada3da40-0c3e-4eae-9489-5276d2aa8521"></a>

###### 2.1.2.11.2.7 Field **rol\_id**

###### 2.1.2.11.2.7.1 **rol\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>rol_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>owner</td></tr></tbody></table>

### <a id="8652be4d-e4e9-4fd3-a3e4-a3c6cbf608c9"></a>

###### 2.1.2.11.2.8 Field **phone**

###### 2.1.2.11.2.8.1 **phone** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>phone</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer64</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>573217816132</td></tr></tbody></table>

### <a id="1bcac5b5-bed8-41bd-bcc3-e9f9aba611e8"></a>

###### 2.1.2.11.2.9 Field **utc**

###### 2.1.2.11.2.9.1 **utc** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>utc</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>-05:00</td></tr></tbody></table>

### <a id="bdfebaca-ed4c-4885-85ac-cb50eebe9c0a"></a>

###### 2.1.2.11.2.10 Field **country\_id**

###### 2.1.2.11.2.10.1 **country\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>country_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>COL</td></tr></tbody></table>

### <a id="4e436acb-44ce-418f-abe3-c907a94a6433"></a>

###### 2.1.2.11.2.11 Field **document**

###### 2.1.2.11.2.11.1 **document** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>document</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="1ed86b23-c769-4069-8fc5-1d75c287b02a"></a>

###### 2.1.2.11.2.12 Field **last\_connection\_date**

###### 2.1.2.11.2.12.1 **last\_connection\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>last_connection_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1742334529</td></tr></tbody></table>

### <a id="4988683d-fdf9-4514-8770-c29be76febbb"></a>

###### 2.1.2.11.2.13 Field **dbname**

###### 2.1.2.11.2.13.1 **dbname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>dbname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>zapatosmujer_1509203294</td></tr></tbody></table>

### <a id="d2595172-03cd-45c5-99b9-bbb24f415f43"></a>

###### 2.1.2.11.2.14 Field **slug**

###### 2.1.2.11.2.14.1 **slug** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>slug</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>zapatosmujer</td></tr></tbody></table>

### <a id="656b690e-f9fa-41ca-a79c-5d231fb8bc84"></a>

###### 2.1.2.11.2.15 Field **can\_publish**

###### 2.1.2.11.2.15.1 **can\_publish** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>can_publish</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="c642d855-5e15-4dd0-818b-ecb1ac545303"></a>

###### 2.1.2.11.2.16 Field **banner\_pic**

###### 2.1.2.11.2.16.1 **banner\_pic** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>banner_pic</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>https://s3-uploads.rocketfy.co/zapatosmujer_1509203294_inbound8444627585987522292.png</td></tr></tbody></table>

### <a id="f3375454-ec3c-4378-a50f-68e4630f36ab"></a>

###### 2.1.2.11.2.17 Field **custom\_commission**

###### 2.1.2.11.2.17.1 **custom\_commission** Tree Diagram

![Hackolade image](Modulo-social/image13.png?raw=true)

###### 2.1.2.11.2.17.2 **custom\_commission** Hierarchy

Parent field: **profiles**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#e6c7f7b5-adba-48c6-8436-4187acc88094 class="margin-NaN">constant_fee</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e50ffd84-ee27-4274-aaac-804740626572 class="margin-NaN">rkf_charge_percent</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#70e62bcc-4bd6-482e-bcca-b7b07062bd12 class="margin-NaN">updated_at</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.11.2.17.3 **custom\_commission** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>custom_commission</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="e6c7f7b5-adba-48c6-8436-4187acc88094"></a>

###### 2.1.2.11.2.18 Field **constant\_fee**

###### 2.1.2.11.2.18.1 **constant\_fee** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>constant_fee</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="e50ffd84-ee27-4274-aaac-804740626572"></a>

###### 2.1.2.11.2.19 Field **rkf\_charge\_percent**

###### 2.1.2.11.2.19.1 **rkf\_charge\_percent** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>rkf_charge_percent</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>0</td></tr></tbody></table>

### <a id="70e62bcc-4bd6-482e-bcca-b7b07062bd12"></a>

###### 2.1.2.11.2.20 Field **updated\_at**

###### 2.1.2.11.2.20.1 **updated\_at** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>updated_at</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1733155553</td></tr></tbody></table>

### <a id="31014fe7-5424-4e93-81a6-898e9a5134ec"></a>

###### 2.1.2.11.2.21 Field **plan**

###### 2.1.2.11.2.21.1 **plan** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>plan</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>basic</td></tr></tbody></table>

### <a id="d481b6c4-da43-4e55-9927-71b0f28f89b3"></a>

###### 2.1.2.11.2.22 Field **scoring**

###### 2.1.2.11.2.22.1 **scoring** Tree Diagram

![Hackolade image](Modulo-social/image14.png?raw=true)

###### 2.1.2.11.2.22.2 **scoring** Hierarchy

Parent field: **profiles**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#6ada6797-21a4-4c80-b9cb-1f116e44588f class="margin-NaN">activated_months</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ab66f991-06cb-4cfe-93a1-abd21b61e9d2 class="margin-NaN">evaluadores</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#63fdc1cb-4c73-467d-9551-daaac909196d class="margin-NaN">final_score</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e0eecf92-fe1d-4ddd-a0f0-d55570afa50b class="margin-NaN">has_seller_ratings</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d6dcfdd4-ae2f-46cc-a0d0-65c9498beb85 class="margin-NaN">horas_despacho</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e24095ac-3a88-4440-a2c4-c7322c36d158 class="margin-NaN">horas_despacho_score</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ca0f224e-f279-4aef-be81-5591c3f01369 class="margin-NaN">horas_genera_guia</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1e08daf6-562a-41af-af12-04fe9fd3925b class="margin-NaN">horas_genera_guia_score</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5d7445a6-a52b-4a27-8297-bf2843fc0f5b class="margin-NaN">last_shipping_date</a></td><td class="no-break-word">date,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#35eaff2e-06ad-4b8a-bdba-a8c691b87ea5 class="margin-NaN">median_response_time</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#03b34316-7d6b-430e-88cc-ed36afd27a25 class="margin-NaN">median_response_time_score</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#59be9c4d-a2b3-4154-8d61-8b4ff4c6ddd1 class="margin-NaN">msgs_calificaciones_sellers</a></td><td class="no-break-word">null,array</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cdd544dd-eaa2-403f-a33f-b76883bddbc0 class="margin-NaN">over_100_shipments</a></td><td class="no-break-word">boolean</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#bb874883-bb94-4fca-94d3-a0122097fc3a class="margin-NaN">porc_respuesta</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#64a5eb17-41f5-4080-aeb5-f070f283297b class="margin-NaN">porc_respuesta_score</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ff33ff86-6c46-4d2f-8e6e-712727fb3049 class="margin-NaN">score</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#fa79af97-79f5-4006-ab20-6065e0f53927 class="margin-NaN">scoring_date</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#f22d7f5c-0a4a-4357-83e2-74f76afa0543 class="margin-NaN">seller_rating</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c88b8997-bb67-424d-b646-bafdda8ba7a1 class="margin-NaN">seller_rating_score</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#74ca7de6-a1a6-4e1a-b882-11753af0ad2d class="margin-NaN">store_name</a></td><td class="no-break-word">string,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3c372d5d-6aff-43fd-b43a-725c7540f4ef class="margin-NaN">total_conversations</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c6ab9759-7efb-4d9b-9948-1f9c9eb27b51 class="margin-NaN">total_evaluaciones</a></td><td class="no-break-word">null,numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#3f26d043-07d0-4638-bbfc-64c82f1fdc6d class="margin-NaN">total_shippings_as_whose</a></td><td class="no-break-word">numeric,null</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.11.2.22.3 **scoring** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>scoring</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="6ada6797-21a4-4c80-b9cb-1f116e44588f"></a>

###### 2.1.2.11.2.23 Field **activated\_months**

###### 2.1.2.11.2.23.1 **activated\_months** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>activated_months</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="ab66f991-06cb-4cfe-93a1-abd21b61e9d2"></a>

###### 2.1.2.11.2.24 Field **evaluadores**

###### 2.1.2.11.2.24.1 **evaluadores** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>evaluadores</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="63fdc1cb-4c73-467d-9551-daaac909196d"></a>

###### 2.1.2.11.2.25 Field **final\_score**

###### 2.1.2.11.2.25.1 **final\_score** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>final_score</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>3</td></tr></tbody></table>

### <a id="e0eecf92-fe1d-4ddd-a0f0-d55570afa50b"></a>

###### 2.1.2.11.2.26 Field **has\_seller\_ratings**

###### 2.1.2.11.2.26.1 **has\_seller\_ratings** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>has_seller_ratings</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="d6dcfdd4-ae2f-46cc-a0d0-65c9498beb85"></a>

###### 2.1.2.11.2.27 Field **horas\_despacho**

###### 2.1.2.11.2.27.1 **horas\_despacho** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>horas_despacho</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>16.3</td></tr></tbody></table>

### <a id="e24095ac-3a88-4440-a2c4-c7322c36d158"></a>

###### 2.1.2.11.2.28 Field **horas\_despacho\_score**

###### 2.1.2.11.2.28.1 **horas\_despacho\_score** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>horas_despacho_score</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>4</td></tr></tbody></table>

### <a id="ca0f224e-f279-4aef-be81-5591c3f01369"></a>

###### 2.1.2.11.2.29 Field **horas\_genera\_guia**

###### 2.1.2.11.2.29.1 **horas\_genera\_guia** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>horas_genera_guia</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>23.9</td></tr></tbody></table>

### <a id="1e08daf6-562a-41af-af12-04fe9fd3925b"></a>

###### 2.1.2.11.2.30 Field **horas\_genera\_guia\_score**

###### 2.1.2.11.2.30.1 **horas\_genera\_guia\_score** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>horas_genera_guia_score</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>3</td></tr></tbody></table>

### <a id="5d7445a6-a52b-4a27-8297-bf2843fc0f5b"></a>

###### 2.1.2.11.2.31 Field **last\_shipping\_date**

###### 2.1.2.11.2.31.1 **last\_shipping\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>last_shipping_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (date,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="35eaff2e-06ad-4b8a-bdba-a8c691b87ea5"></a>

###### 2.1.2.11.2.32 Field **median\_response\_time**

###### 2.1.2.11.2.32.1 **median\_response\_time** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>median_response_time</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="03b34316-7d6b-430e-88cc-ed36afd27a25"></a>

###### 2.1.2.11.2.33 Field **median\_response\_time\_score**

###### 2.1.2.11.2.33.1 **median\_response\_time\_score** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>median_response_time_score</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="59be9c4d-a2b3-4154-8d61-8b4ff4c6ddd1"></a>

###### 2.1.2.11.2.34 Field **msgs\_calificaciones\_sellers**

###### 2.1.2.11.2.34.1 **msgs\_calificaciones\_sellers** Tree Diagram

![Hackolade image](Modulo-social/image15.png?raw=true)

###### 2.1.2.11.2.34.2 **msgs\_calificaciones\_sellers** Hierarchy

Parent field: **scoring**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#5b1b2cbf-9e5c-4465-adb5-7be6e615f138 class="margin-NaN">items</a></td><td class="no-break-word">multipleArray</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.11.2.34.3 **msgs\_calificaciones\_sellers** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>msgs_calificaciones_sellers</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,array)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5b1b2cbf-9e5c-4465-adb5-7be6e615f138"></a>

###### 2.1.2.11.2.35 Field **items**

###### 2.1.2.11.2.35.1 **items** Tree Diagram

![Hackolade image](Modulo-social/image16.png?raw=true)

###### 2.1.2.11.2.35.2 **items** Hierarchy

Parent field: **msgs\_calificaciones\_sellers**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#e564871c-c167-41f5-8c11-1b23428d6fae class="margin-NaN">[0]</a></td><td class="no-break-word">array</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.11.2.35.3 **items** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="e564871c-c167-41f5-8c11-1b23428d6fae"></a>

###### 2.1.2.11.2.36 Field **\[0\]**

###### 2.1.2.11.2.36.1 **\[0\]** Tree Diagram

![Hackolade image](Modulo-social/image17.png?raw=true)

###### 2.1.2.11.2.36.2 **\[0\]** Hierarchy

Parent field: **items**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#e5607e79-5b0a-4e8e-aa18-64576c3140ba class="margin-NaN">[0]</a></td><td class="no-break-word">string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1d8837c9-7026-4450-9eb4-f8704a75e18d class="margin-NaN">[1]</a></td><td class="no-break-word">numeric</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#79f953af-5d64-4899-8611-166310ee4f60 class="margin-NaN">[2]</a></td><td class="no-break-word">date</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.11.2.36.3 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="e5607e79-5b0a-4e8e-aa18-64576c3140ba"></a>

###### 2.1.2.11.2.37 Field **\[0\]**

###### 2.1.2.11.2.37.1 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr></tbody></table>

### <a id="1d8837c9-7026-4450-9eb4-f8704a75e18d"></a>

###### 2.1.2.11.2.38 Field **\[1\]**

###### 2.1.2.11.2.38.1 **\[1\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr></tbody></table>

### <a id="79f953af-5d64-4899-8611-166310ee4f60"></a>

###### 2.1.2.11.2.39 Field **\[2\]**

###### 2.1.2.11.2.39.1 **\[2\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="cdd544dd-eaa2-403f-a33f-b76883bddbc0"></a>

###### 2.1.2.11.2.40 Field **over\_100\_shipments**

###### 2.1.2.11.2.40.1 **over\_100\_shipments** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>over_100_shipments</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>false</td></tr></tbody></table>

### <a id="bb874883-bb94-4fca-94d3-a0122097fc3a"></a>

###### 2.1.2.11.2.41 Field **porc\_respuesta**

###### 2.1.2.11.2.41.1 **porc\_respuesta** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>porc_respuesta</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>100</td></tr></tbody></table>

### <a id="64a5eb17-41f5-4080-aeb5-f070f283297b"></a>

###### 2.1.2.11.2.42 Field **porc\_respuesta\_score**

###### 2.1.2.11.2.42.1 **porc\_respuesta\_score** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>porc_respuesta_score</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>4</td></tr></tbody></table>

### <a id="ff33ff86-6c46-4d2f-8e6e-712727fb3049"></a>

###### 2.1.2.11.2.43 Field **score**

###### 2.1.2.11.2.43.1 **score** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>score</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>double</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>2.9499999999999997</td></tr></tbody></table>

### <a id="fa79af97-79f5-4006-ab20-6065e0f53927"></a>

###### 2.1.2.11.2.44 Field **scoring\_date**

###### 2.1.2.11.2.44.1 **scoring\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>scoring_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>ISODate("2024-02-01")</td></tr></tbody></table>

### <a id="f22d7f5c-0a4a-4357-83e2-74f76afa0543"></a>

###### 2.1.2.11.2.45 Field **seller\_rating**

###### 2.1.2.11.2.45.1 **seller\_rating** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>seller_rating</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="c88b8997-bb67-424d-b646-bafdda8ba7a1"></a>

###### 2.1.2.11.2.46 Field **seller\_rating\_score**

###### 2.1.2.11.2.46.1 **seller\_rating\_score** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>seller_rating_score</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>4</td></tr></tbody></table>

### <a id="74ca7de6-a1a6-4e1a-b882-11753af0ad2d"></a>

###### 2.1.2.11.2.47 Field **store\_name**

###### 2.1.2.11.2.47.1 **store\_name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>store_name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="3c372d5d-6aff-43fd-b43a-725c7540f4ef"></a>

###### 2.1.2.11.2.48 Field **total\_conversations**

###### 2.1.2.11.2.48.1 **total\_conversations** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>total_conversations</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>3</td></tr></tbody></table>

### <a id="c6ab9759-7efb-4d9b-9948-1f9c9eb27b51"></a>

###### 2.1.2.11.2.49 Field **total\_evaluaciones**

###### 2.1.2.11.2.49.1 **total\_evaluaciones** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>total_evaluaciones</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,numeric)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="3f26d043-07d0-4638-bbfc-64c82f1fdc6d"></a>

###### 2.1.2.11.2.50 Field **total\_shippings\_as\_whose**

###### 2.1.2.11.2.50.1 **total\_shippings\_as\_whose** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>total_shippings_as_whose</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (numeric,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

###### 2.1.2.11.3 **profiles** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">dbname_1</td><td class="table-column-property">email_1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">dbname_1</td><td class="table-column-indexes">email_1</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">dbname('ascending')</td><td class="table-column-indexes">email('ascending')</td></tr></tbody></table>

### <a id="db9fa34e-f9da-48e5-8654-548ffee6bae5"></a>

##### 2.1.2.12 Collection **reaction\_types**

###### 2.1.2.12.1 **reaction\_types** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>reaction_types</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030><span class="name-container">rocketfy_social</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.12.2 **reaction\_types** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#c140a2cd-6f4d-4b33-b0d6-d1432a6acf2a class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk, dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#19789781-bf13-4f7e-83c5-1062573d3cc7 class="margin-0">type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1d1e42ee-0c65-44e8-ae02-08e68b3e6696 class="margin-0">icon</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7ed39bda-a7b6-409c-a6a5-3b0730114fca class="margin-0">name</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#583e2787-fde7-4b69-9e00-04277b300fd9 class="margin-0">feeling</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="c140a2cd-6f4d-4b33-b0d6-d1432a6acf2a"></a>

###### 2.1.2.12.2.1 Field **\_id**

###### 2.1.2.12.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="19789781-bf13-4f7e-83c5-1062573d3cc7"></a>

###### 2.1.2.12.2.2 Field **type**

###### 2.1.2.12.2.2.1 **type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>like</td></tr></tbody></table>

### <a id="1d1e42ee-0c65-44e8-ae02-08e68b3e6696"></a>

###### 2.1.2.12.2.3 Field **icon**

###### 2.1.2.12.2.3.1 **icon** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>icon</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>thumbs-up</td></tr></tbody></table>

### <a id="7ed39bda-a7b6-409c-a6a5-3b0730114fca"></a>

###### 2.1.2.12.2.4 Field **name**

###### 2.1.2.12.2.4.1 **name** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>name</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>Me gusta</td></tr></tbody></table>

### <a id="583e2787-fde7-4b69-9e00-04277b300fd9"></a>

###### 2.1.2.12.2.5 Field **feeling**

###### 2.1.2.12.2.5.1 **feeling** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>feeling</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1</td></tr></tbody></table>

###### 2.1.2.12.3 **reaction\_types** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td></tr></tbody></table>

### <a id="a5364c7f-449f-44f2-bae5-2422737da3c0"></a>

##### 2.1.2.13 Collection **reactions**

###### 2.1.2.13.1 **reactions** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>reactions</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030><span class="name-container">rocketfy_social</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.13.2 **reactions** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#56609945-5688-41f8-8ce4-82248d174242 class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b9b4c635-cd78-481d-9244-ff92bc9cb962 class="margin-0">post_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#7172d4a3-07dd-43d1-9364-67b61cca1607 class="margin-0">profile_id</a></td><td class="no-break-word">objectId</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#0ae82904-6101-4cdb-9ac5-36a1496f6258 class="margin-0">created_date</a></td><td class="no-break-word">document</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#c772757b-dd12-459e-bc7c-6d5ca84c924e class="margin-5">unix</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#955c180f-336c-4051-aa6c-5e50339bad5a class="margin-5">iso</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9ea6fddc-953a-4dea-8ffa-3cc10a7438c3 class="margin-5">utc</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9a33b639-5780-46c3-b8d7-a0199b196c3e class="margin-5">format</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8071f203-cbd6-4ec4-ba9f-3531517ea9df class="margin-0">type_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="56609945-5688-41f8-8ce4-82248d174242"></a>

###### 2.1.2.13.2.1 Field **\_id**

###### 2.1.2.13.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="b9b4c635-cd78-481d-9244-ff92bc9cb962"></a>

###### 2.1.2.13.2.2 Field **post\_id**

###### 2.1.2.13.2.2.1 **post\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>post_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#58d2c416-c138-420d-a88c-16430c02938e>posts</a></td></tr><tr><td>Foreign field</td><td><a href=#122bb9a0-92b3-40dc-8bf7-2b6933e208fe>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr></tbody></table>

### <a id="7172d4a3-07dd-43d1-9364-67b61cca1607"></a>

###### 2.1.2.13.2.3 Field **profile\_id**

###### 2.1.2.13.2.3.1 **profile\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>profile_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="0ae82904-6101-4cdb-9ac5-36a1496f6258"></a>

###### 2.1.2.13.2.4 Field **created\_date**

###### 2.1.2.13.2.4.1 **created\_date** Tree Diagram

![Hackolade image](Modulo-social/image18.png?raw=true)

###### 2.1.2.13.2.4.2 **created\_date** Hierarchy

Parent field: **reactions**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#c772757b-dd12-459e-bc7c-6d5ca84c924e class="margin-NaN">unix</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#955c180f-336c-4051-aa6c-5e50339bad5a class="margin-NaN">iso</a></td><td class="no-break-word">date</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9ea6fddc-953a-4dea-8ffa-3cc10a7438c3 class="margin-NaN">utc</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#9a33b639-5780-46c3-b8d7-a0199b196c3e class="margin-NaN">format</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.13.2.4.3 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="c772757b-dd12-459e-bc7c-6d5ca84c924e"></a>

###### 2.1.2.13.2.5 Field **unix**

###### 2.1.2.13.2.5.1 **unix** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>unix</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1743441559</td></tr></tbody></table>

### <a id="955c180f-336c-4051-aa6c-5e50339bad5a"></a>

###### 2.1.2.13.2.6 Field **iso**

###### 2.1.2.13.2.6.1 **iso** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>iso</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>date</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>ISODate("2025-01-07T03:36:17.803Z")</td></tr></tbody></table>

### <a id="9ea6fddc-953a-4dea-8ffa-3cc10a7438c3"></a>

###### 2.1.2.13.2.7 Field **utc**

###### 2.1.2.13.2.7.1 **utc** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>utc</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>-05:00</td></tr></tbody></table>

### <a id="9a33b639-5780-46c3-b8d7-a0199b196c3e"></a>

###### 2.1.2.13.2.8 Field **format**

###### 2.1.2.13.2.8.1 **format** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>format</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>06/01/2025 10:36 PM PM</td></tr></tbody></table>

### <a id="8071f203-cbd6-4ec4-ba9f-3531517ea9df"></a>

###### 2.1.2.13.2.9 Field **type\_id**

###### 2.1.2.13.2.9.1 **type\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>type_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#db9fa34e-f9da-48e5-8654-548ffee6bae5>reaction_types</a></td></tr><tr><td>Foreign field</td><td><a href=#c140a2cd-6f4d-4b33-b0d6-d1432a6acf2a>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr></tbody></table>

###### 2.1.2.13.3 **reactions** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">profile_id_1</td><td class="table-column-property">post_id_1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">profile_id_1</td><td class="table-column-indexes">post_id_1</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">profile_id('ascending')</td><td class="table-column-indexes">post_id('ascending')</td></tr></tbody></table>

### <a id="0a36268a-2d4b-4f7f-96e9-a34870e54fac"></a>

##### 2.1.2.14 Collection **refferals\_monthly\_transactions**

###### 2.1.2.14.1 **refferals\_monthly\_transactions** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>refferals_monthly_transactions</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030><span class="name-container">rocketfy_social</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.14.2 **refferals\_monthly\_transactions** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#47f93990-6680-46d1-8f01-af522ddc217b class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5a012fe7-4840-441d-abcd-41a8ac1f0499 class="margin-0">refferal_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#105f7f69-e382-404d-9299-779aab068f10 class="margin-0">year</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#04cf7774-971c-42b3-a5c7-10c1e49cad5b class="margin-0">month</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#d30e23c2-8a3e-4ea3-a80e-cafa642da5e2 class="margin-0">count</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#6f050443-15d6-4b2b-8621-1b9958659508 class="margin-0">customer_refferal_dbname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#02c2e9bd-43e2-4a02-97a5-a59f8ede44d9 class="margin-0">created_by_script</a></td><td class="no-break-word">string,boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#5ae65dbb-c1ce-4213-935f-830166bbf29c class="margin-0">from_community</a></td><td class="no-break-word">null,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="47f93990-6680-46d1-8f01-af522ddc217b"></a>

###### 2.1.2.14.2.1 Field **\_id**

###### 2.1.2.14.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="5a012fe7-4840-441d-abcd-41a8ac1f0499"></a>

###### 2.1.2.14.2.2 Field **refferal\_id**

###### 2.1.2.14.2.2.1 **refferal\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>refferal_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#4361851d-09df-4aa8-889f-74e8bccdb9a7>refferals</a></td></tr><tr><td>Foreign field</td><td><a href=#2b69fdd4-083b-4754-adeb-0ea66b3ac90b>_id</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr></tbody></table>

### <a id="105f7f69-e382-404d-9299-779aab068f10"></a>

###### 2.1.2.14.2.3 Field **year**

###### 2.1.2.14.2.3.1 **year** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>year</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>2025</td></tr></tbody></table>

### <a id="04cf7774-971c-42b3-a5c7-10c1e49cad5b"></a>

###### 2.1.2.14.2.4 Field **month**

###### 2.1.2.14.2.4.1 **month** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>month</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>12</td></tr></tbody></table>

### <a id="d30e23c2-8a3e-4ea3-a80e-cafa642da5e2"></a>

###### 2.1.2.14.2.5 Field **count**

###### 2.1.2.14.2.5.1 **count** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>count</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>5341</td></tr></tbody></table>

### <a id="6f050443-15d6-4b2b-8621-1b9958659508"></a>

###### 2.1.2.14.2.6 Field **customer\_refferal\_dbname**

###### 2.1.2.14.2.6.1 **customer\_refferal\_dbname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>customer_refferal_dbname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>techhobbies_1561669675</td></tr></tbody></table>

### <a id="02c2e9bd-43e2-4a02-97a5-a59f8ede44d9"></a>

###### 2.1.2.14.2.7 Field **created\_by\_script**

###### 2.1.2.14.2.7.1 **created\_by\_script** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_by_script</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,boolean)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="5ae65dbb-c1ce-4213-935f-830166bbf29c"></a>

###### 2.1.2.14.2.8 Field **from\_community**

###### 2.1.2.14.2.8.1 **from\_community** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>from_community</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

###### 2.1.2.14.3 **refferals\_monthly\_transactions** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">customer_refferal_dbname_-1</td><td class="table-column-property">year_-1</td><td class="table-column-property">month_-1</td><td class="table-column-property">compound_duplicate_index</td><td class="table-column-property">from_community_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">customer_refferal_dbname_-1</td><td class="table-column-indexes">year_-1</td><td class="table-column-indexes">month_-1</td><td class="table-column-indexes">compound_duplicate_index</td><td class="table-column-indexes">from_community_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">customer_refferal_dbname('descending')</td><td class="table-column-indexes">year('descending')</td><td class="table-column-indexes">month('descending')</td><td class="table-column-indexes">refferal_id('descending'), customer_refferal_dbname('descending'), year('descending'), month('descending')</td><td class="table-column-indexes">from_community('descending')</td></tr><tr><td>Unique</td><td class="table-column-indexes"></td><td class="table-column-indexes"></td><td class="table-column-indexes"></td><td class="table-column-indexes">true</td><td class="table-column-indexes"></td></tr></tbody></table>

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">_id_</td><td class="table-column-property">refferal_id_-1</td><td class="table-column-property">customer_refferal_dbname_-1_refferal_id_-1</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">_id_</td><td class="table-column-indexes">refferal_id_-1</td><td class="table-column-indexes">customer_refferal_dbname_-1_refferal_id_-1</td></tr><tr><td>Key</td><td class="table-column-indexes">_id('ascending')</td><td class="table-column-indexes">refferal_id('descending')</td><td class="table-column-indexes">customer_refferal_dbname('descending'), refferal_id('descending')</td></tr></tbody></table>

### <a id="4361851d-09df-4aa8-889f-74e8bccdb9a7"></a>

##### 2.1.2.15 Collection **refferals**

###### 2.1.2.15.1 **refferals** Properties

<table class="collection-properties-table"><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Collection name</td><td>refferals</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Database</td><td><a href=#80bb28e2-9999-4f53-8f5d-0b7ba2dfe030><span class="name-container">rocketfy_social</span></a></td></tr><tr><td>Storage engine</td><td>WiredTiger</td></tr><tr><td>Validation level</td><td>Off</td></tr><tr><td>Validation action</td><td>Warn</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

###### 2.1.2.15.2 **refferals** Fields

<table><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#2b69fdd4-083b-4754-adeb-0ea66b3ac90b class="margin-0">_id</a></td><td class="no-break-word">objectId</td><td>true</td><td>pk, dk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cba96dd0-79c1-49a2-b4b5-38218452d646 class="margin-0">status</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b1308861-54ed-4984-97fa-6b6cecfe0f71 class="margin-0">customer_email</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#233a48f6-2f74-47ff-882d-7124568adaad class="margin-0">customer_dbname</a></td><td class="no-break-word">string,null</td><td>false</td><td>fk</td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2a931822-1081-4d68-b1bd-36c294e2164e class="margin-0">customer_refferal_dbname</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#95c45215-76c4-46b1-8a77-1eb5ddd6135a class="margin-0">goal</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#58ca897c-3fdc-4153-992f-e8b91d78f4d9 class="margin-0">goal_type</a></td><td class="no-break-word">string</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#ca675eee-d2b2-43e7-986d-105dedd7d2bd class="margin-0">reward</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e385f681-a2dc-4835-a76e-b8d08a211b7b class="margin-0">created_date</a></td><td class="no-break-word">integer32</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#79a464ff-4775-40c7-8932-d27e5d20c25f class="margin-0">redeem</a></td><td class="no-break-word">null,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#689321cc-8b7c-4daa-9860-56f1d2850f3d class="margin-0">from_community</a></td><td class="no-break-word">null,string</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2fe7e79c-2a60-4dae-b6bc-f619da041d03 class="margin-0">created_by_script</a></td><td class="no-break-word">string,boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e49835c4-c7db-4ea0-88c6-af1a87285887 class="margin-0">custom_commission</a></td><td class="no-break-word">null,document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b960953e-3cc9-44de-8d8a-f442aae5c892 class="margin-5">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#eb4749de-5266-4dda-b6e1-bd05269e1f2e class="margin-10">constant_fee</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#930e000a-f292-41ea-b3fa-fd0af6919d76 class="margin-10">rkf_charge_percent</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#2170be2f-b9d3-49d7-b1a4-7a426f74e557 class="margin-0">date_referido</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#716699ea-63ad-4fd5-963a-79ea1ce1683e class="margin-0">disabled_date</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#cd0b7dba-21c1-4fa3-998a-47c1ad403fab class="margin-0">fromCommunity</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#1b0701da-7e80-404d-b288-b44108f578e5 class="margin-0">latest_shipping_date</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#461fbab6-a39f-4ea0-9f90-3c5c0333f16f class="margin-0">monthly_shippings</a></td><td class="no-break-word">array</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#e8cfecf3-ee0c-47d7-8c5d-b8a3158ac688 class="margin-5">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#db47f814-33a4-4a00-bd9c-d4289402e2ac class="margin-10">count</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#76f91df5-881b-44f8-adf2-08673102cb17 class="margin-10">month</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8bbd9398-0892-42e5-bd1b-f6f6b821696b class="margin-10">year</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#00b6f548-5ee5-4ba0-8147-5d026990e672 class="margin-0">referral_bonus_processed</a></td><td class="no-break-word">boolean</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#b6dec793-4581-40eb-ba91-fef2b23ef4f5 class="margin-0">shippings_total_count</a></td><td class="no-break-word">integer32</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

### <a id="2b69fdd4-083b-4754-adeb-0ea66b3ac90b"></a>

###### 2.1.2.15.2.1 Field **\_id**

###### 2.1.2.15.2.1.1 **\_id** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>_id</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>objectId</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>true</td></tr></tbody></table>

### <a id="cba96dd0-79c1-49a2-b4b5-38218452d646"></a>

###### 2.1.2.15.2.2 Field **status**

###### 2.1.2.15.2.2.1 **status** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>status</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>approved</td></tr></tbody></table>

### <a id="b1308861-54ed-4984-97fa-6b6cecfe0f71"></a>

###### 2.1.2.15.2.3 Field **customer\_email**

###### 2.1.2.15.2.3.1 **customer\_email** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>customer_email</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>edvid44@gmail.com</td></tr></tbody></table>

### <a id="233a48f6-2f74-47ff-882d-7124568adaad"></a>

###### 2.1.2.15.2.4 Field **customer\_dbname**

###### 2.1.2.15.2.4.1 **customer\_dbname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>customer_dbname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,null)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Foreign collection</td><td><a href=#b1686cab-180b-4cc8-9833-91106170efab>profiles</a></td></tr><tr><td>Foreign field</td><td><a href=#4988683d-fdf9-4514-8770-c29be76febbb>dbname</a></td></tr><tr><td>Relationship type</td><td>Foreign Key</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="2a931822-1081-4d68-b1bd-36c294e2164e"></a>

###### 2.1.2.15.2.5 Field **customer\_refferal\_dbname**

###### 2.1.2.15.2.5.1 **customer\_refferal\_dbname** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>customer_refferal_dbname</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>comunidad30x_238750753</td></tr></tbody></table>

### <a id="95c45215-76c4-46b1-8a77-1eb5ddd6135a"></a>

###### 2.1.2.15.2.6 Field **goal**

###### 2.1.2.15.2.6.1 **goal** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>goal</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1000</td></tr></tbody></table>

### <a id="58ca897c-3fdc-4153-992f-e8b91d78f4d9"></a>

###### 2.1.2.15.2.7 Field **goal\_type**

###### 2.1.2.15.2.7.1 **goal\_type** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>goal_type</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>orders</td></tr></tbody></table>

### <a id="ca675eee-d2b2-43e7-986d-105dedd7d2bd"></a>

###### 2.1.2.15.2.8 Field **reward**

###### 2.1.2.15.2.8.1 **reward** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>reward</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>500</td></tr></tbody></table>

### <a id="e385f681-a2dc-4835-a76e-b8d08a211b7b"></a>

###### 2.1.2.15.2.9 Field **created\_date**

###### 2.1.2.15.2.9.1 **created\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1743177825</td></tr></tbody></table>

### <a id="79a464ff-4775-40c7-8932-d27e5d20c25f"></a>

###### 2.1.2.15.2.10 Field **redeem**

###### 2.1.2.15.2.10.1 **redeem** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>redeem</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="689321cc-8b7c-4daa-9860-56f1d2850f3d"></a>

###### 2.1.2.15.2.11 Field **from\_community**

###### 2.1.2.15.2.11.1 **from\_community** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>from_community</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,string)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="2fe7e79c-2a60-4dae-b6bc-f619da041d03"></a>

###### 2.1.2.15.2.12 Field **created\_by\_script**

###### 2.1.2.15.2.12.1 **created\_by\_script** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>created_by_script</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (string,boolean)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>string</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="e49835c4-c7db-4ea0-88c6-af1a87285887"></a>

###### 2.1.2.15.2.13 Field **custom\_commission**

###### 2.1.2.15.2.13.1 **custom\_commission** Tree Diagram

![Hackolade image](Modulo-social/image19.png?raw=true)

###### 2.1.2.15.2.13.2 **custom\_commission** Hierarchy

Parent field: **refferals**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#b960953e-3cc9-44de-8d8a-f442aae5c892 class="margin-NaN">properties</a></td><td class="no-break-word">multipleDocument</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.15.2.13.3 **custom\_commission** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>custom_commission</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>multiple (null,document)</td></tr><tr><td></td><td>[object Object],[object Object]</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>null</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td></td><td></td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="b960953e-3cc9-44de-8d8a-f442aae5c892"></a>

###### 2.1.2.15.2.14 Field **properties**

###### 2.1.2.15.2.14.1 **properties** Tree Diagram

![Hackolade image](Modulo-social/image20.png?raw=true)

###### 2.1.2.15.2.14.2 **properties** Hierarchy

Parent field: **custom\_commission**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#eb4749de-5266-4dda-b6e1-bd05269e1f2e class="margin-NaN">constant_fee</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#930e000a-f292-41ea-b3fa-fd0af6919d76 class="margin-NaN">rkf_charge_percent</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.15.2.14.3 **properties** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody></tbody></table>

### <a id="eb4749de-5266-4dda-b6e1-bd05269e1f2e"></a>

###### 2.1.2.15.2.15 Field **constant\_fee**

###### 2.1.2.15.2.15.1 **constant\_fee** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>constant_fee</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="930e000a-f292-41ea-b3fa-fd0af6919d76"></a>

###### 2.1.2.15.2.16 Field **rkf\_charge\_percent**

###### 2.1.2.15.2.16.1 **rkf\_charge\_percent** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>rkf_charge_percent</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="2170be2f-b9d3-49d7-b1a4-7a426f74e557"></a>

###### 2.1.2.15.2.17 Field **date\_referido**

###### 2.1.2.15.2.17.1 **date\_referido** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>date_referido</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1715039280</td></tr></tbody></table>

### <a id="716699ea-63ad-4fd5-963a-79ea1ce1683e"></a>

###### 2.1.2.15.2.18 Field **disabled\_date**

###### 2.1.2.15.2.18.1 **disabled\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>disabled_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1742702879</td></tr></tbody></table>

### <a id="cd0b7dba-21c1-4fa3-998a-47c1ad403fab"></a>

###### 2.1.2.15.2.19 Field **fromCommunity**

###### 2.1.2.15.2.19.1 **fromCommunity** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>fromCommunity</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="1b0701da-7e80-404d-b288-b44108f578e5"></a>

###### 2.1.2.15.2.20 Field **latest\_shipping\_date**

###### 2.1.2.15.2.20.1 **latest\_shipping\_date** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>latest_shipping_date</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>1743293897</td></tr></tbody></table>

### <a id="461fbab6-a39f-4ea0-9f90-3c5c0333f16f"></a>

###### 2.1.2.15.2.21 Field **monthly\_shippings**

###### 2.1.2.15.2.21.1 **monthly\_shippings** Tree Diagram

![Hackolade image](Modulo-social/image21.png?raw=true)

###### 2.1.2.15.2.21.2 **monthly\_shippings** Hierarchy

Parent field: **refferals**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#e8cfecf3-ee0c-47d7-8c5d-b8a3158ac688 class="margin-NaN">[0]</a></td><td class="no-break-word">document</td><td>false</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.15.2.21.3 **monthly\_shippings** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>monthly_shippings</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>array</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Additional items</td><td>true</td></tr></tbody></table>

### <a id="e8cfecf3-ee0c-47d7-8c5d-b8a3158ac688"></a>

###### 2.1.2.15.2.22 Field **\[0\]**

###### 2.1.2.15.2.22.1 **\[0\]** Tree Diagram

![Hackolade image](Modulo-social/image22.png?raw=true)

###### 2.1.2.15.2.22.2 **\[0\]** Hierarchy

Parent field: **monthly\_shippings**

Child field(s):

<table class="field-properties-table"><thead><tr><td>Field</td><td>Type</td><td>Req</td><td>Key</td><td>Description</td><td>Comments</td></tr></thead><tbody><tr><td><a href=#db47f814-33a4-4a00-bd9c-d4289402e2ac class="margin-NaN">count</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#76f91df5-881b-44f8-adf2-08673102cb17 class="margin-NaN">month</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr><tr><td><a href=#8bbd9398-0892-42e5-bd1b-f6f6b821696b class="margin-NaN">year</a></td><td class="no-break-word">numeric</td><td>true</td><td></td><td><div class="docs-markdown"></div></td><td><div class="docs-markdown"></div></td></tr></tbody></table>

###### 2.1.2.15.2.22.3 **\[0\]** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>document</td></tr><tr><td>Additional properties</td><td>true</td></tr></tbody></table>

### <a id="db47f814-33a4-4a00-bd9c-d4289402e2ac"></a>

###### 2.1.2.15.2.23 Field **count**

###### 2.1.2.15.2.23.1 **count** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>count</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="76f91df5-881b-44f8-adf2-08673102cb17"></a>

###### 2.1.2.15.2.24 Field **month**

###### 2.1.2.15.2.24.1 **month** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>month</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="8bbd9398-0892-42e5-bd1b-f6f6b821696b"></a>

###### 2.1.2.15.2.25 Field **year**

###### 2.1.2.15.2.25.1 **year** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>year</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Required</td><td>true</td></tr><tr><td>Primary key</td><td>false</td></tr></tbody></table>

### <a id="00b6f548-5ee5-4ba0-8147-5d026990e672"></a>

###### 2.1.2.15.2.26 Field **referral\_bonus\_processed**

###### 2.1.2.15.2.26.1 **referral\_bonus\_processed** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>referral_bonus_processed</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>boolean</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>true</td></tr></tbody></table>

### <a id="b6dec793-4581-40eb-ba91-fef2b23ef4f5"></a>

###### 2.1.2.15.2.27 Field **shippings\_total\_count**

###### 2.1.2.15.2.27.1 **shippings\_total\_count** properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>shippings_total_count</td></tr><tr><td>Activated</td><td>true</td></tr><tr><td>Type</td><td>numeric</td></tr><tr><td>Subtype</td><td>integer32</td></tr><tr><td>Required</td><td>false</td></tr><tr><td>Primary key</td><td>false</td></tr><tr><td>Sample</td><td>13</td></tr></tbody></table>

###### 2.1.2.15.3 **refferals** Indexes

<table class="index-table"><thead><tr><td class="table-property-column">Property</td><td class="table-column-property">customer_refferal_dbname_-1</td><td class="table-column-property">customer_dbname_-1</td><td class="table-column-property">from_community_-1</td><td class="table-column-property">_id_</td></tr></thead><tbody><tr><td>Name</td><td class="table-column-indexes">customer_refferal_dbname_-1</td><td class="table-column-indexes">customer_dbname_-1</td><td class="table-column-indexes">from_community_-1</td><td class="table-column-indexes">_id_</td></tr><tr><td>Key</td><td class="table-column-indexes">customer_refferal_dbname('descending')</td><td class="table-column-indexes">customer_dbname('descending')</td><td class="table-column-indexes">from_community('descending')</td><td class="table-column-indexes">_id('ascending')</td></tr></tbody></table>

### <a id="relationships"></a>

## 3\. Relationships

### <a id="95f5b3a8-9a6f-4219-8590-6ed26b98ac2a"></a>

### 3.17 Relationship **profiles-posts**

#### 3.17.1 **profiles-posts** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#b1686cab-180b-4cc8-9833-91106170efab>profiles</a></td><td><a href=#d37fb002-9140-4232-8c0a-96b4a4b4a0d8>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-social/image55.png?raw=true)![Hackolade image](Modulo-social/image56.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#58d2c416-c138-420d-a88c-16430c02938e>posts</a></td><td><a href=#013392f3-218c-46dc-a16f-2f0c601aad92>profile_id</a></td></tr></tbody></table>

#### 3.17.2 **profiles-posts** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>profiles-posts</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#b1686cab-180b-4cc8-9833-91106170efab>profiles</a></td></tr><tr><td>Parent field</td><td><a href=#d37fb002-9140-4232-8c0a-96b4a4b4a0d8>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#58d2c416-c138-420d-a88c-16430c02938e>posts</a></td></tr><tr><td>Child field</td><td><a href=#013392f3-218c-46dc-a16f-2f0c601aad92>profile_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="cfdb43c2-ddbd-4807-a5a0-b12a395236fe"></a>

### 3.18 Relationship **profiles-groups**

#### 3.18.1 **profiles-groups** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#b1686cab-180b-4cc8-9833-91106170efab>profiles</a></td><td><a href=#d37fb002-9140-4232-8c0a-96b4a4b4a0d8>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-social/image57.png?raw=true)![Hackolade image](Modulo-social/image58.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#08c8e91b-103d-4e25-a982-6753a9d346f4>groups</a></td><td><a href=#90f589fb-1f59-400d-abc1-ff2d67f6104d>owner_id</a></td></tr></tbody></table>

#### 3.18.2 **profiles-groups** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>profiles-groups</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#b1686cab-180b-4cc8-9833-91106170efab>profiles</a></td></tr><tr><td>Parent field</td><td><a href=#d37fb002-9140-4232-8c0a-96b4a4b4a0d8>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#08c8e91b-103d-4e25-a982-6753a9d346f4>groups</a></td></tr><tr><td>Child field</td><td><a href=#90f589fb-1f59-400d-abc1-ff2d67f6104d>owner_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="5b828669-6ed2-4a23-a6d0-dfa012257b38"></a>

### 3.19 Relationship **profiles-members**

#### 3.19.1 **profiles-members** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#b1686cab-180b-4cc8-9833-91106170efab>profiles</a></td><td><a href=#d37fb002-9140-4232-8c0a-96b4a4b4a0d8>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-social/image59.png?raw=true)![Hackolade image](Modulo-social/image60.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#28890b55-1cc0-4ee8-b160-64d122d7afe7>members</a></td><td><a href=#1002d0e2-2af8-4924-badf-560d7569cecf>profile_id</a></td></tr></tbody></table>

#### 3.19.2 **profiles-members** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>profiles-members</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#b1686cab-180b-4cc8-9833-91106170efab>profiles</a></td></tr><tr><td>Parent field</td><td><a href=#d37fb002-9140-4232-8c0a-96b4a4b4a0d8>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#28890b55-1cc0-4ee8-b160-64d122d7afe7>members</a></td></tr><tr><td>Child field</td><td><a href=#1002d0e2-2af8-4924-badf-560d7569cecf>profile_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="79f2c3b1-16a4-4fc4-8ef1-66f7c1f0e2c5"></a>

### 3.20 Relationship **posts-comments**

#### 3.20.1 **posts-comments** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#58d2c416-c138-420d-a88c-16430c02938e>posts</a></td><td><a href=#122bb9a0-92b3-40dc-8bf7-2b6933e208fe>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-social/image61.png?raw=true)![Hackolade image](Modulo-social/image62.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#ca600bb1-368f-4995-9f04-74124feafdba>comments</a></td><td><a href=#03cf0b93-3817-41da-9ec5-0fd37e6e0e8a>post_id</a></td></tr></tbody></table>

#### 3.20.2 **posts-comments** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>posts-comments</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#58d2c416-c138-420d-a88c-16430c02938e>posts</a></td></tr><tr><td>Parent field</td><td><a href=#122bb9a0-92b3-40dc-8bf7-2b6933e208fe>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#ca600bb1-368f-4995-9f04-74124feafdba>comments</a></td></tr><tr><td>Child field</td><td><a href=#03cf0b93-3817-41da-9ec5-0fd37e6e0e8a>post_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="4e2b75bb-2ca5-4f03-93f9-517e5561936b"></a>

### 3.21 Relationship **posts-attachments**

#### 3.21.1 **posts-attachments** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#58d2c416-c138-420d-a88c-16430c02938e>posts</a></td><td><a href=#122bb9a0-92b3-40dc-8bf7-2b6933e208fe>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-social/image63.png?raw=true)![Hackolade image](Modulo-social/image64.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#3110b6c4-7738-4437-af77-997a0209eab2>attachments</a></td><td><a href=#084d9535-3623-45d8-b887-d7eabfc8a8b3>post_id</a></td></tr></tbody></table>

#### 3.21.2 **posts-attachments** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>posts-attachments</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#58d2c416-c138-420d-a88c-16430c02938e>posts</a></td></tr><tr><td>Parent field</td><td><a href=#122bb9a0-92b3-40dc-8bf7-2b6933e208fe>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#3110b6c4-7738-4437-af77-997a0209eab2>attachments</a></td></tr><tr><td>Child field</td><td><a href=#084d9535-3623-45d8-b887-d7eabfc8a8b3>post_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="24c550d9-1a24-4ffb-8094-085ef9201721"></a>

### 3.22 Relationship **posts-reactions**

#### 3.22.1 **posts-reactions** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#58d2c416-c138-420d-a88c-16430c02938e>posts</a></td><td><a href=#122bb9a0-92b3-40dc-8bf7-2b6933e208fe>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-social/image65.png?raw=true)![Hackolade image](Modulo-social/image66.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#a5364c7f-449f-44f2-bae5-2422737da3c0>reactions</a></td><td><a href=#b9b4c635-cd78-481d-9244-ff92bc9cb962>post_id</a></td></tr></tbody></table>

#### 3.22.2 **posts-reactions** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>posts-reactions</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#58d2c416-c138-420d-a88c-16430c02938e>posts</a></td></tr><tr><td>Parent field</td><td><a href=#122bb9a0-92b3-40dc-8bf7-2b6933e208fe>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#a5364c7f-449f-44f2-bae5-2422737da3c0>reactions</a></td></tr><tr><td>Child field</td><td><a href=#b9b4c635-cd78-481d-9244-ff92bc9cb962>post_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="3153f34e-075d-4ef6-9409-d15cf5135202"></a>

### 3.23 Relationship **reactions-reaction\_types**

#### 3.23.1 **reactions-reaction\_types** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#db9fa34e-f9da-48e5-8654-548ffee6bae5>reaction_types</a></td><td><a href=#c140a2cd-6f4d-4b33-b0d6-d1432a6acf2a>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-social/image67.png?raw=true)![Hackolade image](Modulo-social/image68.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#a5364c7f-449f-44f2-bae5-2422737da3c0>reactions</a></td><td><a href=#8071f203-cbd6-4ec4-ba9f-3531517ea9df>type_id</a></td></tr></tbody></table>

#### 3.23.2 **reactions-reaction\_types** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>reactions-reaction_types</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#db9fa34e-f9da-48e5-8654-548ffee6bae5>reaction_types</a></td></tr><tr><td>Parent field</td><td><a href=#c140a2cd-6f4d-4b33-b0d6-d1432a6acf2a>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#a5364c7f-449f-44f2-bae5-2422737da3c0>reactions</a></td></tr><tr><td>Child field</td><td><a href=#8071f203-cbd6-4ec4-ba9f-3531517ea9df>type_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="74a0bfef-cd5c-49d4-a46a-5be153e4a719"></a>

### 3.24 Relationship **profiles-courses**

#### 3.24.1 **profiles-courses** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#b1686cab-180b-4cc8-9833-91106170efab>profiles</a></td><td><a href=#d37fb002-9140-4232-8c0a-96b4a4b4a0d8>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-social/image69.png?raw=true)![Hackolade image](Modulo-social/image70.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#355ab62e-d043-4d61-9433-ae9b23082712>courses</a></td><td><a href=#57160f7b-2fdb-42c2-a1a0-24249a35f1e4>owner_id</a></td></tr></tbody></table>

#### 3.24.2 **profiles-courses** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>profiles-courses</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#b1686cab-180b-4cc8-9833-91106170efab>profiles</a></td></tr><tr><td>Parent field</td><td><a href=#d37fb002-9140-4232-8c0a-96b4a4b4a0d8>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#355ab62e-d043-4d61-9433-ae9b23082712>courses</a></td></tr><tr><td>Child field</td><td><a href=#57160f7b-2fdb-42c2-a1a0-24249a35f1e4>owner_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="ed505039-0467-406c-b97c-8f4551fb7901"></a>

### 3.25 Relationship **courses-courses\_students**

#### 3.25.1 **courses-courses\_students** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#355ab62e-d043-4d61-9433-ae9b23082712>courses</a></td><td><a href=#4195246a-4b17-4a90-b080-4e352748326b>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-social/image71.png?raw=true)![Hackolade image](Modulo-social/image72.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#1964526e-5e24-4114-b088-9fe56c59d7ee>courses_students</a></td><td><a href=#804ea9fe-8408-46b0-864b-5e3f9c9c1f19>course_id</a></td></tr></tbody></table>

#### 3.25.2 **courses-courses\_students** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>courses-courses_students</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#355ab62e-d043-4d61-9433-ae9b23082712>courses</a></td></tr><tr><td>Parent field</td><td><a href=#4195246a-4b17-4a90-b080-4e352748326b>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#1964526e-5e24-4114-b088-9fe56c59d7ee>courses_students</a></td></tr><tr><td>Child field</td><td><a href=#804ea9fe-8408-46b0-864b-5e3f9c9c1f19>course_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="cad9180e-04d9-4ae1-9fae-ead72349be1b"></a>

### 3.26 Relationship **courses-courses\_items**

#### 3.26.1 **courses-courses\_items** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#355ab62e-d043-4d61-9433-ae9b23082712>courses</a></td><td><a href=#4195246a-4b17-4a90-b080-4e352748326b>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-social/image73.png?raw=true)![Hackolade image](Modulo-social/image74.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#151d5e73-3715-46a7-9623-3da0faef42fb>courses_items</a></td><td><a href=#36ad5f3a-c27d-408c-b09c-81397029440f>course_id</a></td></tr></tbody></table>

#### 3.26.2 **courses-courses\_items** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>courses-courses_items</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#355ab62e-d043-4d61-9433-ae9b23082712>courses</a></td></tr><tr><td>Parent field</td><td><a href=#4195246a-4b17-4a90-b080-4e352748326b>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#151d5e73-3715-46a7-9623-3da0faef42fb>courses_items</a></td></tr><tr><td>Child field</td><td><a href=#36ad5f3a-c27d-408c-b09c-81397029440f>course_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="e96ac9f6-0d6f-4b8f-9ef5-92e90659f20b"></a>

### 3.27 Relationship **courses\_categories-courses**

#### 3.27.1 **courses\_categories-courses** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#970d314e-cca9-4f99-9df5-3f07c6b8f4b0>courses_categories</a></td><td><a href=#a27601ea-81a8-47d2-bb61-5da3e02bf920>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-social/image75.png?raw=true)![Hackolade image](Modulo-social/image76.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#355ab62e-d043-4d61-9433-ae9b23082712>courses</a></td><td><a href=#745eebd9-902d-4f02-be3b-9695ad63f422>category_id</a></td></tr></tbody></table>

#### 3.27.2 **courses\_categories-courses** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>courses_categories-courses</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#970d314e-cca9-4f99-9df5-3f07c6b8f4b0>courses_categories</a></td></tr><tr><td>Parent field</td><td><a href=#a27601ea-81a8-47d2-bb61-5da3e02bf920>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#355ab62e-d043-4d61-9433-ae9b23082712>courses</a></td></tr><tr><td>Child field</td><td><a href=#745eebd9-902d-4f02-be3b-9695ad63f422>category_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="b10c7d77-9e4d-4fd2-bc42-9e8accedf905"></a>

### 3.28 Relationship **groups-members**

#### 3.28.1 **groups-members** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#08c8e91b-103d-4e25-a982-6753a9d346f4>groups</a></td><td><a href=#1b95761a-aab4-45c2-b5a1-d56dd6fe65bf>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-social/image77.png?raw=true)![Hackolade image](Modulo-social/image78.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#28890b55-1cc0-4ee8-b160-64d122d7afe7>members</a></td><td><a href=#b497a926-b01e-436f-9eef-15a2f5d60dac>group_id</a></td></tr></tbody></table>

#### 3.28.2 **groups-members** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>groups-members</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#08c8e91b-103d-4e25-a982-6753a9d346f4>groups</a></td></tr><tr><td>Parent field</td><td><a href=#1b95761a-aab4-45c2-b5a1-d56dd6fe65bf>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#28890b55-1cc0-4ee8-b160-64d122d7afe7>members</a></td></tr><tr><td>Child field</td><td><a href=#b497a926-b01e-436f-9eef-15a2f5d60dac>group_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="25bc313e-138a-488a-a303-41ba1a513281"></a>

### 3.29 Relationship **profiles-refferals**

#### 3.29.1 **profiles-refferals** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#b1686cab-180b-4cc8-9833-91106170efab>profiles</a></td><td><a href=#4988683d-fdf9-4514-8770-c29be76febbb>dbname</a></td></tr></tbody></table>

![Hackolade image](Modulo-social/image79.png?raw=true)![Hackolade image](Modulo-social/image80.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#4361851d-09df-4aa8-889f-74e8bccdb9a7>refferals</a></td><td><a href=#233a48f6-2f74-47ff-882d-7124568adaad>customer_dbname</a></td></tr></tbody></table>

#### 3.29.2 **profiles-refferals** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>profiles-refferals</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#b1686cab-180b-4cc8-9833-91106170efab>profiles</a></td></tr><tr><td>Parent field</td><td><a href=#4988683d-fdf9-4514-8770-c29be76febbb>dbname</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#4361851d-09df-4aa8-889f-74e8bccdb9a7>refferals</a></td></tr><tr><td>Child field</td><td><a href=#233a48f6-2f74-47ff-882d-7124568adaad>customer_dbname</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

### <a id="dc0a24e9-09bd-4b6c-a813-e27aa1cb3db3"></a>

### 3.30 Relationship **refferals-monthly\_transactions**

#### 3.30.1 **refferals-monthly\_transactions** Diagram

<table><thead><tr><td>Parent Table</td><td>Parent field</td></tr></thead><tbody><tr><td><a href=#4361851d-09df-4aa8-889f-74e8bccdb9a7>refferals</a></td><td><a href=#2b69fdd4-083b-4754-adeb-0ea66b3ac90b>_id</a></td></tr></tbody></table>

![Hackolade image](Modulo-social/image81.png?raw=true)![Hackolade image](Modulo-social/image82.png?raw=true)

<table><thead><tr><td>Child Table</td><td>Child field</td></tr></thead><tbody><tr><td><a href=#0a36268a-2d4b-4f7f-96e9-a34870e54fac>refferals_monthly_transactions</a></td><td><a href=#5a012fe7-4840-441d-abcd-41a8ac1f0499>refferal_id</a></td></tr></tbody></table>

#### 3.30.2 **refferals-monthly\_transactions** Properties

<table><thead><tr><td>Property</td><td>Value</td></tr></thead><tbody><tr><td>Name</td><td>refferals-monthly_transactions</td></tr><tr><td>Description</td><td></td></tr><tr><td>Parent Collection</td><td><a href=#4361851d-09df-4aa8-889f-74e8bccdb9a7>refferals</a></td></tr><tr><td>Parent field</td><td><a href=#2b69fdd4-083b-4754-adeb-0ea66b3ac90b>_id</a></td></tr><tr><td>Parent Cardinality</td><td>1</td></tr><tr><td>Child Collection</td><td><a href=#0a36268a-2d4b-4f7f-96e9-a34870e54fac>refferals_monthly_transactions</a></td></tr><tr><td>Child field</td><td><a href=#5a012fe7-4840-441d-abcd-41a8ac1f0499>refferal_id</a></td></tr><tr><td>Child Cardinality</td><td>1</td></tr><tr><td>Comments</td><td></td></tr></tbody></table>

