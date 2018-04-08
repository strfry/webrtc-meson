libaudio_files = files(
    'audio_level.cc',
    'audio_level.h',
    'audio_receive_stream.cc',
    'audio_receive_stream.h',
    'audio_send_stream.cc',
    'audio_send_stream.h',
    'audio_state.cc',
    'audio_state.h',
    'audio_transport_impl.cc',
    'audio_transport_impl.h',
    'channel.cc',
    'channel.h',
    'channel_proxy.cc',
    'channel_proxy.h',
    'conversion.h',
    'null_audio_poller.cc',
    'null_audio_poller.h',
    'remix_resample.cc',
    'remix_resample.h',
    'time_interval.cc',
    'time_interval.h',
    'transport_feedback_packet_loss_tracker.cc',
    'transport_feedback_packet_loss_tracker.h',
)

# audio/utility
libaudio_files += files(
    'utility/audio_frame_operations.cc',
    'utility/audio_frame_operations.h',
)

libaudio = static_library(
  'audio',
  libaudio_files,
  include_directories : inc_common,
  cpp_args: internal_args,
)

all_libraries += libaudio
