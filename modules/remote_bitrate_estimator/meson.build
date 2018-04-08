libremote_bitrate_estimator_files = files(
    'aimd_rate_control.cc',
    'aimd_rate_control.h',
    'bwe_defines.cc',
    'include/bwe_defines.h',
    'include/remote_bitrate_estimator.h',
    'inter_arrival.cc',
    'inter_arrival.h',
    'overuse_detector.cc',
    'overuse_detector.h',
    'overuse_estimator.cc',
    'overuse_estimator.h',
    'remote_bitrate_estimator_abs_send_time.cc',
    'remote_bitrate_estimator_abs_send_time.h',
    'remote_bitrate_estimator_single_stream.cc',
    'remote_bitrate_estimator_single_stream.h',
    'remote_estimator_proxy.cc',
    'remote_estimator_proxy.h',
    'test/bwe_test_logging.h',

    #bwe_rtp
    'tools/bwe_rtp.cc',
    'tools/bwe_rtp.h',
)

libremote_bitrate_estimator = static_library(
  'remote_bitrate_estimator',
  libremote_bitrate_estimator_files,
  include_directories : [inc_common],
  cpp_args: internal_args,
)

all_libraries += libremote_bitrate_estimator
