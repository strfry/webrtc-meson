libbitrate_controller_files = files(
    'bitrate_controller_impl.cc',
    'bitrate_controller_impl.h',
    'include/bitrate_controller.h',
    'send_side_bandwidth_estimation.cc',
    'send_side_bandwidth_estimation.h',
)

libbitrate_controller = static_library(
  'bitrate_controller',
  libbitrate_controller_files,
  include_directories : [inc_common],
  cpp_args: internal_args,
)

all_libraries += libbitrate_controller
