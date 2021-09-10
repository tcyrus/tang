project('jose', 'c', license: 'APL2',
  version: '11',
  default_options: [
    'c_std=gnu99',
    'prefix=/usr',
    'warning_level=2',
    'werror=true'
  ]
)

add_project_arguments(
  '-Wstrict-aliasing',
  '-Wchar-subscripts',
  '-Wformat-security',
  '-Wmissing-declarations',
  '-Wmissing-prototypes',
  '-Wnested-externs',
  '-Wpointer-arith',
  '-Wshadow',
  '-Wsign-compare',
  '-Wstrict-prototypes',
  '-Wtype-limits',
  '-Wunused-function',
  '-Wno-missing-field-initializers',
  '-Wno-unused-command-line-argument',
  '-Wno-unused-parameter',
  '-Wno-unknown-pragmas',
  language: 'c'
)

zlib = dependency('zlib', static: true)
threads = dependency('threads', static: true)
jansson = dependency('jansson', version: '>=2.10', static: true)
libcrypto = dependency('libcrypto', version: '>=1.0.2', static: true)

subdir('include')
subdir('lib')
