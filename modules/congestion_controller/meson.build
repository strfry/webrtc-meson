libcongestion_controller_files = files(
    'include/network_changed_observer.h',
    'include/receive_side_congestion_controller.h',
    'include/send_side_congestion_controller.h',
    'include/send_side_congestion_controller_interface.h',
    'probe_controller.cc',
    'probe_controller.h',
    'receive_side_congestion_controller.cc',
    'send_side_congestion_controller.cc',

    # transport_feedback
    'send_time_history.cc',
    'send_time_history.h',
    'transport_feedback_adapter.cc',
    'transport_feedback_adapter.h',

    # estimators
    'acknowledged_bitrate_estimator.cc',
    'acknowledged_bitrate_estimator.h',
    'bitrate_estimator.cc',
    'bitrate_estimator.h',
    'delay_increase_detector_interface.h',
    'median_slope_estimator.cc',
    'median_slope_estimator.h',
    'probe_bitrate_estimator.cc',
    'probe_bitrate_estimator.h',
    'trendline_estimator.cc',
    'trendline_estimator.h',

    # delay_based_bwe
    'delay_based_bwe.cc',
    'delay_based_bwe.h',
)

# modules/congestion_controller/rtp
libcongestion_controller_files += files(
    'rtp/include/send_side_congestion_controller.h',
    'rtp/pacer_controller.cc',
    'rtp/pacer_controller.h',
    'rtp/send_side_congestion_controller.cc',

    # transport_feedback
    'rtp/send_time_history.cc',
    'rtp/send_time_history.h',
    'rtp/transport_feedback_adapter.cc',
    'rtp/transport_feedback_adapter.h',
)

# modules/congestion_controller/network_control
libcongestion_controller_files += files(
    'network_control/include/network_control.h',
    'network_control/include/network_types.h',
    'network_control/include/network_units.h',
    'network_control/include/network_units_to_string.h',
    'network_control/network_types.cc',
    'network_control/network_units.cc',
    'network_control/network_units_to_string.cc',
)

# modules/congestion_controller/goog_cc
libcongestion_controller_files += files(
    'goog_cc/alr_detector.cc',
    'goog_cc/alr_detector.h',
    'goog_cc/goog_cc_factory.cc',
    'goog_cc/goog_cc_network_control.cc',
    'goog_cc/goog_cc_network_control.h',
    'goog_cc/include/goog_cc_factory.h',
    'goog_cc/probe_controller.cc',
    'goog_cc/probe_controller.h',

    # estimators
    'goog_cc/acknowledged_bitrate_estimator.cc',
    'goog_cc/acknowledged_bitrate_estimator.h',
    'goog_cc/bitrate_estimator.cc',
    'goog_cc/bitrate_estimator.h',
    'goog_cc/delay_increase_detector_interface.h',
    'goog_cc/median_slope_estimator.cc',
    'goog_cc/median_slope_estimator.h',
    'goog_cc/probe_bitrate_estimator.cc',
    'goog_cc/probe_bitrate_estimator.h',
    'goog_cc/trendline_estimator.cc',
    'goog_cc/trendline_estimator.h',

    # delay_based_bwe
    'goog_cc/delay_based_bwe.cc',
    'goog_cc/delay_based_bwe.h',
)

libcongestion_controller = static_library(
  'congestion_controller',
  libcongestion_controller_files,
  include_directories : [inc_common],
  cpp_args : internal_args,
)

all_libraries += libcongestion_controller
