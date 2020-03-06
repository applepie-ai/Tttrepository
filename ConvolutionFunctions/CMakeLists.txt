cmake_minimum_required (VERSION 3.5)

project(CMSISNNConvolutions)

file(GLOB SRC "./*_*.c")

add_library(CMSISNNConvolutions STATIC ${SRC})

### Includes
target_include_directories(CMSISNNConvolutions PUBLIC "${NN}/Include")
target_include_directories(CMSISNNConvolutions PUBLIC "${DSP}/Include")
