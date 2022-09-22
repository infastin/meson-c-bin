src_files = [
]

header_files = [
]

libproject = both_libraries('project', src_files)

libproject_dep = declare_dependency(
  sources: header_files,
  link_with: libproject,
  include_directories: include_directories('.'),
)

main = executable('main', 'main.c',
  dependencies: libproject_dep
)
