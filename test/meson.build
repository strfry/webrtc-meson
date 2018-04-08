libtest_files = files(
    'fake_texture_frame.cc',
    'fake_texture_frame.h',
    'frame_generator.cc',
    'frame_generator.h',
    'frame_generator_capturer.cc',
    'frame_generator_capturer.h',
    'frame_utils.cc',
    'frame_utils.h',
    'vcm_capturer.cc',
    'vcm_capturer.h',
    'video_capturer.cc',
    'video_capturer.h',
    'video_codec_settings.h',

    # rtp_test_utils
    'rtcp_packet_parser.cc',
    'rtcp_packet_parser.h',
    'rtp_file_reader.cc',
    'rtp_file_reader.h',
    'rtp_file_writer.cc',
    'rtp_file_writer.h',

    # field_trial
    'field_trial.cc',
    'field_trial.h',

    # perf_test
    'testsupport/perf_test.cc',
    'testsupport/perf_test.h',
)


libtest = static_library(
  'webrtc_test',
  libtest_files,
  include_directories : [inc_common],
  cpp_args: internal_args,
)

all_libraries += libtest
