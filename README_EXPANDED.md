# di-ept-json-lidar-expanded

This repo is a sample workspace to list and download the EPT JSON dataset and Lidar data from the [USGS 3DEP Lidar Point clouds published in a public Amazon S3 bucket](https://registry.opendata.aws/usgs-lidar/).<br/>

Credits

## Features
Completed
* Read directly from the USGS public bucket <br/>
* List all projects from the bucket<br/>
* Filter project list (Optional - by typing a state abbreviation in user paramter) <br/>   
* Read the EPT JSON Lidar dataset<br/>
* Create the coverage of each project using the boundary.json file<br/>
* Read, split and create data derivatives from the Lidar point cloud.<br/>
Being considered:
* Add a State geometry filter parameter.<br/>
* Share as web tool<br/>

## Warning: 
1. FMW or Workbench workspaces are readable in text format in Git. Please do not make any edits on the fmw files unless you absolutely know what you are doing when making changes.
2. Not all workspaces or workspace templates are expected to run after being downloaded. Web Connections or database connections must be added or reconfigured in the Workbench Tools Options dialog prior to running these samples.

## Instructions

1. Download the workspace or fork this repo.
2. Open the Workspace using Data INteroperability or FME Desktop.
3. Configure your parameters and map your writer feature type to your destination file geodatabase
4. Run translation

## Reader and Writer formats and Transformers used
Amazon S3 Bucket reader
EPT reader
JSONFragmenter
FILEGDB writer

## Requirements

* ArcGIS Pro 2.9 or  higher
* Data Interoperability for ArcGIS Pro 2.9 or higher

For Sharing as web tool solution
* ArcGIS Server 10.9.1
* Data Interoperability for Server 10.9.1 or higher


## Product information
ArcGIS Data Interoperability is an OEM version of Safe Software's FME Desktop. DI is an extension to ArcGIS Pro that requires a separate install and license. Similar to FME Desktop, DI for Pro will operate without launching ArcGIS Pro. Spatial ETL tool is a feature in ArcGIS Pro that incoporates DI workspaces into the Pro Project. Spatial ETL tools can be shared as web tools in ArcGis Enterprise or published as a GP service in ArcGis Server with the DI Server extension. 


## Resources

Below are links to essential references for this repo.
[USGS-Lidar repo](https://github.com/hobu/usgs-lidar/)
[USGS Entwine viewer](https://usgs.entwine.io/) - link to EPT, Cesium and Potree URLS to the data
[Open Topography viewer](https://portal.opentopography.org/datasets) - Topo dataset derivatives
[EPT format resource](https://entwine.io/entwine-point-tile.html)

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
