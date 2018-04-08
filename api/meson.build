libapi_files=files(
    'candidate.cc',
    'candidate.h',
    'cryptoparams.h',
    'datachannelinterface.h',
    'dtmfsenderinterface.h',
    'jsep.cc',
    'jsep.h',
    'jsepicecandidate.h',
    'jsepsessiondescription.h',
    'mediaconstraintsinterface.cc',
    'mediaconstraintsinterface.h',
    'mediastreaminterface.cc',
    'mediastreaminterface.h',
    'mediastreamproxy.h',
    'mediastreamtrackproxy.h',
    'mediatypes.cc',
    'mediatypes.h',
    'notifier.h',
    'peerconnectionfactoryproxy.h',
    'peerconnectioninterface.h',
    'peerconnectionproxy.h',
    'proxy.cc',
    'proxy.h',
    'rtcerror.cc',
    'rtcerror.h',
    'rtp_headers.cc',
    'rtp_headers.h',
    'rtpparameters.cc',
    'rtpparameters.h',
    'rtpreceiverinterface.cc',
    'rtpreceiverinterface.h',
    'rtpsenderinterface.h',
    'rtptransceiverinterface.h',
    'setremotedescriptionobserverinterface.h',
    'statstypes.cc',
    'statstypes.h',
    'turncustomizer.h',
    'umametrics.cc',
    'umametrics.h',
    'videosourceinterface.cc',
    'videosourceinterface.h',
    'videosourceproxy.h',

    # ortc_api
    'ortc/mediadescription.cc',
    'ortc/mediadescription.h',
    'ortc/ortcfactoryinterface.h',
    'ortc/ortcrtpreceiverinterface.h',
    'ortc/ortcrtpsenderinterface.h',
    'ortc/packettransportinterface.h',
    'ortc/rtptransportcontrollerinterface.h',
    'ortc/rtptransportinterface.h',
    'ortc/sessiondescription.cc',
    'ortc/sessiondescription.h',
    'ortc/srtptransportinterface.h',
    'ortc/udptransportinterface.h',

    # rtc_stats_api
    'stats/rtcstats.h',
    'stats/rtcstats_objects.h',
    'stats/rtcstatscollectorcallback.h',
    'stats/rtcstatsreport.h',

    # video_frame_api
    'video/video_content_type.cc',
    'video/video_content_type.h',
    'video/video_frame.cc',
    'video/video_frame.h',
    'video/video_frame_buffer.cc',
    'video/video_frame_buffer.h',
    'video/video_rotation.h',
    'video/video_timing.cc',
    'video/video_timing.h',
    'videosinkinterface.h',

    # encoded_frame_api
    'video/encoded_frame.cc',
    'video/encoded_frame.h',

    # video_stream_decoder_create
    #'video/video_stream_decoder_create.cc',
    #'video/video_stream_decoder_create.h',

    # video_frame_api_i420
    'video/i420_buffer.cc',
    'video/i420_buffer.h',

    # optional
    'optional.cc',
    'optional.h',

    # transport_api
    'call/transport.cc',
    'call/transport.h',
)

# video_frame_api
libapi_files += files(
    'video/video_content_type.cc',
    'video/video_content_type.h',
    'video/video_frame.cc',
    'video/video_frame.h',
    'video/video_frame_buffer.cc',
    'video/video_frame_buffer.h',
    'video/video_rotation.h',
    'video/video_timing.cc',
    'video/video_timing.h',
    'videosinkinterface.h',
)

# audio api
libapi_files += files(
    'audio/audio_frame.cc',
    'audio/audio_frame.h',
    'audio/echo_canceller3_config.cc',
    'audio/echo_canceller3_config.h',
    'audio/echo_canceller3_factory.cc',
    'audio/echo_canceller3_factory.h',
    'audio/echo_control.h',
)

# audio_codecs api
libapi_files += files(
    'audio_codecs/audio_codec_pair_id.cc',
    'audio_codecs/audio_codec_pair_id.h',
    'audio_codecs/audio_decoder.cc',
    'audio_codecs/audio_decoder.h',
    'audio_codecs/audio_decoder_factory.cc',
    'audio_codecs/audio_decoder_factory.h',
    'audio_codecs/audio_decoder_factory_template.h',
    'audio_codecs/audio_encoder.cc',
    'audio_codecs/audio_encoder.h',
    'audio_codecs/audio_encoder_factory.cc',
    'audio_codecs/audio_encoder_factory.h',
    'audio_codecs/audio_encoder_factory_template.h',
    'audio_codecs/audio_format.cc',
    'audio_codecs/audio_format.h',

    # builtin_audio_decoder_factory
    'audio_codecs/builtin_audio_decoder_factory.cc',
    'audio_codecs/builtin_audio_decoder_factory.h',
    
    # builtin_audio_encoder_factory
    'audio_codecs/builtin_audio_encoder_factory.cc',
    'audio_codecs/builtin_audio_encoder_factory.h',
)

# audio_codecs/opus
libapi_files += files(
    # audio_encoder_opus_config
    'audio_codecs/opus/audio_encoder_opus_config.cc',
    'audio_codecs/opus/audio_encoder_opus_config.h',

    # audio_encoder_opus
    'audio_codecs/opus/audio_encoder_opus.cc',
    'audio_codecs/opus/audio_encoder_opus.h',

    # audio_decoder_opus
    'audio_codecs/opus/audio_decoder_opus.cc',
    'audio_codecs/opus/audio_decoder_opus.h',
)

# audio_codecs/L16
libapi_files += files(
    # audio_encoder_L16
    'audio_codecs/L16/audio_encoder_L16.cc',
    'audio_codecs/L16/audio_encoder_L16.h',

    # audio_decoder_L16
    'audio_codecs/L16/audio_decoder_L16.cc',
    'audio_codecs/L16/audio_decoder_L16.h',
)

# audio_codecs/g711
libapi_files += files(
    # audio_encoder_g711
    'audio_codecs/g711/audio_encoder_g711.cc',
    'audio_codecs/g711/audio_encoder_g711.h',

    # audio_decoder_g711
    'audio_codecs/g711/audio_decoder_g711.cc',
    'audio_codecs/g711/audio_decoder_g711.h',
)

# audio_codecs/g722
libapi_files += files(
    # audio_encoder_g722
    'audio_codecs/g722/audio_encoder_g722.cc',
    'audio_codecs/g722/audio_encoder_g722.h',

    # audio_decoder_g711
    'audio_codecs/g722/audio_decoder_g722.cc',
    'audio_codecs/g722/audio_decoder_g722.h',
)

# audio_codecs/isac
libapi_files += files(
    # audio_encoder_isac
    'audio_codecs/isac/audio_encoder_isac_float.cc',
    'audio_codecs/isac/audio_encoder_isac.h',

    # audio_decoder_g711
    'audio_codecs/isac/audio_decoder_isac_float.cc',
    'audio_codecs/isac/audio_decoder_isac.h',
)

# video codecs api
libapi_files += files(
    'video_codecs/sdp_video_format.cc',
    'video_codecs/sdp_video_format.h',
    'video_codecs/video_decoder.cc',
    'video_codecs/video_decoder.h',
    'video_codecs/video_decoder_factory.h',
    'video_codecs/video_encoder.cc',
    'video_codecs/video_encoder.h',
    'video_codecs/video_encoder_factory.h',
)

libapi = static_library(
  'jingle_peerconnection_api',
  libapi_files,
  dependencies: dep_opus,
  include_directories : [inc_common],
  cpp_args: internal_args,
)

all_libraries += libapi
