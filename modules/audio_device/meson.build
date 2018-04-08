libaudio_device_files = files(

    # audio_device_buffer
    'audio_device_buffer.cc',
    'audio_device_buffer.h',
    'audio_device_config.h',
    'fine_audio_buffer.cc',
    'fine_audio_buffer.h',

    # audio_device_generic
    'audio_device_generic.cc',
    'audio_device_generic.h',

    # audio_device_impl
    'dummy/audio_device_dummy.cc',
    'dummy/audio_device_dummy.h',
    'dummy/file_audio_device.cc',
    'dummy/file_audio_device.h',
    'include/fake_audio_device.h',
    'include/test_audio_device.cc',
    'include/test_audio_device.h',
    'audio_device_data_observer.cc',
    'audio_device_impl.cc',
    'audio_device_impl.h',
    'include/audio_device_data_observer.h',

    # TODO: Platform switch
    'linux/alsasymboltable_linux.cc',
    'linux/alsasymboltable_linux.h',
    'linux/audio_device_alsa_linux.cc',
    'linux/audio_device_alsa_linux.h',
    'linux/audio_mixer_manager_alsa_linux.cc',
    'linux/audio_mixer_manager_alsa_linux.h',
    'linux/latebindingsymboltable_linux.cc',
    'linux/latebindingsymboltable_linux.h',

    # TODO: Pulseaudio support?
)

libaudio_device = static_library(
  'audio_device',
  libaudio_device_files,
  override_options: 'cpp_std=gnu++11', # enable GNU extensions because of typeof() macro
  include_directories : [inc_common],
  cpp_args: internal_args + ['-DLINUX_ALSA'],
)

all_libraries += libaudio_device
