cxx_library(
  name = 'grpc',
  header_namespace = '',
  exported_headers = subdir_glob([
    ('grpc', '**/*.h'),
  ]),
  srcs = glob([
    'grpc/src/**/*.cpp',
  ]),
)

cxx_library(
  name = 'flatbuffers',
  header_namespace = 'flatbuffers',
  exported_headers = subdir_glob([
    ('include/flatbuffers', '*.h'),
  ]),
  srcs = glob([
    'src/*.cpp',
  ]),
  compiler_flags = [
    '-std=c++14',
  ],
  visibility = [
    'PUBLIC',
  ],
  deps = [
    ':grpc',
  ],
)
