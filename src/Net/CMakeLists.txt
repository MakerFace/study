
find_package(Poco COMPONENTS Net)

add_executable(server server.cpp)
target_link_libraries(server Poco::Net)

add_executable(client client.cpp)
target_link_libraries(client Poco::Net)