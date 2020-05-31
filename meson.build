project('bimg', 'cpp', version : '1.0.0', license: 'BSD 2-Clause', default_options : ['cpp_std=c++14'])

includes = ['include', '3rdparty', '3rdparty/astc-codec/include', '3rdparty/iqa/include']

src = [
  'src/image.cpp',
  'src/image_cubemap_filter.cpp',
  'src/image_decode.cpp',
  'src/image_encode.cpp',
  'src/image_gnf.cpp'  
]

bx_dep = dependency('bx', fallback: ['bx', 'bx_dep'])

lib = static_library(
  'libbimg',
  src,
  include_directories : includes,
  dependencies        : bx_dep
)

bimg_dep = declare_dependency(include_directories : includes, link_with: lib)