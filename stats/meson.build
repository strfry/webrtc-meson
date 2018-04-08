libstats_files = files(
    'rtcstats.cc',
    'rtcstats_objects.cc',
    'rtcstatsreport.cc',
)



libstats = static_library(
  'stats',
  libstats_files,
  include_directories : [inc_common],
)

all_libraries += libstats
