################################################################################
#                                                                              #
# This file is part of IfcOpenShell.                                           #
#                                                                              #
# IfcOpenShell is free software: you can redistribute it and/or modify         #
# it under the terms of the Lesser GNU General Public License as published by  #
# the Free Software Foundation, either version 3.0 of the License, or          #
# (at your option) any later version.                                          #
#                                                                              #
# IfcOpenShell is distributed in the hope that it will be useful,              #
# but WITHOUT ANY WARRANTY; without even the implied warranty of               #
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the                 #
# Lesser GNU General Public License for more details.                          #
#                                                                              #
# You should have received a copy of the Lesser GNU General Public License     #
# along with this program. If not, see <http://www.gnu.org/licenses/>.         #
#                                                                              #
################################################################################

ADD_EXECUTABLE(hdf5_federate federate.cpp)
TARGET_LINK_LIBRARIES(hdf5_federate IfcParse ${ICU_LIBRARIES} ${Boost_LIBRARIES})

ADD_EXECUTABLE(hdf5_lod lod.cpp)
TARGET_LINK_LIBRARIES(hdf5_lod IfcParse IfcGeom ${OPENCASCADE_LIBRARIES} ${Boost_LIBRARIES} ${ICU_LIBRARIES})
