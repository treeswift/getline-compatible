project('getline-compatible', 'c',
  version : '1.0.0',
  default_options : ['warning_level=3'])

getline = shared_library('getline',
    files(
      'ggetws.c',
      'ggets.c',
      'getwline.c',
      'getline.c',
    ),
    install: true
  )

executable('test-getline',
    files('tests/test.c'),
    link_with: getline,
    install: true
  )

install_headers(
    files(
      'getline.h',
      'getwline.h',
      'ggets.h',
      'ggetws.h',
    ),
    subdir: 'getline',
  )
