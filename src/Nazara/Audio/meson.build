nazara_audio_sources = files(
    'Audio.cpp',
    'Music.cpp',
    'OpenAL.cpp',
    'Sound.cpp',
    'SoundBuffer.cpp',
    'SoundEmitter.cpp',
    'SoundStream.cpp',
    'Formats/sndfileLoader.cpp',)

sndfile_dep = cxx.find_library('sndfile')

library('nazara-audio',
  nazara_audio_sources,
  include_directories: [nazara_includes, thirdparty_includes],
  dependencies: [sndfile_dep, nazara_core_dep],
  cpp_args: ['-DNAZARA_AUDIO_OPENAL'])
