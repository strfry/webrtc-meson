libvideo_capture_files = files(
    #'external/device_info_external.cc',
    #'external/video_capture_external.cc',
    
    # video_capture_module
    'device_info_impl.cc',
    'device_info_impl.h',
    'video_capture.h',
    'video_capture_config.h',
    'video_capture_defines.h',
    'video_capture_factory.cc',
    'video_capture_factory.h',
    'video_capture_impl.cc',
    'video_capture_impl.h',
)

# TODO: Test for Linux
libvideo_capture_files += files(
    'linux/device_info_linux.cc',
    'linux/device_info_linux.h',
    'linux/video_capture_linux.cc',
    'linux/video_capture_linux.h',
)


libvideo_capture = static_library(
  'video_capture',
  libvideo_capture_files,
  include_directories : [inc_common],
  cpp_args: internal_args,
)

all_libraries += libvideo_capture
