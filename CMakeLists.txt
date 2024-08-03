cmake_minimum_required(VERSION 3.28)
project(RubiksCubeSolver)

set(CMAKE_CXX_STANDARD 17)

add_executable(RubiksCubeSolver main.cpp
        Model/RubiksCube.cpp
        Model/RubiksCube.h
        Model/RubiksCube1dArray.cpp
        Model/RubiksCube3dArray.cpp
        Model/RubiksCubeBitboard.cpp
        Model/PatternDatabase/PatternDatabase.h
        PatternDatabases/CornerDBMaker.cpp
        PatternDatabases/CornerDBMaker.h
        PatternDatabases/CornerPatternDatabase.cpp
        PatternDatabases/CornerPatternDatabase.h
        PatternDatabases/NibbleArray.cpp
        PatternDatabases/NibbleArray.h
        PatternDatabases/PatternDatabase.cpp
        PatternDatabases/PatternDatabase.h
        PatternDatabases/math.cpp
        PatternDatabases/math.h
        PatternDatabases/PermutationIndexer.h
        Solvers/BFSSolver.h
        Solvers/DFSSolver.h
        Solvers/IDAStarSolver.h
        Solvers/IDDFSSolver.h)
