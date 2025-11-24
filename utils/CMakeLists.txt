# SPDX-FileCopyrightText: 2025 Contributors to the Media eXchange Layer project.
# SPDX-License-Identifier: Apache-2.0

if(CPACK_DEBIAN_PACKAGE_DEPENDS MATCHES ".*gst.*")
    message(STATUS "Adding gst-looping-filesrc")
	add_subdirectory(gst-looping-filesrc)
else()
    message(STATUS "Skipping gst-looping-filesrc")
endif()
