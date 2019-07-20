nazara_physics3d_sources = files(
    'Collider3D.cpp',
    'Physics3D.cpp',
    'PhysWorld3D.cpp',
    'RigidBody3D.cpp',)

#xkbcommon_x11_dep = cxx.find_library('xkbcommon-x11')

newton_dep = cxx.find_library('newton')

library('nazara-physics3d',
  nazara_physics3d_sources,
  include_directories: [nazara_includes, thirdparty_includes],
  dependencies: [newton_dep, nazara_core_dep])
