nazara_lua_sources = files(
    'LuaCoroutine.cpp',
    'Lua.cpp',
    'LuaInstance.cpp',
    'LuaState.cpp',)

lua_dep = cxx.find_library('lua')

library('nazara-lua',
  nazara_lua_sources,
  include_directories: [nazara_includes],
  dependencies: [lua_dep, nazara_core_dep])
