# di-ept-json-lidar

This repo is a sample workspace to read an EPT JSON dataset from the [USGS 3DEP Lidar Point clouds published in a public Amazon S3 bucket](https://registry.opendata.aws/usgs-lidar/), read the Lidar data. Contributions to enhance the FME workspace are welcome. Creating raster, DEMs, 3D and feature outputs from the LAS datasets would be desirable enhancements to this worksapce.<br/>

Credits to Michael Grieco of AllPointsGIS for  this user suggested workflow. Michael intends to instruct his students in getting public data Las data from the USGS and create raster data from them.

## Features

Completed
* Read the EPT JSON <br/>
* Read the Las dataset, split and create data derivatives from the Lidar point cloud.<br/>

Being considered:
* Share as web tool<br/>

## Warning: 
1. FMW or Workbench workspaces are readable in text format in Git. Please do not make any edits on the fmw files unless you absolutely know what you are doing when making changes.<br/>
2. Not all workspaces or workspace templates are expected to run after being downloaded. Web Connections or database connections must be added or reconfigured in the Workbench Tools Options dialog prior to running these samples.<br/>

## Instructions

Disclaimer: This sample workspace is a functional workspace that require minimum configuration.
1. Open the [USGS Entwine viewer](https://usgs.entwine.io/) and identify your project.
2. Copy the URL of your identified project from the viewer removing the "/ept.json" from the URL path. The sample workspace URL https://s3.us-west-2.amazonaws.com/usgs-lidar-public/ARRA-TX_CalhounCo_2010 wiil be used as the Dataset parameter in the FeatureReader transformer of the workspace.<br/>
![image](https://user-images.githubusercontent.com/87094963/139481331-df8ccd78-7cc2-413e-a7dc-da7986709002.png)

3. Download the repo using Github Desktop or from your browser go to the [fmw file](https://github.com/salvaleonrp/di-ept-json-lidar/blob/main/EptLasToRaster28Incomplete.fmw) and download by right clicking on RAW as shown from a Google browser below.<br/>

![image](https://user-images.githubusercontent.com/87094963/139471922-a740933d-ef61-4419-8505-a744a3ba70c8.png)
 
4. Open the Workspace using Data Interoperability or FME Desktop.
5. On the FeatureReader transformer, leave the configured parameters or change it with your identified URL, following the screenshot below the steps configure the ept.json feature type. <br/>
 Step a. <br/>
![image](https://user-images.githubusercontent.com/87094963/139481888-75747c69-c981-4377-bb8f-4faf53c9eb86.png)
 Step b. <br/>
![image](https://user-images.githubusercontent.com/87094963/139482183-df10c0ea-0cba-4b78-97a7-31730b4f9e11.png)


6. Configure the writer feature type with your destination folder
7. Run translation

## Reader and Writer formats and Transformers used
EPT reader (started with ArcGIS Pro 2.7 & FME 2020)<br/>
PointCloudSplitter<br/>
SurfaceModeller<br/>

## Workspace Requirements
* ArcGIS Pro 2.8 or  higher
* Data Interoperability for ArcGIS Pro 2.9 or higher

For Sharing as web tool solution later
* ArcGIS Server 10.9.1
* Data Interoperability for Server 10.9.1 or higher


## Product information
ArcGIS Data Interoperability is an OEM version of Safe Software's FME Desktop. DI is an extension to ArcGIS Pro that requires a separate install and license. Similar to FME Desktop, DI for Pro will operate without launching ArcGIS Pro. Spatial ETL tool is a feature in ArcGIS Pro that incoporates DI workspaces into the Pro Project. Spatial ETL tools can be shared as web tools in ArcGis Enterprise or published as a GP service in ArcGis Server with the DI Server extension. 


## Resources

Below are links to essential references for this repo.<br/>
[USGS-Lidar repo](https://github.com/hobu/usgs-lidar/)<br/>
[USGS Entwine viewer](https://usgs.entwine.io/) - link to EPT, Cesium and Potree URLS to the data<br/>
[Open Topography viewer](https://portal.opentopography.org/datasets) - Topo dataset derivatives<br/>
[EPT format resource](https://entwine.io/entwine-point-tile.html)<br/>

## Issues

Find a bug or want to request a new feature?  Please let us know by submitting an issue.

## Contributing

Esri welcomes contributions from anyone and everyone. Please see our [guidelines for contributing](https://github.com/esri/contributing).

Add your contributions to this repo [URL](https://github.com/awslabs/open-data-registry/blob/main/datasets/usgs-lidar.yaml)

## USGS Data Attribution & License
US Government Public Domain https://www.usgs.gov/faqs/what-are-terms-uselicensing-map-services-and-data-national-map

## Licensing
Copyright 2021 Esri

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

A copy of the license is available in the repository's [license.txt](https://github.com/salvaleonrp/di-data-driven-electric-utility-export-subnetwork/blob/main/license.txt) file.

[](Esri Tags: Data Interoperability for ArcGIS Pro)
[](Esri Tags: Utility Network)
