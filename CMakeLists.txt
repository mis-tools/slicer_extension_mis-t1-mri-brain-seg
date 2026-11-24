cmake_minimum_required(VERSION 3.28.0...3.28.0 FATAL_ERROR)

project(MIS_T1_MRI_BRAIN_SEGMENTATION_EXTENSION)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://www.slicer.org/wiki/Documentation/Nightly/Extensions/MIS_T1_MRI_BRAIN_SEGMENTATION_EXTENSION")
set(EXTENSION_CONTRIBUTORS "MIS (MIS Org)")
set(EXTENSION_DESCRIPTION "Brain Segmentation of 3D T1 MRI Image")
set(EXTENSION_ICONURL "https://www.example.com/Slicer/Extensions/MIS_T1_MRI_BRAIN_SEGMENTATION_EXTENSION.png")
set(EXTENSION_SCREENSHOTURLS "https://www.example.com/Slicer/Extensions/MIS_T1_MRI_BRAIN_SEGMENTATION_EXTENSION/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(MIS_T1_MRI_BRAIN_SEGMENTATION_MODULE)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
