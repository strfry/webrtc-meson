libsystem_wrappers_files = files(
    'include/clock.h',
    'include/cpu_info.h',
    'include/event_wrapper.h',
    'include/ntp_time.h',
    'include/rtp_to_ntp_estimator.h',
    'include/sleep.h',
    'source/clock.cc',
    'source/cpu_features.cc',
    'source/cpu_info.cc',
    'source/event.cc',
    'source/event_timer_posix.cc',
    'source/event_timer_posix.h',
#    'source/event_timer_win.cc', # Why is this not wrapped in BUILD.gn?
#    'source/event_timer_win.h',
    'source/rtp_to_ntp_estimator.cc',
    'source/sleep.cc',

    # field_trial_default
    'include/field_trial_default.h',
    'source/field_trial_default.cc',

    # runtime_enabled_features_default
    'source/runtime_enabled_features_default.cc',

    # metrics_default
    'include/metrics_default.h',
    'source/metrics_default.cc',

    # TODO: make portable
    # cpu_features_linux
    'source/cpu_features_linux.c',
)

libsystem_wrappers_files += files(
    # metrics_default
    'include/metrics_default.h',
    'source/metrics_default.cc',

    # field_trial_default
    'include/field_trial_default.h',
    'source/field_trial_default.cc',

)

libsystem_wrappers = static_library(
  'system_wrappers',
  libsystem_wrappers_files,
  include_directories : [inc_common],
  cpp_args: internal_args,
)

all_libraries += libsystem_wrappers
