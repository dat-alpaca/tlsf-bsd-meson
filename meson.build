project('tlsf-bsd', 'c')

sources = files(
    'src/tlsf.c',
    'src/tlsf_thread.c'
)

tlsf_includes = include_directories('include')
tlsf_lib = static_library(
    'tlsf',
    sources: sources,
    include_directories: tlsf_includes,
)

tlsf_dep = declare_dependency(
    include_directories: tlsf_includes,
    link_with: tlsf_lib
)