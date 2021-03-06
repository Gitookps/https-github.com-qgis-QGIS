#############################################################
# sources

SET(QGIS_ANALYSIS_SRCS
  interpolation/qgsgridfilewriter.cpp
  interpolation/qgsidwinterpolator.cpp
  interpolation/qgsinterpolator.cpp
  interpolation/qgstininterpolator.cpp
  interpolation/Bezier3D.cpp
  interpolation/CloughTocherInterpolator.cpp
  interpolation/DualEdgeTriangulation.cpp
  interpolation/HalfEdge.cpp
  interpolation/LinTriangleInterpolator.cpp
  interpolation/MathUtils.cpp
  interpolation/NormVecDecorator.cpp
  interpolation/ParametricLine.cpp
  interpolation/TriangleInterpolator.cpp
  interpolation/Triangulation.cpp
  interpolation/TriDecorator.cpp
  interpolation/Vector3D.cpp

  processing/qgsalgorithmaddincrementalfield.cpp
  processing/qgsalgorithmassignprojection.cpp
  processing/qgsalgorithmboundary.cpp
  processing/qgsalgorithmboundingbox.cpp
  processing/qgsalgorithmbuffer.cpp
  processing/qgsalgorithmcentroid.cpp
  processing/qgsalgorithmclip.cpp
  processing/qgsalgorithmconvexhull.cpp
  processing/qgsalgorithmdissolve.cpp
  processing/qgsalgorithmdropgeometry.cpp
  processing/qgsalgorithmdropmzvalues.cpp
  processing/qgsalgorithmextenttolayer.cpp
  processing/qgsalgorithmextractbyattribute.cpp
  processing/qgsalgorithmextractbyexpression.cpp
  processing/qgsalgorithmextractbyextent.cpp
  processing/qgsalgorithmextractbylocation.cpp
  processing/qgsalgorithmextractvertices.cpp
  processing/qgsalgorithmfiledownloader.cpp
  processing/qgsalgorithmfixgeometries.cpp
  processing/qgsalgorithmjoinbyattribute.cpp
  processing/qgsalgorithmjoinwithlines.cpp
  processing/qgsalgorithmimportphotos.cpp
  processing/qgsalgorithmlineintersection.cpp
  processing/qgsalgorithmloadlayer.cpp
  processing/qgsalgorithmmeancoordinates.cpp
  processing/qgsalgorithmmergelines.cpp
  processing/qgsalgorithmmergevector.cpp
  processing/qgsalgorithmminimumenclosingcircle.cpp
  processing/qgsalgorithmmultiparttosinglepart.cpp
  processing/qgsalgorithmmultiringconstantbuffer.cpp
  processing/qgsalgorithmorderbyexpression.cpp
  processing/qgsalgorithmorientedminimumboundingbox.cpp
  processing/qgsalgorithmpackage.cpp
  processing/qgsalgorithmpointonsurface.cpp
  processing/qgsalgorithmprojectpointcartesian.cpp
  processing/qgsalgorithmpromotetomultipart.cpp
  processing/qgsalgorithmrasterlayeruniquevalues.cpp
  processing/qgsalgorithmremoveduplicatevertices.cpp
  processing/qgsalgorithmremoveholes.cpp
  processing/qgsalgorithmremovenullgeometry.cpp
  processing/qgsalgorithmrenamelayer.cpp
  processing/qgsalgorithmrotate.cpp
  processing/qgsalgorithmsaveselectedfeatures.cpp
  processing/qgsalgorithmsegmentize.cpp
  processing/qgsalgorithmsimplify.cpp
  processing/qgsalgorithmsmooth.cpp
  processing/qgsalgorithmsnaptogrid.cpp
  processing/qgsalgorithmsplitwithlines.cpp
  processing/qgsalgorithmstringconcatenation.cpp
  processing/qgsalgorithmsubdivide.cpp
  processing/qgsalgorithmtransect.cpp
  processing/qgsalgorithmtransform.cpp
  processing/qgsalgorithmtranslate.cpp
  processing/qgsalgorithmuniquevalueindex.cpp

  processing/qgsnativealgorithms.cpp

  raster/qgsalignraster.cpp
  raster/qgsninecellfilter.cpp
  raster/qgsruggednessfilter.cpp
  raster/qgsderivativefilter.cpp
  raster/qgshillshadefilter.cpp
  raster/qgskde.cpp
  raster/qgsslopefilter.cpp
  raster/qgsaspectfilter.cpp
  raster/qgstotalcurvaturefilter.cpp
  raster/qgsrelief.cpp
  raster/qgsrastercalcnode.cpp
  raster/qgsrastercalculator.cpp
  raster/qgsrastermatrix.cpp
  vector/mersenne-twister.cpp
  vector/qgsgeometrysnapper.cpp
  vector/qgszonalstatistics.cpp

  network/qgsgraph.cpp
  network/qgsgraphbuilder.cpp
  network/qgsnetworkspeedstrategy.cpp
  network/qgsnetworkdistancestrategy.cpp
  network/qgsvectorlayerdirector.cpp
  network/qgsgraphanalyzer.cpp

  vector/geometry_checker/qgsfeaturepool.cpp
  vector/geometry_checker/qgsgeometrychecker.cpp
  vector/geometry_checker/qgsgeometryanglecheck.cpp
  vector/geometry_checker/qgsgeometryareacheck.cpp
  vector/geometry_checker/qgsgeometrycheck.cpp
  vector/geometry_checker/qgsgeometrychecker.cpp
  vector/geometry_checker/qgsgeometrycheckerutils.cpp
  vector/geometry_checker/qgsgeometrycontainedcheck.cpp
  vector/geometry_checker/qgsgeometrydanglecheck.cpp
  vector/geometry_checker/qgsgeometrydegeneratepolygoncheck.cpp
  vector/geometry_checker/qgsgeometryduplicatecheck.cpp
  vector/geometry_checker/qgsgeometryduplicatenodescheck.cpp
  vector/geometry_checker/qgsgeometrygapcheck.cpp
  vector/geometry_checker/qgsgeometryfollowboundariescheck.cpp
  vector/geometry_checker/qgsgeometryholecheck.cpp
  vector/geometry_checker/qgsgeometrylineintersectioncheck.cpp
  vector/geometry_checker/qgsgeometrylinelayerintersectioncheck.cpp
  vector/geometry_checker/qgsgeometrymultipartcheck.cpp
  vector/geometry_checker/qgsgeometryoverlapcheck.cpp
  vector/geometry_checker/qgsgeometrypointcoveredbylinecheck.cpp
  vector/geometry_checker/qgsgeometrypointinpolygoncheck.cpp
  vector/geometry_checker/qgsgeometrysegmentlengthcheck.cpp
  vector/geometry_checker/qgsgeometryselfcontactcheck.cpp
  vector/geometry_checker/qgsgeometryselfintersectioncheck.cpp
  vector/geometry_checker/qgsgeometrysliverpolygoncheck.cpp
  vector/geometry_checker/qgsgeometrytypecheck.cpp
)

SET(QGIS_ANALYSIS_MOC_HDRS
  processing/qgsnativealgorithms.h

  vector/qgsgeometrysnapper.h

  network/qgsgraphdirector.h
  network/qgsvectorlayerdirector.h

  processing/qgsalgorithmfiledownloader.h

  vector/geometry_checker/qgsfeaturepool.h
  vector/geometry_checker/qgsgeometrychecker.h
  vector/geometry_checker/qgsgeometryanglecheck.h
  vector/geometry_checker/qgsgeometryareacheck.h
  vector/geometry_checker/qgsgeometrychecker.h
  vector/geometry_checker/qgsgeometrycheck.h
  vector/geometry_checker/qgsgeometrycontainedcheck.h
  vector/geometry_checker/qgsgeometrydanglecheck.h
  vector/geometry_checker/qgsgeometrydegeneratepolygoncheck.h
  vector/geometry_checker/qgsgeometryduplicatecheck.h
  vector/geometry_checker/qgsgeometryduplicatenodescheck.h
  vector/geometry_checker/qgsgeometryfollowboundariescheck.h
  vector/geometry_checker/qgsgeometrygapcheck.h
  vector/geometry_checker/qgsgeometryholecheck.h
  vector/geometry_checker/qgsgeometrylineintersectioncheck.h
  vector/geometry_checker/qgsgeometrylinelayerintersectioncheck.h
  vector/geometry_checker/qgsgeometrymultipartcheck.h
  vector/geometry_checker/qgsgeometryoverlapcheck.h
  vector/geometry_checker/qgsgeometrypointcoveredbylinecheck.h
  vector/geometry_checker/qgsgeometrypointinpolygoncheck.h
  vector/geometry_checker/qgsgeometrysegmentlengthcheck.h
  vector/geometry_checker/qgsgeometryselfcontactcheck.h
  vector/geometry_checker/qgsgeometryselfintersectioncheck.h
  vector/geometry_checker/qgsgeometrysliverpolygoncheck.h
  vector/geometry_checker/qgsgeometrytypecheck.h
)

INCLUDE_DIRECTORIES(SYSTEM ${SPATIALITE_INCLUDE_DIR})
INCLUDE_DIRECTORIES(SYSTEM ${SQLITE3_INCLUDE_DIR})
INCLUDE_DIRECTORIES(BEFORE raster)

ADD_FLEX_FILES_PREFIX(QGIS_ANALYSIS_SRCS raster raster/qgsrastercalclexer.ll)

ADD_BISON_FILES_PREFIX(QGIS_ANALYSIS_SRCS raster raster/qgsrastercalcparser.yy)

IF(NOT MSVC)
  SET_SOURCE_FILES_PROPERTIES(
    ${CMAKE_BINARY_DIR}/src/analysis/qgsrastercalcparser.cpp
    PROPERTIES COMPILE_FLAGS "-w"
  )
ELSE(NOT MSVC)
  IF(PEDANTIC)
    # 4127 expression is constant
    # 4702 unreachable code
    SET_SOURCE_FILES_PROPERTIES(
      ${CMAKE_BINARY_DIR}/src/analysis/qgsrastercalcparser.cpp
      PROPERTIES COMPILE_FLAGS "-wd4127 -wd4702"
    )
  ENDIF(PEDANTIC)
ENDIF(NOT MSVC)

IF (CMAKE_CXX_COMPILER_ID MATCHES "Clang")
  SET_SOURCE_FILES_PROPERTIES(
    interpolation/qgstininterpolator.cpp
    interpolation/NormVecDecorator.cpp
    interpolation/CloughTocherInterpolator.cpp
    PROPERTIES COMPILE_FLAGS "-Wno-overloaded-virtual"
  )
ENDIF (CMAKE_CXX_COMPILER_ID MATCHES "Clang")

QT5_WRAP_CPP(QGIS_ANALYSIS_MOC_SRCS ${QGIS_ANALYSIS_MOC_HDRS})

# install headers

SET(QGIS_ANALYSIS_HDRS
  processing/qgsalgorithmimportphotos.h

  raster/qgsalignraster.h
  raster/qgsaspectfilter.h
  raster/qgsderivativefilter.h
  raster/qgshillshadefilter.h
  raster/qgskde.h
  raster/qgsninecellfilter.h
  raster/qgsrastercalculator.h
  raster/qgsrelief.h
  raster/qgsruggednessfilter.h
  raster/qgsslopefilter.h
  raster/qgsrastermatrix.h
  raster/qgsrastercalcnode.h
  raster/qgstotalcurvaturefilter.h

  vector/mersenne-twister.h
  vector/qgsgeometrysnapper.h
  vector/qgszonalstatistics.h
  vector/geometry_checker/qgsgeometrycheckerutils.h

  interpolation/qgsinterpolator.h
  interpolation/qgsgridfilewriter.h
  interpolation/qgsidwinterpolator.h
  interpolation/qgstininterpolator.h
  interpolation/Bezier3D.h
  interpolation/ParametricLine.h
  interpolation/CloughTocherInterpolator.h
  interpolation/TriangleInterpolator.h
  interpolation/Vector3D.h
  interpolation/DualEdgeTriangulation.h
  interpolation/MathUtils.h
  interpolation/TriDecorator.h
  interpolation/Triangulation.h
  interpolation/HalfEdge.h
  interpolation/LinTriangleInterpolator.h
  interpolation/NormVecDecorator.h

  network/qgsgraph.h
  network/qgsgraphbuilderinterface.h
  network/qgsgraphbuilder.h
  network/qgsnetworkstrategy.h
  network/qgsnetworkspeedstrategy.h
  network/qgsnetworkdistancestrategy.h
  network/qgsgraphanalyzer.h
  network/qgsvectorlayerdirector.h
)

INCLUDE_DIRECTORIES(
  ${CMAKE_CURRENT_SOURCE_DIR}
  ${CMAKE_SOURCE_DIR}/src/core/
  ${CMAKE_SOURCE_DIR}/src/core/geometry
  ${CMAKE_SOURCE_DIR}/src/core/processing
  ${CMAKE_SOURCE_DIR}/src/core/raster
  ${CMAKE_SOURCE_DIR}/src/core/symbology
  ${CMAKE_SOURCE_DIR}/src/core/metadata
  ${CMAKE_SOURCE_DIR}/src/core/expression
  ${CMAKE_BINARY_DIR}/src/core
  ${CMAKE_BINARY_DIR}/src/analysis
  interpolation
  network
)
INCLUDE_DIRECTORIES(SYSTEM
  ${SPATIALINDEX_INCLUDE_DIR} # before GEOS for case-insensitive filesystems
  ${PROJ_INCLUDE_DIR}
  ${GEOS_INCLUDE_DIR}
  ${GDAL_INCLUDE_DIR}
  ${SQLITE3_INCLUDE_DIR}
)

#############################################################
# qgis_analysis library

ADD_LIBRARY(qgis_analysis SHARED ${QGIS_ANALYSIS_SRCS} ${QGIS_ANALYSIS_MOC_SRCS} ${QGIS_ANALYSIS_HDRS})

GENERATE_EXPORT_HEADER(
   qgis_analysis
   BASE_NAME ANALYSIS
   EXPORT_FILE_NAME qgis_analysis.h
)
IF(MSVC)
  SET_TARGET_PROPERTIES(qgis_analysis PROPERTIES LINK_FLAGS "/FORCE:MULTIPLE")
ENDIF(MSVC)

SET(QGIS_ANALYSIS_HDRS ${QGIS_ANALYSIS_HDRS} ${CMAKE_CURRENT_BINARY_DIR}/qgis_analysis.h)

IF(NOT APPLE)
  INSTALL(FILES ${QGIS_ANALYSIS_HDRS} DESTINATION ${QGIS_INCLUDE_DIR})
ELSE(NOT APPLE)
  SET_TARGET_PROPERTIES(qgis_analysis PROPERTIES
    # no moc headers, messes up PROPERTIES syntax
    CLEAN_DIRECT_OUTPUT 1
    FRAMEWORK 1
    FRAMEWORK_VERSION "${CPACK_PACKAGE_VERSION_MAJOR}.${CPACK_PACKAGE_VERSION_MINOR}"
    MACOSX_FRAMEWORK_INFO_PLIST "${CMAKE_SOURCE_DIR}/mac/framework.info.plist.in"
    MACOSX_FRAMEWORK_SHORT_VERSION_STRING ${COMPLETE_VERSION}
    MACOSX_FRAMEWORK_IDENTIFIER org.qgis.qgis3_analysis
    BUILD_WITH_INSTALL_RPATH TRUE
    PUBLIC_HEADER "${QGIS_ANALYSIS_HDRS}"
    LINK_FLAGS "${CMAKE_SHARED_LINKER_FLAGS}"
  )
  # generated export header does not get copied with PUBLIC_HEADER files
  ADD_CUSTOM_COMMAND(TARGET qgis_analysis
    POST_BUILD
    COMMAND ${CMAKE_COMMAND} -E copy qgis_analysis.h
            "${QGIS_OUTPUT_DIRECTORY}/${QGIS_LIB_SUBDIR}/qgis_analysis.framework/Headers"
    WORKING_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}
    DEPENDS qgis_analysis.h
  )
ENDIF(NOT APPLE)

#generate unversioned libs for android
IF (NOT ANDROID)
  SET_TARGET_PROPERTIES(qgis_analysis PROPERTIES
    VERSION ${COMPLETE_VERSION}
    SOVERSION ${COMPLETE_VERSION}
    )
ENDIF (NOT ANDROID)

TARGET_LINK_LIBRARIES(qgis_analysis qgis_core)

# clang-tidy
IF(CLANG_TIDY_EXE)
  SET_TARGET_PROPERTIES(
    qgis_analysis PROPERTIES
    CXX_CLANG_TIDY "${DO_CLANG_TIDY}"
  )
ENDIF(CLANG_TIDY_EXE)

# install

INSTALL(TARGETS qgis_analysis
  RUNTIME DESTINATION ${QGIS_BIN_DIR}
  LIBRARY DESTINATION ${QGIS_LIB_DIR}
  ARCHIVE DESTINATION ${QGIS_LIB_DIR}
  FRAMEWORK DESTINATION ${QGIS_FW_SUBDIR}
  PUBLIC_HEADER DESTINATION ${QGIS_INCLUDE_DIR})

# Mac dev frameworks

IF (APPLE AND QGIS_MACAPP_INSTALL_DEV)
  INSTALL(TARGETS qgis_analysis FRAMEWORK DESTINATION ${QGIS_MACAPP_DEV_PREFIX})
  INSTALL(CODE "EXECUTE_PROCESS(COMMAND install_name_tool -id \"${QGIS_MACAPP_DEV_PREFIX}/qgis_analysis.framework/Versions/${CPACK_PACKAGE_VERSION_MAJOR}.${CPACK_PACKAGE_VERSION_MINOR}/qgis_analysis\" \"$ENV{DESTDIR}${QGIS_MACAPP_DEV_PREFIX}/qgis_analysis.framework/qgis_analysis\")")
  INSTALL(CODE "EXECUTE_PROCESS(COMMAND install_name_tool -change \"${CMAKE_INSTALL_NAME_DIR}/qgis_core.framework/Versions/${CPACK_PACKAGE_VERSION_MAJOR}.${CPACK_PACKAGE_VERSION_MINOR}/qgis_core\" \"${QGIS_MACAPP_DEV_PREFIX}/qgis_core.framework/Versions/${CPACK_PACKAGE_VERSION_MAJOR}.${CPACK_PACKAGE_VERSION_MINOR}/qgis_core\" \"$ENV{DESTDIR}${QGIS_MACAPP_DEV_PREFIX}/qgis_analysis.framework/qgis_analysis\")")
ENDIF (APPLE AND QGIS_MACAPP_INSTALL_DEV)
