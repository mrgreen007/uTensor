set(src_utensor_core
    types.cpp
    uTensor_util.cpp
    tensorBase.cpp
    memoryManagementInterface.cpp
    context.cpp
    tensor.cpp
    TensorMap.cpp
    operatorBase.cpp
    errorHandler.cpp
    modelBase.cpp
    quantizationPrimitives.cpp
   )

set(hdr_utensor_core
    types.hpp
    uTensor_util.hpp
    tensorBase.hpp
    memoryManagementInterface.hpp
    context.hpp
    tensor.hpp
    TensorMap.hpp
    operatorBase.hpp
    utensor_string.hpp
    errorHandler.hpp
    modelBase.hpp
    quantizationPrimitives.hpp
   )
    
add_library(utensor_core ${src_utensor_core} )
target_include_directories(utensor_core PUBLIC .)
target_compile_features(utensor_core PUBLIC cxx_std_11)
