zlib_dep = dependency('zlib', required: get_option('zlib'))
if not zlib_dep.found()
  subdir_done()
endif

zlib = static_library(
  'zlib',
  'Error.cxx',
  include_directories: inc,
  dependencies: [
    zlib_dep,
  ],
)

zlib_dep = declare_dependency(
  link_with: zlib,
)
