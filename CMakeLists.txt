cmake_minimum_required (VERSION 3.24)

project(ImGuizmo)

set(IMGUIZMO_FILES 
	GraphEditor.cpp
	ImCurveEdit.cpp
	ImGradient.cpp
	ImGuizmo.cpp
	ImSequencer.cpp
)

add_library(${PROJECT_NAME} STATIC ${IMGUIZMO_FILES})
target_include_directories(${PROJECT_NAME} PUBLIC ./ ./example)