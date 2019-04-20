nazara_platform_sources = files(
    'Cursor.cpp',
    'Icon.cpp',
    'Keyboard.cpp',
    'Mouse.cpp',
    'Platform.cpp',
    'VideoMode.cpp',
    'Window.cpp',)

nazara_platform_x11_sources = files(
    'X11/CursorImpl.cpp',
    'X11/CursorImpl.hpp',
    'X11/Display.cpp',
    'X11/Display.hpp',
    'X11/IconImpl.cpp',
    'X11/IconImpl.hpp',
    'X11/InputImpl.cpp',
    'X11/InputImpl.hpp',
    'X11/ScopedXCB.cpp',
    'X11/ScopedXCB.hpp',
    'X11/VideoModeImpl.cpp',
    'X11/VideoModeImpl.hpp',
    'X11/WindowImpl.cpp',
    'X11/WindowImpl.hpp',)

nazara_platform_sources += nazara_platform_x11_sources

xcb_dep = cxx.find_library('xcb')
xcb_randr_dep = cxx.find_library('xcb-randr')
xcb_icccm_dep = cxx.find_library('xcb-icccm')
xcb_ewmh_dep = cxx.find_library('xcb-ewmh')
xcb_xkb_dep = cxx.find_library('xcb-xkb')
xkbcommon_x11_dep = cxx.find_library('xkbcommon-x11')

library('nazara-platform',
  nazara_platform_sources,
  include_directories: [nazara_includes, thirdparty_includes],
  dependencies: [
    xcb_dep,
    xcb_randr_dep,
    xcb_icccm_dep,
    xcb_ewmh_dep,
    xkbcommon_x11_dep,
    nazara_core_dep])
