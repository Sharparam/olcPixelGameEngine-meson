project('olcPixelGameEngine', 'cpp',
  version: '2.23',
  default_options: ['cpp_std=c++17'])

libpng_dep = dependency('libpng')
gl_dep = dependency('gl')
x11_dep = dependency('x11')

olc_pge_incdir = include_directories('include')

olc_pge_sources = files(['src/olcPixelGameEngine.cpp'])

olc_pge_lib = library('olcPixelGameEngine', olc_pge_sources,
  include_directories: olc_pge_incdir,
  dependencies: [libpng_dep, gl_dep, x11_dep],
  install: true)

olc_pge_dep = declare_dependency(
  include_directories: olc_pge_incdir,
  link_with: olc_pge_lib)
