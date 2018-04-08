librtc_base_files = files(
    'asyncinvoker-inl.h',
    'asyncinvoker.cc',
    'asyncinvoker.h',
    'asyncpacketsocket.cc',
    'asyncpacketsocket.h',
    'asyncresolverinterface.cc',
    'asyncresolverinterface.h',
    'asyncsocket.cc',
    'asyncsocket.h',
    'asynctcpsocket.cc',
    'asynctcpsocket.h',
    'asyncudpsocket.cc',
    'asyncudpsocket.h',
    'crc32.cc',
    'crc32.h',
    'cryptstring.cc',
    'cryptstring.h',
    'data_rate_limiter.cc',
    'data_rate_limiter.h',
    'dscp.h',
    'filerotatingstream.cc',
    'filerotatingstream.h',
    'fileutils.cc',
    'fileutils.h',
    'gunit_prod.h',
    'helpers.cc',
    'helpers.h',
    'httpcommon-inl.h',
    'httpcommon.cc',
    'httpcommon.h',
    'ipaddress.cc',
    'ipaddress.h',
    'keep_ref_until_done.h',
    'messagedigest.cc',
    'messagedigest.h',
    'messagehandler.cc',
    'messagehandler.h',
    'messagequeue.cc',
    'messagequeue.h',
    'nethelper.cc',
    'nethelper.h',
    'nethelpers.cc',
    'nethelpers.h',
    'network.cc',
    'network.h',
    'network_constants.h',
    'networkmonitor.cc',
    'networkmonitor.h',
    'networkroute.h',
    'nullsocketserver.cc',
    'nullsocketserver.h',
    'openssl.h',
    'openssladapter.cc',
    'openssladapter.h',
    'opensslcommon.cc',
    'opensslcommon.h',
    'openssldigest.cc',
    'openssldigest.h',
    'opensslidentity.cc',
    'opensslidentity.h',
    'opensslsessioncache.cc',
    'opensslsessioncache.h',
    'opensslstreamadapter.cc',
    'opensslstreamadapter.h',
    'physicalsocketserver.cc',
    'physicalsocketserver.h',
    'proxyinfo.cc',
    'proxyinfo.h',
    'rtccertificate.cc',
    'rtccertificate.h',
    'rtccertificategenerator.cc',
    'rtccertificategenerator.h',
    'signalthread.cc',
    'signalthread.h',
    'sigslot.cc',
    'sigslot.h',
    'sigslotrepeater.h',
    'socket.h',
    'socketadapters.cc',
    'socketadapters.h',
    'socketaddress.cc',
    'socketaddress.h',
    'socketaddresspair.cc',
    'socketaddresspair.h',
    'socketfactory.h',
    'socketserver.h',
    'socketstream.cc',
    'socketstream.h',
    'ssladapter.cc',
    'ssladapter.h',
    'sslfingerprint.cc',
    'sslfingerprint.h',
    'sslidentity.cc',
    'sslidentity.h',
    'sslstreamadapter.cc',
    'sslstreamadapter.h',
    'stream.cc',
    'stream.h',
    'thread.cc',
    'thread.h',


    # rtc_base_approved_generic
    'base64.cc',
    'base64.h',
    'bind.h',
    'bitbuffer.cc',
    'bitbuffer.h',
    'bitrateallocationstrategy.cc',
    'bitrateallocationstrategy.h',
    'buffer.h',
    'bufferqueue.cc',
    'bufferqueue.h',
    'bytebuffer.cc',
    'bytebuffer.h',
    'byteorder.h',
    'copyonwritebuffer.cc',
    'copyonwritebuffer.h',
    'event_tracer.cc',
    'event_tracer.h',
    'file.cc',
    'file.h',
    'flags.cc',
    'flags.h',
    'function_view.h',
    'ignore_wundef.h',
    'location.cc',
    'location.h',
    'numerics/histogram_percentile_counter.cc',
    'numerics/histogram_percentile_counter.h',
    'numerics/mod_ops.h',
    'numerics/moving_max_counter.h',
    'onetimeevent.h',
    'pathutils.cc',
    'pathutils.h',
    'platform_file.cc',
    'platform_file.h',
    'race_checker.cc',
    'race_checker.h',
    'random.cc',
    'random.h',
    'rate_statistics.cc',
    'rate_statistics.h',
    'ratetracker.cc',
    'ratetracker.h',
    'string_to_number.cc',
    'string_to_number.h',
    'swap_queue.h',
    'template_util.h',
    'timestampaligner.cc',
    'timestampaligner.h',
    'trace_event.h',
    'zero_memory.cc',
    'zero_memory.h',
)


# Random stuff that is not part of rtc_base in GN
librtc_base_files += files(
    'location.cc',
    'location.h',

    # platform_thread_types
    'platform_thread_types.cc',
    'platform_thread_types.h',

    # criticalsection
    'criticalsection.cc',
    'criticalsection.h',

    # platform_thread
    'platform_thread.cc',
    'platform_thread.h',

    # rtc_event
    'event.cc',
    'event.h',

    # logging
    'logging.cc',
    'logging.h',

    # thread_checker
    'thread_checker.h',
    'thread_checker_impl.cc',
    'thread_checker_impl.h',    

    # checks
    'checks.cc',
    'checks.h',
    
    # rate_limiter
    'rate_limiter.cc',
    'rate_limiter.h',

    # timeutils
    'timeutils.cc',
    'timeutils.h',

    # stringutils
    'stringencode.cc',
    'stringencode.h',
    'strings/string_builder.cc',
    'strings/string_builder.h',
    'stringutils.cc',
    'stringutils.h',

    # audio_format_to_string
    'strings/audio_format_to_string.cc',
    'strings/audio_format_to_string.h',
    
    # sequenced_task_checker
    'sequenced_task_checker.h',
    'sequenced_task_checker_impl.cc',
    'sequenced_task_checker_impl.h',

    # weak_ptr
    'weak_ptr.cc',
    'weak_ptr.h',

    # rtc_numerics
    'numerics/exp_filter.cc',
    'numerics/exp_filter.h',
    'numerics/moving_median_filter.h',
    'numerics/percentile_filter.h',
    'numerics/sequence_number_util.h',

    # rtc_json
    #'json.cc',
    #'json.h',
)

# rtc_base/system
librtc_base_files += files(
    'system/file_wrapper.cc',
    'system/file_wrapper.h',
)

# rtc_base/memory
librtc_base_files += files(
    'memory/aligned_malloc.cc',
    'memory/aligned_malloc.h',
)

# rtc_base/time
librtc_base_files += files(
    'time/timestamp_extrapolator.cc',
    'time/timestamp_extrapolator.h',
)

# rtc_base/experiments
librtc_base_files += files(
    'experiments/alr_experiment.cc',
    'experiments/alr_experiment.h',
)

# Platform-dependent stuff, to improve for non-Linux
librtc_base_files += files(
    'file_posix.cc',
    'synchronization/rw_lock_posix.cc',
    'synchronization/rw_lock_posix.h',
    'synchronization/rw_lock_posix.cc',
    'synchronization/rw_lock_posix.h',
    'synchronization/rw_lock_wrapper.cc',
    'synchronization/rw_lock_wrapper.h',

    'ifaddrs_converter.cc',
    'ifaddrs_converter.h',
    'unixfilesystem.cc',
    'unixfilesystem.h',

    'task_queue_libevent.cc',
    'task_queue_posix.cc',
    'task_queue_posix.h',
)

librtc_base = static_library(
  'rtc_base',
  librtc_base_files,
  include_directories : [inc_common],
  cpp_args: internal_args,
)

all_libraries += librtc_base
