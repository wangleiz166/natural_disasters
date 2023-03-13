## **模块分为:**

## 所有的前端页面
不要用JS-作业要求
根据自己负责的模块修改

## 数据录入模块
要求数据录入到数据库要完整精确 
prase_csv.py : csv精简数据（3000-7000条），设计数据库，设计表结构， 数据录入脚本

## 仪表盘模块
打算作为首页，要做的好看一些，各种top10,统计图 
disaster_dashboard： 仪表盘大屏显示，柱状图，饼图，地图，报警 等统计数据

## Ucenter模块
不能用js操作cookie的方式，把用户登录信息存在数据库里。 
disaster_authen ：1.用户认证 2.登录 3.注册等。

## 接入open ai模块
disaster_chat ：使用openai服务，进行定制化服务（需求待定）。

## 列表页模块
功能较多 需要展示数据，做分页，做搜索，逻辑删除等
disaster_list ：数据管理：列表页+分页+搜索

## 编辑模块
disaster_edit ：数据管理：联表查询+详情页显示+编辑

## 恢复删除模块
disaster_trash_list： 用于显示已删除的数据+恢复逻辑删除状态。



## CSV解释

## 1900_2021_DISASTERS.xlsx - emdat data.csv

这些字段包含了关于一个灾害事件的多种信息，下面是各个字段的解释：
这些字段中包含了大量有关灾害事件的信息，这些信息可以用来进行统计和分析，以便更好地理解和预测未来可能发生的自然和人为灾害。

| 字段名              | 描述                                       |
|-------------------|-------------------------------------------|
| Year              | 灾害事件发生的年份。                            |
| Seq               | 灾害事件在该年中的序号。                          |
| Glide             | 灾害事件的全球灾害和应急响应平台 (GLIDE) 编号。       |
| Disaster Group    | 灾害事件的大类别，包括 Natural、Technological 和 Complex。|
| Disaster Subgroup | 灾害事件的子类别，包括 Climatological、Geophysical、Hydrological、Meteorological 和 Biological。|
| Disaster Type     | 灾害事件的类型，例如 Flood、Drought、Earthquake、Epidemic 等。|
| Disaster Subtype  | 灾害事件的子类型，例如 Flash flood、Landslide、Heat wave、Influenza 等。|
| Disaster Subsubtype | 灾害事件的子子类型，例如 Tropical storm、Mudslide、Wildfire、Malaria 等。 |
| Event Name        | 灾害事件的名称或描述。                           |
| Country           | 灾害事件发生的国家或地区。                         |
| ISO               | 该国家或地区的 ISO 3166-1 alpha-3 代码。           |
| Region            | 该国家或地区所属的联合国统计分区。                     |
| Continent         | 该国家或地区所属的洲。                            |
| Location          | 灾害事件发生的具体位置。                          |
| Origin            | 灾害事件的起因或来源。                           |
| Associated Dis    | 与该灾害事件相关的其他灾害事件的 Glide 编号。          |
| Associated Dis2   | 与该灾害事件相关的另一个灾害事件的 Glide 编号。       |
| OFDA Response     | 是否有美国联邦紧急管理署 (OFDA) 参与应对该灾害事件。        |
| Appeal            | 联合国是否发布了为该灾害事件发起的人道主义援助呼吁。           |
| Declaration       | 联合国是否发布了为该灾害事件的官方声明。                |
| Aid Contribution  | 提供给该灾害事件的援助总金额。                       |
| Dis Mag Value     | 该灾害事件的规模或严重程度。                          |
| Dis Mag Scale     | 灾害事件规模或严重程度的计量标准。                       |
| Latitude          | 灾害事件发生地的纬度。                             |
| Longitude         | 灾害事件发生地的经度。                             |
| Local Time        | 灾害事件发生的当地时间。                           |
| River Basin       | 该灾害事件所在的河流流域。                          |
| Start Year        | 灾害事件开始的年份。                             |
| Start Month       | 灾害事件开始的月份。                             |
| Start Day         | 灾害事件开始的日期。 |
| End Year          | 灾害事件结束的年份。 |
| End Month         | 灾害事件结束的月份。 |
| End Day           | 灾害事件结束的日期。 |
| Total Deaths      | 该灾害事件导致的总死亡人数。 |
| No Injured        | 该灾害事件导致的受伤人数。 |
| No Affected       | 该灾害事件导致的受影响人数。 |
| No Homeless       | 该灾害事件导致的无家可归的人数。 |
| Total Affected    | 该灾害事件总共影响到的人数。 |
| Insured Damages ('000 US$) | 该灾害事件造成的已投保损失，单位为千美元。 |
| Total Damages ('000 US$)   | 该灾害事件总共造成的损失，单位为千美元。 |
| CPI               | 该灾害事件发生时的消费者物价指数 (CPI)。 |
| Adm Level         | 地理行政区划级别，例如国家、省、市、县等。 |
| Admin1 Code       | 一级行政区划的代码。 |
| Admin2 Code       | 二级行政区划的代码。 |
| Geo Locations     | 该灾害事件的地理位置信息。 |

## 1970-2021_DISASTERS.xlsx - emdat data.csv
这些字段是关于一次特定的灾害事件的详细信息，下面是各个字段的解释：
这些字段提供了关于一次灾害事件的非常详细的信息，这些信息可以用于监测和预测灾害事件的趋势，并帮助国家和国际组织及时采取行动来减轻灾害的影响。

| 字段名                          | 描述                                         |
| ------------------------------- | -------------------------------------------- |
| Dis No                          | 该灾害事件的唯一编号，通常由年份、序号和国家/地区的 ISO 3166-1 alpha-3 代码组成。 |
| Year                            | 灾害事件发生的年份。                         |
| Seq                             | 该年中该灾害事件的序号。                     |
| Glide                           | 该灾害事件的全球灾害和应急响应平台 (GLIDE) 编号。 |
| Disaster Group                  | 灾害事件的大类别，包括 Natural (自然灾害)、Technological (技术灾害) 和 Complex (复杂灾害)。 |
| Disaster Subgroup               | 灾害事件的子类别，包括 Climatological (气候灾害)、Geophysical (地质灾害)、Hydrological (水文灾害)、Meteorological (气象灾害) 和 Biological (生物灾害)。 |
| Disaster Type                   | 灾害事件的类型，例如 Flood、Drought、Earthquake、Epidemic 等。 |
| Disaster Subtype                | 灾害事件的子类型，例如 Flash flood、Landslide、Heat wave、Influenza 等。 |
| Disaster Subsubtype             | 灾害事件的子子类型，例如 Tropical storm、Mudslide、Wildfire、Malaria 等。 |
| Event Name                      | 灾害事件的名称或描述。                       |
| Country                         | 灾害事件发生的国家或地区。                   |
| ISO                             | 该国家或地区的 ISO 3166-1 alpha-3 代码。      |
| Region                          | 该国家或地区所属的联合国统计分区。             |
| Continent                       | 该国家或地区所属的洲。                       |
| Location                        | 灾害事件发生的具体位置。                     |
| Origin                          | 灾害事件的起因或来源。                       |
| Associated Dis                  | 与该灾害事件相关的其他灾害事件的 Glide 编号。 |
| Associated Dis2                 | 与该灾害事件相关的另一个灾害事件的 Glide 编号。 |
| OFDA Response                   | 是否有美国联邦紧急管理署 (OFDA) 参与应对该灾害事件。 |
| Appeal                          | 联合国是否发布了为该灾害事件发起的人道主义援助呼吁。 |
| Declaration                     | 联合国是否发布了为该灾害事件的官方声明。     |
| Aid Contribution                | 提供给该灾害事件的援助总金额。               |
| Dis Mag Value                   | 该灾害事件的规模或严重程度。                 |
| Dis Mag Scale                   | 灾害事件规模或严
| 字段                           | 描述                                   |
| ----------------------------- | -------------------------------------- |
| Latitude                      | 灾害事件发生地的纬度                 |
| Longitude                     | 灾害事件发生地的经度                 |
| Local Time                    | 灾害事件发生的当地时间               |
| River Basin                   | 该灾害事件所在的河流流域             |
| Start Year                    | 灾害事件开始的年份                   |
| Start Month                   | 灾害事件开始的月份                   |
| Start Day                     | 灾害事件开始的日期                   |
| End Year                      | 灾害事件结束的年份                   |
| End Month                     | 灾害事件结束的月份                   |
| End Day                       | 灾害事件结束的日期                   |
| Total Deaths                  | 该灾害事件导致的总死亡人数           |
| No Injured                    | 该灾害事件导致的受伤人数             |
| No Affected                   | 该灾害事件导致的受影响人数           |
| No Homeless                   | 该灾害事件导致的无家可归的人数       |
| Total Affected                | 该灾害事件总共影响到的人数           |
| Reconstruction Costs ('000 US$)| 灾后重建的总成本，单位为千美元     |
| Insured Damages ('000 US$)    | 该灾害事件造成的已投保损失，单位为千美元 |
| Total Damages ('000 US$)      | 该灾害事件总共造成的损失，单位为千美元 |
| CPI                           | 该灾害事件发生时的消费者物价指数     |
| Adm Level                     | 地理行政区划级别，例如国家、省、市、县等 |
| Admin1 Code                   | 一级行政区划的代码                     |
| Admin2 Code                   | 二级行政区划的代码                     |
| Geo Locations                 | 该灾害事件的地理位置信息             |
