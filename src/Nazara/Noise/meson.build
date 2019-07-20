nazara_noise_sources = files(
    'FBM.cpp',
    'HybridMultiFractal.cpp',
    'MixerBase.cpp',
    'NoiseBase.cpp',
    'Noise.cpp',
    'NoiseTools.cpp',
    'Perlin.cpp',
    'Simplex.cpp',
    'Worley.cpp',
    'Debug/NewOverload.cpp',)

library('nazara-noise',
  nazara_noise_sources,
  include_directories: [nazara_includes, thirdparty_includes],
  dependencies: [nazara_core_dep])
