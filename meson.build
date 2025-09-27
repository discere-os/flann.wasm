project('flann.wasm',['cpp'],version:'1.9.x',meson_version:'>=1.3.0',default_options:['buildtype=release','cpp_std=c++17'])
fs = import('fs')
if get_option('simd')
  add_project_arguments('-msimd128', language:'cpp')
endif
incs = [ include_directories('src/cpp'), include_directories('src/cpp/flann') ]
core = static_library('flann_core', ['src/cpp/flann/flann.cpp','src/cpp/flann/flann_cpp.cpp'], include_directories: incs)
if get_option('main_module')
  executable('flann-main','src/flann_wasm_module.cpp', link_with: core, include_directories: incs, install:true,
    link_args:['--no-entry','-sMODULARIZE=1','-sEXPORT_ES6=1','-sALLOW_MEMORY_GROWTH=1','-sENVIRONMENT=web,webview,worker','-sNO_FILESYSTEM=1','-sEXPORTED_RUNTIME_METHODS=["cwrap","ccall","UTF8ToString"]','-sEXPORTED_FUNCTIONS=@' + meson.project_source_root()/get_option('exports')])
endif
if get_option('side_module')
  shared_module('flann-side','src/flann_wasm_side.cpp', link_whole: core, include_directories: incs, name_prefix:'', install:true, link_args:['-sSIDE_MODULE=2','-fPIC'])
endif
