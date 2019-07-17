nazara_network_sources = files(
    'AbstractSocket.cpp',
    'AlgorithmNetwork.cpp',
    'ENetCompressor.cpp',
    'ENetHost.cpp',
    'ENetPacket.cpp',
    'ENetPeer.cpp',
    'IpAddress.cpp',
    'NetPacket.cpp',
    'Network.cpp',
    'RUdpConnection.cpp',
    'SocketPoller.cpp',
    'TcpClient.cpp',
    'TcpServer.cpp',
    'UdpSocket.cpp',)

nazara_network_posix_sources = files(
    'Posix/IpAddressImpl.cpp',
    'Posix/SocketImpl.cpp',
    'Posix/SocketPollerImpl.cpp',)

nazara_network_linux_sources = files(
    'Posix/IpAddressImpl.cpp',
    'Posix/SocketImpl.cpp',
    'Linux/SocketPollerImpl.cpp',)

nazara_network_sources += nazara_network_linux_sources

library('nazara-network',
  nazara_network_sources,
  include_directories: [nazara_includes, thirdparty_includes],
  dependencies: [nazara_core_dep])
