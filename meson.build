project('ganash', 'c',
        version: '0.1.0',
        meson_version: '>= 0.40.0',
)

i18n = import('i18n')

config_h = configuration_data()
config_h.set_quoted('GETTEXT_PACKAGE', 'ganash')
config_h.set_quoted('LOCALEDIR', join_paths(get_option('prefix'), get_option('localedir')))
configure_file(
  output: 'ganash-config.h',
  configuration: config_h,
)
add_project_arguments([
  '-I' + meson.build_root(),
], language: 'c')

