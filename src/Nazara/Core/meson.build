nazara_core_sources = files(
    'AbstractHash.cpp',
    'AbstractLogger.cpp',
    'AlgorithmCore.cpp',
    'ByteArray.cpp',
    'ByteStream.cpp',
    'Clock.cpp',
    'Color.cpp',
    'ConditionVariable.cpp',
    'Core.cpp',
    'Directory.cpp',
    'DynLib.cpp',
    'Error.cpp',
    'ErrorFlags.cpp',
    'File.cpp',
    'FileLogger.cpp',
    'GuillotineBinPack.cpp',
    'HandledObject.cpp',
    'HardwareInfo.cpp',
    'Log.cpp',
    'MemoryManager.cpp',
    'MemoryStream.cpp',
    'MemoryView.cpp',
    'Mutex.cpp',
    'ParameterList.cpp',
    'PluginManager.cpp',
    'PrimitiveList.cpp',
    'RefCounted.cpp',
    'Resource.cpp',
    'Semaphore.cpp',
    'SerializationContext.cpp',
    'StdLogger.cpp',
    'Stream.cpp',
    'String.cpp',
    'StringStream.cpp',
    'TaskScheduler.cpp',
    'Thread.cpp',
    'Unicode.cpp',
    'UnicodeData.hpp',
    'Updatable.cpp',)

nazara_core_hash_sources = files(
  'Hash/SHA/Internal.cpp',
  'Hash/SHA/Internal.hpp',
  'Hash/CRC32.cpp',
  'Hash/CRC64.cpp',
  'Hash/Fletcher16.cpp',
  'Hash/MD5.cpp',
  'Hash/SHA1.cpp',
  'Hash/SHA224.cpp',
  'Hash/SHA256.cpp',
  'Hash/SHA384.cpp',
  'Hash/SHA512.cpp',
  'Hash/Whirlpool.cpp',)
nazara_core_sources += nazara_core_hash_sources

nazara_core_posix_sources = files(
    'Posix/ClockImpl.cpp',
    'Posix/ClockImpl.hpp',
    'Posix/ConditionVariableImpl.cpp',
    'Posix/ConditionVariableImpl.hpp',
    'Posix/DirectoryImpl.cpp',
    'Posix/DirectoryImpl.hpp',
    'Posix/DynLibImpl.cpp',
    'Posix/DynLibImpl.hpp',
    'Posix/FileImpl.cpp',
    'Posix/FileImpl.hpp',
    'Posix/HardwareInfoImpl.cpp',
    'Posix/HardwareInfoImpl.hpp',
    'Posix/MutexImpl.cpp',
    'Posix/MutexImpl.hpp',
    'Posix/SemaphoreImpl.cpp',
    'Posix/SemaphoreImpl.hpp',
    'Posix/TaskSchedulerImpl.cpp',
    'Posix/TaskSchedulerImpl.hpp',
    'Posix/ThreadImpl.cpp',
    'Posix/ThreadImpl.hpp',)

nazara_core_sources += nazara_core_posix_sources

thread_dep = dependency('threads')
dl_dep = cxx.find_library('dl', required: false)

nazara_core_lib = library('nazara-core',
  nazara_core_sources,
  include_directories: [nazara_includes, thirdparty_includes],
  dependencies: [thread_dep, dl_dep])

nazara_core_dep = declare_dependency(link_with: nazara_core_lib)
