licenses(['notice'])
package(default_visibility=['//visibility:public'])

cc_library(
    name = 'args',
    hdrs = [
        'args.hxx',
    ],
    includes = [
        '.',
    ],
    copts = [
        '-Wall',
        '-Werror',
        '-Wextra',
        '-Wshadow',
        '-Wunused-parameter',
        '-pedantic',
        '-std=gnu++11',
    ],
    linkopts = [
        '-lm',
    ],
)

cc_binary(
    name = 'gitlike',
    srcs = [
        'gitlike.cxx',
    ],
    deps = [
        ':args',
    ],
)

cc_test(
    name = 'test',
    srcs = [
        'test.cxx',
        'catch.hpp',
    ],
    deps = [
        ':args',
    ],
    testonly = 1,
)
