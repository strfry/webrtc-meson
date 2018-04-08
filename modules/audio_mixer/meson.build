libaudio_mixer_files = files(
    'audio_frame_manipulator.cc',
    'audio_frame_manipulator.h',
    
    # audio_mixer_impl
    'audio_mixer_impl.cc',
    'audio_mixer_impl.h',
    'default_output_rate_calculator.cc',
    'default_output_rate_calculator.h',
    'frame_combiner.cc',
    'frame_combiner.h',
    'output_rate_calculator.h',
    'audio_mixer_impl.h',
    'default_output_rate_calculator.h',  # For creating a mixer with limiter disabled.
    'frame_combiner.h',
)

libaudio_mixer = static_library(
  'audio_mixer',
  libaudio_mixer_files,
  include_directories : [inc_common],
  cpp_args: internal_args,
)

all_libraries += libaudio_mixer
