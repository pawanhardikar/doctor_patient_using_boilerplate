cmake_minimum_required(VERSION 3.10)
project(doctor_patient_system VERSION 0.1.0 DESCRIPTION "Doctor Patient Creation and Appointment created using cpp devops boilerplate template" LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

include_directories(include)

file(GLOB SOURCES "src/*.cpp")

add_executable(doctor_patient_system ${SOURCES})

# enable_testing()
# add_executable(test_runner tests/test_sample.cpp)
# add_test(NAME test_runner COMMAND test_runner)