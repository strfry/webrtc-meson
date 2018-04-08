libcall_files = files(
    'call.cc',
    'callfactory.cc',
    'callfactory.h',
    'degraded_call.cc',
    'degraded_call.h',
    'flexfec_receive_stream_impl.cc',
    'flexfec_receive_stream_impl.h',
    'receive_time_calculator.cc',
    'receive_time_calculator.h',

    # call_interfaces
    'audio_receive_stream.h',
    'audio_send_stream.h',
    'audio_state.h',
    'call.h',
    'flexfec_receive_stream.h',
    'syncable.cc',
    'syncable.h',
    'audio_send_stream.cc',

    # rtp_interfaces
    'bitrate_constraints.cc',
    'bitrate_constraints.h',
    'rtcp_packet_sink_interface.h',
    'rtp_config.cc',
    'rtp_config.h',
    'rtp_packet_sink_interface.h',
    'rtp_stream_receiver_controller_interface.h',
    'rtp_transport_controller_send_interface.h',

    # rtp_sender
    'rtp_transport_controller_send.cc',
    'rtp_transport_controller_send.h',

    # rtp_receiver
    'rtcp_demuxer.cc',
    'rtcp_demuxer.h',
    'rtp_demuxer.cc',
    'rtp_demuxer.h',
    'rtp_rtcp_demuxer_helper.cc',
    'rtp_rtcp_demuxer_helper.h',
    'rtp_stream_receiver_controller.cc',
    'rtp_stream_receiver_controller.h',
    'rtx_receive_stream.cc',
    'rtx_receive_stream.h',
    'ssrc_binding_observer.h',

    # bitrate_configurator
    'rtp_bitrate_configurator.cc',
    'rtp_bitrate_configurator.h',

    # bitrate_allocator
    'bitrate_allocator.cc',
    'bitrate_allocator.h',

    # video_stream_api
    'video_config.cc',
    'video_config.h',
    'video_receive_stream.cc',
    'video_receive_stream.h',
    'video_send_stream.cc',
    'video_send_stream.h',

    # fake_network
    'fake_network_pipe.cc',
    'fake_network_pipe.h',
)


libcall = static_library(
  'call',
  libcall_files,
  include_directories : [inc_common],
  cpp_args: internal_args,
)

all_libraries += libcall
