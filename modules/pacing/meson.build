libpacing_files = files(
    'alr_detector.cc',
    'alr_detector.h',
    'bitrate_prober.cc',
    'bitrate_prober.h',
    'interval_budget.cc',
    'interval_budget.h',
    'paced_sender.cc',
    'paced_sender.h',
    'pacer.h',
    'packet_queue.cc',
    'packet_queue.h',
    'packet_queue_interface.cc',
    'packet_queue_interface.h',
    'packet_router.cc',
    'packet_router.h',
    'round_robin_packet_queue.cc',
    'round_robin_packet_queue.h',
)

libpacing = static_library(
  'pacing',
  libpacing_files,
  include_directories : [inc_common],
  cpp_args: internal_args,
)

all_libraries += libpacing
