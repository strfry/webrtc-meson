libmedia_base_files = files(
    'base/adaptedvideotracksource.cc',
    'base/adaptedvideotracksource.h',
    'base/audiosource.h',
    'base/codec.cc',
    'base/codec.h',
    'base/cryptoparams.h',
    'base/device.h',
    'base/mediachannel.h',
    'base/mediaconstants.cc',
    'base/mediaconstants.h',
    'base/mediaengine.cc',
    'base/mediaengine.h',
    'base/rtpdataengine.cc',
    'base/rtpdataengine.h',
    'base/rtputils.cc',
    'base/rtputils.h',
    'base/streamparams.cc',
    'base/streamparams.h',
    'base/turnutils.cc',
    'base/turnutils.h',
    'base/videoadapter.cc',
    'base/videoadapter.h',
    'base/videobroadcaster.cc',
    'base/videobroadcaster.h',
    'base/videocapturer.cc',
    'base/videocapturer.h',
    'base/videocapturerfactory.h',
    'base/videocommon.cc',
    'base/videocommon.h',
    'base/videosourcebase.cc',
    'base/videosourcebase.h',

    # rtc_h264_profile_id
    'base/h264_profile_level_id.cc',
    'base/h264_profile_level_id.h',


    # rtc_data
    'sctp/noop.cc'
)

libmedia_engine_files = files(
    # rtc_audio_video
    'engine/adm_helpers.cc',
    'engine/adm_helpers.h',
    'engine/apm_helpers.cc',
    'engine/apm_helpers.h',
    'engine/nullwebrtcvideoengine.h',
    'engine/payload_type_mapper.cc',
    'engine/payload_type_mapper.h',
    'engine/simulcast.cc',
    'engine/simulcast.h',
    'engine/webrtcmediaengine.cc',
    'engine/webrtcmediaengine.h',
    'engine/webrtcvideocapturer.cc',
    'engine/webrtcvideocapturer.h',
    'engine/webrtcvideocapturerfactory.cc',
    'engine/webrtcvideocapturerfactory.h',
    'engine/webrtcvideodecoderfactory.cc',
    'engine/webrtcvideodecoderfactory.h',
    'engine/webrtcvideoencoderfactory.cc',
    'engine/webrtcvideoencoderfactory.h',
    'engine/webrtcvideoengine.cc',
    'engine/webrtcvideoengine.h',
    'engine/webrtcvoiceengine.cc',
    'engine/webrtcvoiceengine.h',

    # rtc_constants
    'engine/constants.cc',
    'engine/constants.h',

    # rtc_internal_video_codecs
    'engine/convert_legacy_video_factory.cc',
    'engine/convert_legacy_video_factory.h',
    'engine/internaldecoderfactory.cc',
    'engine/internaldecoderfactory.h',
    'engine/internalencoderfactory.cc',
    'engine/internalencoderfactory.h',
    'engine/multiplexcodecfactory.cc',
    'engine/multiplexcodecfactory.h',
    'engine/scopedvideodecoder.cc',
    'engine/scopedvideodecoder.h',
    'engine/scopedvideoencoder.cc',
    'engine/scopedvideoencoder.h',
    'engine/simulcast_encoder_adapter.cc',
    'engine/simulcast_encoder_adapter.h',
    'engine/vp8_encoder_simulcast_proxy.cc',
    'engine/vp8_encoder_simulcast_proxy.h',
    'engine/webrtcvideodecoderfactory.h',
    'engine/webrtcvideoencoderfactory.h',

    # rtc_software_fallback_wrappers
    'engine/videodecodersoftwarefallbackwrapper.cc',
    'engine/videodecodersoftwarefallbackwrapper.h',
    'engine/videoencodersoftwarefallbackwrapper.cc',
    'engine/videoencodersoftwarefallbackwrapper.h',
)

libmedia_base = static_library(
  'media_base',
  libmedia_base_files,
  include_directories : [inc_common],
  cpp_args: internal_args,
)

libmedia_engine = static_library(
  'media_engine',
  libmedia_engine_files,
  include_directories : [inc_common],
  cpp_args: internal_args,
)

all_libraries += [libmedia_base, libmedia_engine]
