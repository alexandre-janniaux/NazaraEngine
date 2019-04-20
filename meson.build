project('nazara', ['cpp'],
  version: '0.4.0',
  default_options: [],
  meson_version: '>= 0.47.0',
  license: 'MIT')

nazara_soname_version = '0.4.0'

# tools
cxx = meson.get_compiler('cpp')

nazara_includes = include_directories('include')
thirdparty_includes = include_directories('thirdparty/include')

subdir('src')
# subdir(examples)
# subdir(SDK)
# subdir(tests)
