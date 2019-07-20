nazara_physics2d_sources = files(
    'Arbiter2D.cpp',
    'Collider2D.cpp',
    'Constraint2D.cpp',
    'Physics2D.cpp',
    'PhysWorld2D.cpp',
    'RigidBody2D.cpp',
    'Debug/NewOverload.cpp',)

chipmunk_dep = cxx.find_library('chipmunk', version: '>= 7.0.2')

library('nazara-physics2d',
  nazara_physics2d_sources,
  include_directories: [nazara_includes],
  dependencies: [chipmunk_dep, nazara_core_dep])
