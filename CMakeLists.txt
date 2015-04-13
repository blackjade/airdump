# CMakeLists.txt

cmake_minimum_required(VERSION 2.8)
project( airdump )
set (CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake")
find_package( PCAP REQUIRED )
add_executable( airdump main.cpp util.cpp sniffer.cpp )
target_link_libraries( airdump ${PCAP_LIBRARY} )
