# Basic
yaml_build = custom_target(
  'basic.yml',
  input: 'basic.yml.in',
  output: 'basic.yml',
  console: true,
  install: true,
  install_dir: sysconfdir / 'icicle',
  command: [
    ymlconvert,
    '@INPUT@',
    '@OUTPUT@'
  ]
)

# Advanced
yaml_build = custom_target(
  'advanced.yml',
  input: 'advanced.yml.in',
  output: 'advanced.yml',
  console: true,
  install: true,
  install_dir: sysconfdir / 'icicle',
  command: [
    ymlconvert,
    '@INPUT@',
    '@OUTPUT@'
  ]
)

install_data('config.yml', install_dir : sysconfdir / 'icicle')

install_subdir('basic', install_dir : sysconfdir / 'icicle')
install_subdir('advanced', install_dir : sysconfdir / 'icicle')

subdir('branding/snowflakeos')
