nazara_utility_sources = files(
  'AbstractAtlas.cpp',
  'AbstractBuffer.cpp',
  'AbstractImage.cpp',
  'AbstractTextDrawer.cpp',
  'AlgorithmUtility.cpp',
  'Animation.cpp',
  'Buffer.cpp',
  'Font.cpp',
  'FontData.cpp',
  'GuillotineImageAtlas.cpp',
  'Image.cpp',
  'IndexBuffer.cpp',
  'IndexMapper.cpp',
  'Joint.cpp',
  'Mesh.cpp',
  'Node.cpp',
  'PixelFormat.cpp',
  'SimpleTextDrawer.cpp',
  'SkeletalMesh.cpp',
  'Skeleton.cpp',
  'SoftwareBuffer.cpp',
  'StaticMesh.cpp',
  'SubMesh.cpp',
  'TriangleIterator.cpp',
  'Utility.cpp',
  'VertexBuffer.cpp',
  'VertexDeclaration.cpp',
  'VertexMapper.cpp',
  'Formats/DDSConstants.cpp',
  'Formats/DDSLoader.cpp',
  'Formats/FreeTypeLoader.cpp',
  'Formats/MD2Constants.cpp',
  'Formats/MD2Loader.cpp',
  'Formats/MD5AnimLoader.cpp',
  'Formats/MD5AnimParser.cpp',
  'Formats/MD5MeshLoader.cpp',
  'Formats/MD5MeshParser.cpp',
  'Formats/MTLParser.cpp',
  'Formats/OBJLoader.cpp',
  'Formats/OBJParser.cpp',
  'Formats/OBJSaver.cpp',
  'Formats/PCXLoader.cpp',
  'Formats/STBLoader.cpp',
  'Formats/STBSaver.cpp',)

nazara_utility_sources += stbimage_sources

freetype_dep = cxx.find_library('freetype')

nazara_utility_lib = library('nazara-utility',
  nazara_utility_sources,
  include_directories: [nazara_includes, thirdparty_includes],
  dependencies: [nazara_core_dep, freetype_dep])

nazara_utility_dep = declare_dependency(link_with: nazara_utility_lib)

