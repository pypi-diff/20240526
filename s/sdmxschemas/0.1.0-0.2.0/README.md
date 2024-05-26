# Comparing `tmp/sdmxschemas-0.1.0.tar.gz` & `tmp/sdmxschemas-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdmxschemas-0.1.0.tar", max compression
+gzip compressed data, was "sdmxschemas-0.2.0.tar", max compression
```

## Comparing `sdmxschemas-0.1.0.tar` & `sdmxschemas-0.2.0.tar`

### file list

```diff
@@ -1,120 +1,121 @@
--rw-r--r--   0        0        0    11357 2024-05-26 09:08:04.870032 sdmxschemas-0.1.0/LICENSE
--rw-r--r--   0        0        0      318 2024-05-26 09:08:04.870032 sdmxschemas-0.1.0/README.md
--rw-r--r--   0        0        0      766 2024-05-26 09:08:04.870032 sdmxschemas-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1372 2024-05-26 09:08:04.870032 sdmxschemas-0.1.0/sdmxschemas/__init__.py
--rw-r--r--   0        0        0    35039 2024-05-26 09:08:04.870032 sdmxschemas-0.1.0/sdmxschemas/json/sdmx10/sdmx-json-data-schema.json
--rw-r--r--   0        0        0    35295 2024-05-26 09:08:04.870032 sdmxschemas-0.1.0/sdmxschemas/json/sdmx10/sdmx-json-metadata-schema.json
--rw-r--r--   0        0        0   174422 2024-05-26 09:08:04.870032 sdmxschemas-0.1.0/sdmxschemas/json/sdmx10/sdmx-json-structure-schema.json
--rw-r--r--   0        0        0    37751 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/json/sdmx20/sdmx-json-data-schema.json
--rw-r--r--   0        0        0    38825 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/json/sdmx20/sdmx-json-metadata-schema.json
--rw-r--r--   0        0        0   253644 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/json/sdmx20/sdmx-json-structure-schema.json
--rw-r--r--   0        0        0     5289 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXCommon.xsd
--rw-r--r--   0        0        0     2601 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXCompactData.xsd
--rw-r--r--   0        0        0     2956 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXCrossSectionalData.xsd
--rw-r--r--   0        0        0     7989 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXGenericData.xsd
--rw-r--r--   0        0        0    14649 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXMessage.xsd
--rw-r--r--   0        0        0    12955 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXQuery.xsd
--rw-r--r--   0        0        0    26604 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXStructure.xsd
--rw-r--r--   0        0        0     3377 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXUtilityData.xsd
--rw-r--r--   0        0        0     2700 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/xml.xsd
--rw-r--r--   0        0        0    14115 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXCommon.xsd
--rw-r--r--   0        0        0     4448 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXCompactData.xsd
--rw-r--r--   0        0        0     4553 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXCrossSectionalData.xsd
--rw-r--r--   0        0        0    10266 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXGenericData.xsd
--rw-r--r--   0        0        0    16212 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXGenericMetadata.xsd
--rw-r--r--   0        0        0    19904 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXMessage.xsd
--rw-r--r--   0        0        0     3626 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXMetadataReport.xsd
--rw-r--r--   0        0        0    26969 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXQuery.xsd
--rw-r--r--   0        0        0    56497 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXRegistry.xsd
--rw-r--r--   0        0        0   138319 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXStructure.xsd
--rw-r--r--   0        0        0     5228 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXUtilityData.xsd
--rw-r--r--   0        0        0     2700 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/xml.xsd
--rw-r--r--   0        0        0    97090 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXCommon.xsd
--rw-r--r--   0        0        0   235092 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXCommonReferences.xsd
--rw-r--r--   0        0        0      710 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXDataGeneric.xsd
--rw-r--r--   0        0        0    16286 2024-05-26 09:08:04.874032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXDataGenericBase.xsd
--rw-r--r--   0        0        0     6748 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXDataGenericTimeSeries.xsd
--rw-r--r--   0        0        0     1123 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXDataStructureSpecific.xsd
--rw-r--r--   0        0        0    28227 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXDataStructureSpecificBase.xsd
--rw-r--r--   0        0        0     6305 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXDataStructureSpecificTimeSeries.xsd
--rw-r--r--   0        0        0    74849 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXMessage.xsd
--rw-r--r--   0        0        0     3167 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXMessageFooter.xsd
--rw-r--r--   0        0        0    10799 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXMetadataGeneric.xsd
--rw-r--r--   0        0        0    20430 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXMetadataStructureSpecific.xsd
--rw-r--r--   0        0        0     2222 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQuery.xsd
--rw-r--r--   0        0        0    38832 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryBase.xsd
--rw-r--r--   0        0        0     5506 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryCategorisation.xsd
--rw-r--r--   0        0        0     5029 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryCategory.xsd
--rw-r--r--   0        0        0     4630 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryCodelist.xsd
--rw-r--r--   0        0        0     5630 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryConcept.xsd
--rw-r--r--   0        0        0     9777 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryConstraint.xsd
--rw-r--r--   0        0        0    28572 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryData.xsd
--rw-r--r--   0        0        0    16592 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryDataStructure.xsd
--rw-r--r--   0        0        0     3608 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryDataflow.xsd
--rw-r--r--   0        0        0     4562 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryHierarchicalCodelist.xsd
--rw-r--r--   0        0        0    21067 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryMetadata.xsd
--rw-r--r--   0        0        0    12632 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryMetadataStructure.xsd
--rw-r--r--   0        0        0     3745 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryMetadataflow.xsd
--rw-r--r--   0        0        0     6467 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryOrganisation.xsd
--rw-r--r--   0        0        0     7752 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryProcess.xsd
--rw-r--r--   0        0        0     4862 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryProvisionAgreement.xsd
--rw-r--r--   0        0        0     6620 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryReportingTaxonomy.xsd
--rw-r--r--   0        0        0     4531 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQuerySchema.xsd
--rw-r--r--   0        0        0     8680 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryStructureSet.xsd
--rw-r--r--   0        0        0     3258 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryStructures.xsd
--rw-r--r--   0        0        0    28272 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryTransformation.xsd
--rw-r--r--   0        0        0     1070 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXRegistry.xsd
--rw-r--r--   0        0        0    12289 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXRegistryBase.xsd
--rw-r--r--   0        0        0    13830 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXRegistryRegistration.xsd
--rw-r--r--   0        0        0     7491 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXRegistryStructure.xsd
--rw-r--r--   0        0        0    44425 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXRegistrySubscription.xsd
--rw-r--r--   0        0        0    38110 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructure.xsd
--rw-r--r--   0        0        0    33862 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureBase.xsd
--rw-r--r--   0        0        0     1848 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureCategorisation.xsd
--rw-r--r--   0        0        0     3541 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureCategory.xsd
--rw-r--r--   0        0        0     4215 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureCodelist.xsd
--rw-r--r--   0        0        0     6708 2024-05-26 09:08:04.878032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureConcept.xsd
--rw-r--r--   0        0        0    22858 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureConstraint.xsd
--rw-r--r--   0        0        0    38217 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureDataStructure.xsd
--rw-r--r--   0        0        0     1925 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureDataflow.xsd
--rw-r--r--   0        0        0    15490 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureHierarchicalCodelist.xsd
--rw-r--r--   0        0        0    27161 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureMetadataStructure.xsd
--rw-r--r--   0        0        0     1990 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureMetadataflow.xsd
--rw-r--r--   0        0        0    16142 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureOrganisation.xsd
--rw-r--r--   0        0        0     9413 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureProcess.xsd
--rw-r--r--   0        0        0     2244 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureProvisionAgreement.xsd
--rw-r--r--   0        0        0     4459 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureReportingTaxonomy.xsd
--rw-r--r--   0        0        0    28667 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureStructureSet.xsd
--rw-r--r--   0        0        0    30974 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureTransformation.xsd
--rw-r--r--   0        0        0     2700 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/xml.xsd
--rw-r--r--   0        0        0    72649 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXCommon.xsd
--rw-r--r--   0        0        0    65819 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXCommonReferences.xsd
--rw-r--r--   0        0        0    26656 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXDataStructureSpecific.xsd
--rw-r--r--   0        0        0    29580 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXMessage.xsd
--rw-r--r--   0        0        0     3040 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXMessageFooter.xsd
--rw-r--r--   0        0        0     6649 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXMetadataGeneric.xsd
--rw-r--r--   0        0        0     1070 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXRegistry.xsd
--rw-r--r--   0        0        0    12262 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXRegistryBase.xsd
--rw-r--r--   0        0        0    13530 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXRegistryRegistration.xsd
--rw-r--r--   0        0        0     7498 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXRegistryStructure.xsd
--rw-r--r--   0        0        0    44425 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXRegistrySubscription.xsd
--rw-r--r--   0        0        0    56553 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructure.xsd
--rw-r--r--   0        0        0    29093 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureBase.xsd
--rw-r--r--   0        0        0     2641 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureCategorisation.xsd
--rw-r--r--   0        0        0     3845 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureCategory.xsd
--rw-r--r--   0        0        0    18189 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureCodelist.xsd
--rw-r--r--   0        0        0     6994 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureConcept.xsd
--rw-r--r--   0        0        0    46306 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureConstraint.xsd
--rw-r--r--   0        0        0    38634 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureDataStructure.xsd
--rw-r--r--   0        0        0     2065 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureDataflow.xsd
--rw-r--r--   0        0        0    13241 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureHierarchicalCodelist.xsd
--rw-r--r--   0        0        0    10038 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureMetadataStructure.xsd
--rw-r--r--   0        0        0     3015 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureMetadataflow.xsd
--rw-r--r--   0        0        0    19451 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureOrganisation.xsd
--rw-r--r--   0        0        0    10950 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureProcess.xsd
--rw-r--r--   0        0        0     5571 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureProvisionAgreement.xsd
--rw-r--r--   0        0        0     4762 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureReportingTaxonomy.xsd
--rw-r--r--   0        0        0    22794 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureStructureMappings.xsd
--rw-r--r--   0        0        0    36325 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureTransformation.xsd
--rw-r--r--   0        0        0     2700 2024-05-26 09:08:04.882032 sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/xml.xsd
--rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 sdmxschemas-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-26 09:23:48.300163 sdmxschemas-0.2.0/LICENSE
+-rw-r--r--   0        0        0      339 2024-05-26 09:23:48.300163 sdmxschemas-0.2.0/README.md
+-rw-r--r--   0        0        0      766 2024-05-26 09:23:48.300163 sdmxschemas-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1468 2024-05-26 09:23:48.300163 sdmxschemas-0.2.0/sdmxschemas/__init__.py
+-rw-r--r--   0        0        0    35039 2024-05-26 09:23:48.300163 sdmxschemas-0.2.0/sdmxschemas/json/sdmx10/sdmx-json-data-schema.json
+-rw-r--r--   0        0        0    35295 2024-05-26 09:23:48.300163 sdmxschemas-0.2.0/sdmxschemas/json/sdmx10/sdmx-json-metadata-schema.json
+-rw-r--r--   0        0        0   174422 2024-05-26 09:23:48.300163 sdmxschemas-0.2.0/sdmxschemas/json/sdmx10/sdmx-json-structure-schema.json
+-rw-r--r--   0        0        0    37751 2024-05-26 09:23:48.300163 sdmxschemas-0.2.0/sdmxschemas/json/sdmx20/sdmx-json-data-schema.json
+-rw-r--r--   0        0        0    38825 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/json/sdmx20/sdmx-json-metadata-schema.json
+-rw-r--r--   0        0        0   253644 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/json/sdmx20/sdmx-json-structure-schema.json
+-rw-r--r--   0        0        0        0 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/py.typed
+-rw-r--r--   0        0        0     5289 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXCommon.xsd
+-rw-r--r--   0        0        0     2601 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXCompactData.xsd
+-rw-r--r--   0        0        0     2956 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXCrossSectionalData.xsd
+-rw-r--r--   0        0        0     7989 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXGenericData.xsd
+-rw-r--r--   0        0        0    14649 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXMessage.xsd
+-rw-r--r--   0        0        0    12955 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXQuery.xsd
+-rw-r--r--   0        0        0    26604 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXStructure.xsd
+-rw-r--r--   0        0        0     3377 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXUtilityData.xsd
+-rw-r--r--   0        0        0     2700 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/xml.xsd
+-rw-r--r--   0        0        0    14115 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXCommon.xsd
+-rw-r--r--   0        0        0     4448 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXCompactData.xsd
+-rw-r--r--   0        0        0     4553 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXCrossSectionalData.xsd
+-rw-r--r--   0        0        0    10266 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXGenericData.xsd
+-rw-r--r--   0        0        0    16212 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXGenericMetadata.xsd
+-rw-r--r--   0        0        0    19904 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXMessage.xsd
+-rw-r--r--   0        0        0     3626 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXMetadataReport.xsd
+-rw-r--r--   0        0        0    26969 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXQuery.xsd
+-rw-r--r--   0        0        0    56497 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXRegistry.xsd
+-rw-r--r--   0        0        0   138319 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXStructure.xsd
+-rw-r--r--   0        0        0     5228 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXUtilityData.xsd
+-rw-r--r--   0        0        0     2700 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/xml.xsd
+-rw-r--r--   0        0        0    97090 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXCommon.xsd
+-rw-r--r--   0        0        0   235092 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXCommonReferences.xsd
+-rw-r--r--   0        0        0      710 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXDataGeneric.xsd
+-rw-r--r--   0        0        0    16286 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXDataGenericBase.xsd
+-rw-r--r--   0        0        0     6748 2024-05-26 09:23:48.304163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXDataGenericTimeSeries.xsd
+-rw-r--r--   0        0        0     1123 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXDataStructureSpecific.xsd
+-rw-r--r--   0        0        0    28227 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXDataStructureSpecificBase.xsd
+-rw-r--r--   0        0        0     6305 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXDataStructureSpecificTimeSeries.xsd
+-rw-r--r--   0        0        0    74849 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXMessage.xsd
+-rw-r--r--   0        0        0     3167 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXMessageFooter.xsd
+-rw-r--r--   0        0        0    10799 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXMetadataGeneric.xsd
+-rw-r--r--   0        0        0    20430 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXMetadataStructureSpecific.xsd
+-rw-r--r--   0        0        0     2222 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQuery.xsd
+-rw-r--r--   0        0        0    38832 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryBase.xsd
+-rw-r--r--   0        0        0     5506 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryCategorisation.xsd
+-rw-r--r--   0        0        0     5029 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryCategory.xsd
+-rw-r--r--   0        0        0     4630 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryCodelist.xsd
+-rw-r--r--   0        0        0     5630 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryConcept.xsd
+-rw-r--r--   0        0        0     9777 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryConstraint.xsd
+-rw-r--r--   0        0        0    28572 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryData.xsd
+-rw-r--r--   0        0        0    16592 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryDataStructure.xsd
+-rw-r--r--   0        0        0     3608 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryDataflow.xsd
+-rw-r--r--   0        0        0     4562 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryHierarchicalCodelist.xsd
+-rw-r--r--   0        0        0    21067 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryMetadata.xsd
+-rw-r--r--   0        0        0    12632 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryMetadataStructure.xsd
+-rw-r--r--   0        0        0     3745 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryMetadataflow.xsd
+-rw-r--r--   0        0        0     6467 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryOrganisation.xsd
+-rw-r--r--   0        0        0     7752 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryProcess.xsd
+-rw-r--r--   0        0        0     4862 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryProvisionAgreement.xsd
+-rw-r--r--   0        0        0     6620 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryReportingTaxonomy.xsd
+-rw-r--r--   0        0        0     4531 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQuerySchema.xsd
+-rw-r--r--   0        0        0     8680 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryStructureSet.xsd
+-rw-r--r--   0        0        0     3258 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryStructures.xsd
+-rw-r--r--   0        0        0    28272 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryTransformation.xsd
+-rw-r--r--   0        0        0     1070 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXRegistry.xsd
+-rw-r--r--   0        0        0    12289 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXRegistryBase.xsd
+-rw-r--r--   0        0        0    13830 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXRegistryRegistration.xsd
+-rw-r--r--   0        0        0     7491 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXRegistryStructure.xsd
+-rw-r--r--   0        0        0    44425 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXRegistrySubscription.xsd
+-rw-r--r--   0        0        0    38110 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructure.xsd
+-rw-r--r--   0        0        0    33862 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureBase.xsd
+-rw-r--r--   0        0        0     1848 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureCategorisation.xsd
+-rw-r--r--   0        0        0     3541 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureCategory.xsd
+-rw-r--r--   0        0        0     4215 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureCodelist.xsd
+-rw-r--r--   0        0        0     6708 2024-05-26 09:23:48.308163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureConcept.xsd
+-rw-r--r--   0        0        0    22858 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureConstraint.xsd
+-rw-r--r--   0        0        0    38217 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureDataStructure.xsd
+-rw-r--r--   0        0        0     1925 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureDataflow.xsd
+-rw-r--r--   0        0        0    15490 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureHierarchicalCodelist.xsd
+-rw-r--r--   0        0        0    27161 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureMetadataStructure.xsd
+-rw-r--r--   0        0        0     1990 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureMetadataflow.xsd
+-rw-r--r--   0        0        0    16142 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureOrganisation.xsd
+-rw-r--r--   0        0        0     9413 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureProcess.xsd
+-rw-r--r--   0        0        0     2244 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureProvisionAgreement.xsd
+-rw-r--r--   0        0        0     4459 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureReportingTaxonomy.xsd
+-rw-r--r--   0        0        0    28667 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureStructureSet.xsd
+-rw-r--r--   0        0        0    30974 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureTransformation.xsd
+-rw-r--r--   0        0        0     2700 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/xml.xsd
+-rw-r--r--   0        0        0    72649 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXCommon.xsd
+-rw-r--r--   0        0        0    65819 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXCommonReferences.xsd
+-rw-r--r--   0        0        0    26656 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXDataStructureSpecific.xsd
+-rw-r--r--   0        0        0    29580 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXMessage.xsd
+-rw-r--r--   0        0        0     3040 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXMessageFooter.xsd
+-rw-r--r--   0        0        0     6649 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXMetadataGeneric.xsd
+-rw-r--r--   0        0        0     1070 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXRegistry.xsd
+-rw-r--r--   0        0        0    12262 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXRegistryBase.xsd
+-rw-r--r--   0        0        0    13530 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXRegistryRegistration.xsd
+-rw-r--r--   0        0        0     7498 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXRegistryStructure.xsd
+-rw-r--r--   0        0        0    44425 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXRegistrySubscription.xsd
+-rw-r--r--   0        0        0    56553 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructure.xsd
+-rw-r--r--   0        0        0    29093 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureBase.xsd
+-rw-r--r--   0        0        0     2641 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureCategorisation.xsd
+-rw-r--r--   0        0        0     3845 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureCategory.xsd
+-rw-r--r--   0        0        0    18189 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureCodelist.xsd
+-rw-r--r--   0        0        0     6994 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureConcept.xsd
+-rw-r--r--   0        0        0    46306 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureConstraint.xsd
+-rw-r--r--   0        0        0    38634 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureDataStructure.xsd
+-rw-r--r--   0        0        0     2065 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureDataflow.xsd
+-rw-r--r--   0        0        0    13241 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureHierarchicalCodelist.xsd
+-rw-r--r--   0        0        0    10038 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureMetadataStructure.xsd
+-rw-r--r--   0        0        0     3015 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureMetadataflow.xsd
+-rw-r--r--   0        0        0    19451 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureOrganisation.xsd
+-rw-r--r--   0        0        0    10950 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureProcess.xsd
+-rw-r--r--   0        0        0     5571 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureProvisionAgreement.xsd
+-rw-r--r--   0        0        0     4762 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureReportingTaxonomy.xsd
+-rw-r--r--   0        0        0    22794 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureStructureMappings.xsd
+-rw-r--r--   0        0        0    36325 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureTransformation.xsd
+-rw-r--r--   0        0        0     2700 2024-05-26 09:23:48.312163 sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/xml.xsd
+-rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 sdmxschemas-0.2.0/PKG-INFO
```

### Comparing `sdmxschemas-0.1.0/LICENSE` & `sdmxschemas-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/pyproject.toml` & `sdmxschemas-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdmxschemas"
-version = "0.1.0"
+version = "0.2.0"
 description = "SDMX schemas for Python"
 authors = ["Francisco Javier Hernandez del Caño <javier.hernandez@meaningfuldata.eu>"]
 readme = "README.md"
 packages = [
     { include = "sdmxschemas", from = "."}
 ]
 keywords = ["sdmx"]
```

### Comparing `sdmxschemas-0.1.0/sdmxschemas/json/sdmx10/sdmx-json-data-schema.json` & `sdmxschemas-0.2.0/sdmxschemas/json/sdmx10/sdmx-json-data-schema.json`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/json/sdmx10/sdmx-json-metadata-schema.json` & `sdmxschemas-0.2.0/sdmxschemas/json/sdmx10/sdmx-json-metadata-schema.json`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/json/sdmx10/sdmx-json-structure-schema.json` & `sdmxschemas-0.2.0/sdmxschemas/json/sdmx10/sdmx-json-structure-schema.json`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/json/sdmx20/sdmx-json-data-schema.json` & `sdmxschemas-0.2.0/sdmxschemas/json/sdmx20/sdmx-json-data-schema.json`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/json/sdmx20/sdmx-json-metadata-schema.json` & `sdmxschemas-0.2.0/sdmxschemas/json/sdmx20/sdmx-json-metadata-schema.json`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/json/sdmx20/sdmx-json-structure-schema.json` & `sdmxschemas-0.2.0/sdmxschemas/json/sdmx20/sdmx-json-structure-schema.json`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXCommon.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXCommon.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXCompactData.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXCompactData.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXCrossSectionalData.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXCrossSectionalData.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXGenericData.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXGenericData.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXMessage.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXMessage.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXQuery.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXQuery.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXStructure.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/SDMXUtilityData.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/SDMXUtilityData.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx10/xml.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx10/xml.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXCommon.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXCommon.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXCompactData.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXCompactData.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXCrossSectionalData.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXCrossSectionalData.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXGenericData.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXGenericData.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXGenericMetadata.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXGenericMetadata.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXMessage.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXMessage.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXMetadataReport.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXMetadataReport.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXQuery.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXQuery.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXRegistry.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXRegistry.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXStructure.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/SDMXUtilityData.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/SDMXUtilityData.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx20/xml.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx20/xml.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXCommon.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXCommon.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXCommonReferences.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXCommonReferences.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXDataGeneric.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXDataGeneric.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXDataGenericBase.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXDataGenericBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXDataGenericTimeSeries.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXDataGenericTimeSeries.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXDataStructureSpecific.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXDataStructureSpecific.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXDataStructureSpecificBase.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXDataStructureSpecificBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXDataStructureSpecificTimeSeries.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXDataStructureSpecificTimeSeries.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXMessage.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXMessage.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXMessageFooter.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXMessageFooter.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXMetadataGeneric.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXMetadataGeneric.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXMetadataStructureSpecific.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXMetadataStructureSpecific.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQuery.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQuery.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryBase.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryCategorisation.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryCategorisation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryCategory.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryCategory.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryCodelist.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryCodelist.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryConcept.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryConcept.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryConstraint.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryConstraint.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryData.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryData.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryDataStructure.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryDataStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryDataflow.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryDataflow.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryHierarchicalCodelist.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryHierarchicalCodelist.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryMetadata.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryMetadata.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryMetadataStructure.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryMetadataStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryMetadataflow.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryMetadataflow.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryOrganisation.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryOrganisation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryProcess.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryProcess.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryProvisionAgreement.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryProvisionAgreement.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryReportingTaxonomy.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryReportingTaxonomy.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQuerySchema.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQuerySchema.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryStructureSet.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryStructureSet.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryStructures.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryStructures.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXQueryTransformation.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXQueryTransformation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXRegistry.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXRegistry.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXRegistryBase.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXRegistryBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXRegistryRegistration.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXRegistryRegistration.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXRegistryStructure.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXRegistryStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXRegistrySubscription.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXRegistrySubscription.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructure.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureBase.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureCategorisation.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureCategorisation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureCategory.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureCategory.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureCodelist.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureCodelist.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureConcept.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureConcept.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureConstraint.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureConstraint.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureDataStructure.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureDataStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureDataflow.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureDataflow.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureHierarchicalCodelist.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureHierarchicalCodelist.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureMetadataStructure.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureMetadataStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureMetadataflow.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureMetadataflow.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureOrganisation.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureOrganisation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureProcess.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureProcess.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureProvisionAgreement.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureProvisionAgreement.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureReportingTaxonomy.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureReportingTaxonomy.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureStructureSet.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureStructureSet.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/SDMXStructureTransformation.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/SDMXStructureTransformation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx21/xml.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx21/xml.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXCommon.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXCommon.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXCommonReferences.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXCommonReferences.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXDataStructureSpecific.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXDataStructureSpecific.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXMessage.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXMessage.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXMessageFooter.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXMessageFooter.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXMetadataGeneric.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXMetadataGeneric.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXRegistry.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXRegistry.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXRegistryBase.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXRegistryBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXRegistryRegistration.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXRegistryRegistration.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXRegistryStructure.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXRegistryStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXRegistrySubscription.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXRegistrySubscription.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructure.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureBase.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureCategorisation.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureCategorisation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureCategory.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureCategory.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureCodelist.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureCodelist.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureConcept.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureConcept.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureConstraint.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureConstraint.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureDataStructure.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureDataStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureDataflow.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureDataflow.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureHierarchicalCodelist.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureHierarchicalCodelist.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureMetadataStructure.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureMetadataStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureMetadataflow.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureMetadataflow.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureOrganisation.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureOrganisation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureProcess.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureProcess.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureProvisionAgreement.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureProvisionAgreement.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureReportingTaxonomy.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureReportingTaxonomy.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureStructureMappings.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureStructureMappings.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/SDMXStructureTransformation.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/SDMXStructureTransformation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/sdmxschemas/xml/sdmx30/xml.xsd` & `sdmxschemas-0.2.0/sdmxschemas/xml/sdmx30/xml.xsd`

 * *Files identical despite different names*

### Comparing `sdmxschemas-0.1.0/PKG-INFO` & `sdmxschemas-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdmxschemas
-Version: 0.1.0
+Version: 0.2.0
 Summary: SDMX schemas for Python
 Home-page: https://github.com/Meaningful-Data/sdmx-schemas
 License: Apache-2.0
 Keywords: sdmx
 Author: Francisco Javier Hernandez del Caño
 Author-email: javier.hernandez@meaningfuldata.eu
 Requires-Python: >=3.8,<4.0
@@ -28,10 +28,11 @@
 The schemas are provided in the form of JSON Schema files and XSD files.
 
 Included are the following schemas:
 
 - SDMX-JSON 1.0 Schema
 - SDMX-JSON 2.0 Schema
 - SDMX-ML 1.0 Schema
+- SDMX-ML 2.0 Schema
 - SDMX-ML 2.1 Schema
 - SDMX-ML 3.0 Schema
```

