nazara_renderer_sources = files(
  'Context.cpp',
  'ContextParameters.cpp',
  'DebugDrawer.cpp',
  'GlslWriter.cpp',
  'GpuQuery.cpp',
  'HardwareBuffer.cpp',
  'OpenGL.cpp',
  'RenderBuffer.cpp',
  'Renderer.cpp',
  'RenderTarget.cpp',
  'RenderTexture.cpp',
  'RenderWindow.cpp',
  'Shader.cpp',
  'ShaderAst.cpp',
  'ShaderStage.cpp',
  'ShaderWriter.cpp',
  'Texture.cpp',
  'TextureSampler.cpp',
  'UberShader.cpp',
  'UberShaderInstance.cpp',
  'UberShaderInstancePreprocessor.cpp',
  'UberShaderPreprocessor.cpp',)

nazara_renderer_glx_sources = files(
  'GLX/ContextImpl.cpp',)

nazara_renderer_sources += nazara_renderer_glx_sources

glx_dep = cxx.find_library('GLX')
xcb_dep = cxx.find_library('xcb')
x11_dep = cxx.find_library('X11')

library('nazara-renderer',
  nazara_renderer_sources,
  include_directories: [nazara_includes],
  dependencies: [ xcb_dep, glx_dep, x11_dep,
                  nazara_platform_dep, nazara_utility_dep, nazara_core_dep ],
  cpp_args: '-DNAZARA_RENDERER_OPENGL')
