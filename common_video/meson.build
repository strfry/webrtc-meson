libcommon_video_files = files(
    'bitrate_adjuster.cc',
    'h264/h264_bitstream_parser.cc',
    'h264/h264_bitstream_parser.h',
    'h264/h264_common.cc',
    'h264/h264_common.h',
    'h264/pps_parser.cc',
    'h264/pps_parser.h',
    'h264/profile_level_id.h',
    'h264/sps_parser.cc',
    'h264/sps_parser.h',
    'h264/sps_vui_rewriter.cc',
    'h264/sps_vui_rewriter.h',
    'i420_buffer_pool.cc',
    'include/bitrate_adjuster.h',
    'include/frame_callback.h',
    'include/i420_buffer_pool.h',
    'include/incoming_video_stream.h',
    'include/video_bitrate_allocator.h',
    'include/video_frame.h',
    'include/video_frame_buffer.h',
    'incoming_video_stream.cc',
    'libyuv/include/webrtc_libyuv.h',
    'libyuv/webrtc_libyuv.cc',
    'video_frame.cc',
    'video_frame_buffer.cc',
    'video_render_frames.cc',
    'video_render_frames.h',
)

libcommon_video = static_library(
  'common_video',
  libcommon_video_files,
  include_directories : [inc_common],
  cpp_args: internal_args,
)

all_libraries += libcommon_video
