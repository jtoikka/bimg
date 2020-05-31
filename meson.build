project('bimg', 'cpp', version : '1.0.0', license: 'BSD 2-Clause', default_options : ['cpp_std=c++14'])

includes = ['include', '3rdparty']

src = ['src/amalgamated.cpp']

lib = static_library(
  'libbimg',
  src,
  include_directories : includes
)

bimg_dep = declare_dependency(include_directories : includes, link_with: lib)