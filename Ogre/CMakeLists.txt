FIND_PACKAGE(OGRE REQUIRED)
FIND_PACKAGE(OIS REQUIRED)

INCLUDE_DIRECTORIES (${OGRE_INCLUDE_DIRS} ${OIS_INCLUDE_DIRS})
LINK_LIBRARIES      (${OGRE_LIBRARIES} ${OIS_LIBRARIES})

IF(OGRE_FOUND)
  GENERATE_BINDINGS(Ogre)
ENDIF()