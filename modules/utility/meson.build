libutility_files = files(
    #'include/helpers_android.h',
    #'include/jvm_android.h',
    'include/process_thread.h',
    #'source/helpers_android.cc',
    #'source/jvm_android.cc',
    'source/process_thread_impl.cc',
    'source/process_thread_impl.h',
)


libutility = static_library(
  'utility',
  libutility_files,
  include_directories : [inc_common],
  cpp_args: internal_args,
)

all_libraries += libutility
