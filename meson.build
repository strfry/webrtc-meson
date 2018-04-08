project('webrtc', ['c', 'cpp'], version : '1', license : 'BSD',
    default_options : ['c_std=c99', 'cpp_std=c++11'])


# Defines that are needed for every library including webrtc headers
external_args = [
  '-DWEBRTC_POSIX',
  '-DWEBRTC_LINUX',
]

# Internal defines, should be more configurable. Maybe split out to subdirs like in modules/audio_coding?
internal_args = external_args + [
  '-DUSE_BUILTIN_SW_CODECS',
  '-DWEBRTC_CODEC_ISAC',
  '-DWEBRTC_USE_BUILTIN_ISAC_FLOAT',
  '-DHAVE_WEBRTC_VIDEO',
  '-DHAVE_WEBRTC_VOICE',
  '-DWEBRTC_INTELLIGIBILITY_ENHANCER=1', # This is not the GN default
  '-DWEBRTC_OPUS_SUPPORT_120MS_PTIME=1',
  '-DWEBRTC_OPUS_VARIABLE_COMPLEXITY=0',
  '-DWEBRTC_APM_DEBUG_DUMP=0',
  '-DWEBRTC_NS_FLOAT', # replace with WEBRTC_NS_FIXED on some platforms?
  '-DWEBRTC_INCLUDE_INTERNAL_AUDIO_DEVICE',
  '-DWEBRTC_INITIALIZE_FFMPEG',
]

#with_h264 = get_option('openh264') # Figure out how to use options
with_h264 = true

if not with_h264
    error('Building without OpenH264 not implemented, yet')
else
    internal_args += '-DWEBRTC_USE_H264'
endif

#dep_srtp = dependency('libsrtp2', version: '>=2.1.0') # TODO: Can we check if it was build with --enable-openssl?
sub_srtp = subproject('libsrtp')
dep_srtp = sub_srtp.get_variable('libsrtp_dep')

# Work around the fact that WebRTC includes libsrtp's internal headers:
inc_srtp_priv = sub_srtp.get_variable('internal_inc')
inc_srtp_conf = sub_srtp.get_variable('config_inc')

dep_dl = meson.get_compiler('cpp').find_library('dl', required: false)

dep_thread = dependency('threads')
dep_ssl= dependency('openssl')
dep_event = dependency('libevent', version: '>=2.0')

dep_json = dependency('jsoncpp')

dep_alsa = dependency('alsa')
dep_opus = dependency('opus')
dep_vpx = dependency('vpx', version: '>=1.7.0')
dep_h264 = dependency('openh264')
dep_avcodec = dependency('libavcodec')
dep_avutil = dependency('libavutil')
dep_avformat = dependency('libavformat')

sub_yuv = subproject('libyuv')
dep_yuv = sub_yuv.get_variable('libyuv_dep')
inc_yuv = sub_yuv.get_variable('libyuv_inc')

inc_external = [inc_yuv, include_directories('.')]
inc_internal = [inc_srtp_priv, inc_srtp_conf]
inc_common = [inc_external, inc_internal]

all_libraries = []

subdir('common_audio')
subdir('common_video')
subdir('logging')
subdir('media')
subdir('modules/audio_coding')
subdir('modules/audio_device')
subdir('modules/audio_processing')
subdir('modules/pacing')
subdir('modules/rtp_rtcp')
subdir('modules/video_capture')
subdir('modules/video_coding')
subdir('p2p')
subdir('pc')
subdir('rtc_base')
subdir('system_wrappers')
subdir('stats')
subdir('video')

subdir('api')
subdir('call')
subdir('modules/audio_mixer')
subdir('audio')
subdir('modules/utility')
subdir('modules/congestion_controller')
subdir('modules/bitrate_controller')
subdir('modules/remote_bitrate_estimator')
subdir('test')

libwebrtc_full_files = files(
  'common_types.cc',
  'common_types.h',
)

deps = [dep_dl, dep_thread, dep_ssl, dep_srtp, dep_opus,
    dep_vpx, dep_h264, dep_avcodec, dep_avutil, dep_avformat, 
    dep_event, dep_json, dep_yuv, dep_alsa]

webrtc_lib = library(
    'webrtc',
    libwebrtc_full_files,
    link_whole: all_libraries,
    cpp_args: internal_args,
    include_directories: inc_common,
    dependencies : deps,
)

webrtc_dep = declare_dependency(
    include_directories: inc_external,
    compile_args: external_args,
    link_with: webrtc_lib,
    dependencies: deps,
)
