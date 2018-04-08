liblogging_files = files(
    # rtc_event_log_api
    'rtc_event_log/encoder/rtc_event_log_encoder.h',
    'rtc_event_log/events/rtc_event.h',
    'rtc_event_log/rtc_event_log.cc',
    'rtc_event_log/rtc_event_log.h',
    'rtc_event_log/rtc_event_log_factory_interface.h',

    # rtc_stream_config
    'rtc_event_log/rtc_stream_config.cc',
    'rtc_event_log/rtc_stream_config.h',

    # rtc_event_pacing
    'rtc_event_log/events/rtc_event_alr_state.cc',
    'rtc_event_log/events/rtc_event_alr_state.h',

    # rtc_event_audio
    'rtc_event_log/events/rtc_event_audio_network_adaptation.cc',
    'rtc_event_log/events/rtc_event_audio_network_adaptation.h',
    'rtc_event_log/events/rtc_event_audio_playout.cc',
    'rtc_event_log/events/rtc_event_audio_playout.h',
    'rtc_event_log/events/rtc_event_audio_receive_stream_config.cc',
    'rtc_event_log/events/rtc_event_audio_receive_stream_config.h',
    'rtc_event_log/events/rtc_event_audio_send_stream_config.cc',
    'rtc_event_log/events/rtc_event_audio_send_stream_config.h',

    # rtc_event_bwe
    'rtc_event_log/events/rtc_event_bwe_update_delay_based.cc',
    'rtc_event_log/events/rtc_event_bwe_update_delay_based.h',
    'rtc_event_log/events/rtc_event_bwe_update_loss_based.cc',
    'rtc_event_log/events/rtc_event_bwe_update_loss_based.h',
    'rtc_event_log/events/rtc_event_probe_cluster_created.cc',
    'rtc_event_log/events/rtc_event_probe_cluster_created.h',
    'rtc_event_log/events/rtc_event_probe_result_failure.cc',
    'rtc_event_log/events/rtc_event_probe_result_failure.h',
    'rtc_event_log/events/rtc_event_probe_result_success.cc',
    'rtc_event_log/events/rtc_event_probe_result_success.h',

    # rtc_event_rtp_rtcp
    'rtc_event_log/events/rtc_event_rtcp_packet_incoming.cc',
    'rtc_event_log/events/rtc_event_rtcp_packet_incoming.h',
    'rtc_event_log/events/rtc_event_rtcp_packet_outgoing.cc',
    'rtc_event_log/events/rtc_event_rtcp_packet_outgoing.h',
    'rtc_event_log/events/rtc_event_rtp_packet_incoming.cc',
    'rtc_event_log/events/rtc_event_rtp_packet_incoming.h',
    'rtc_event_log/events/rtc_event_rtp_packet_outgoing.cc',
    'rtc_event_log/events/rtc_event_rtp_packet_outgoing.h',

    # rtc_event_video
    'rtc_event_log/events/rtc_event_video_receive_stream_config.cc',
    'rtc_event_log/events/rtc_event_video_receive_stream_config.h',
    'rtc_event_log/events/rtc_event_video_send_stream_config.cc',
    'rtc_event_log/events/rtc_event_video_send_stream_config.h',

    # rtc_event_log_impl_encoder
    'rtc_event_log/encoder/rtc_event_log_encoder_legacy.cc',
    'rtc_event_log/encoder/rtc_event_log_encoder_legacy.h',

    # rtc_event_log_impl_output
    'rtc_event_log/output/rtc_event_log_output_file.cc',
    'rtc_event_log/output/rtc_event_log_output_file.h',

    # rtc_event_log_impl_base
    'rtc_event_log/rtc_event_log_factory.cc',
    'rtc_event_log/rtc_event_log_factory.h',
    'rtc_event_log/rtc_event_log_impl.cc',

    # ice_log
    'rtc_event_log/events/rtc_event_ice_candidate_pair.cc',
    'rtc_event_log/events/rtc_event_ice_candidate_pair.h',
    'rtc_event_log/events/rtc_event_ice_candidate_pair_config.cc',
    'rtc_event_log/events/rtc_event_ice_candidate_pair_config.h',
    'rtc_event_log/icelogger.cc',
    'rtc_event_log/icelogger.h',
)


liblogging = static_library(
  'logging',
  liblogging_files,
  include_directories : [inc_common],
  cpp_args: internal_args,
)

all_libraries += liblogging
