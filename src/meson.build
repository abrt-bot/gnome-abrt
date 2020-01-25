i18n.merge_file(
  input: 'org.freedesktop.GnomeAbrt.appdata.xml.in',
  install: true,
  install_dir: join_paths(datadir, 'metainfo'),
  output: 'org.freedesktop.GnomeAbrt.appdata.xml',
  po_dir: join_paths(meson.source_root(), 'po'),
  type: 'xml'
)

i18n.merge_file(
  input: 'org.freedesktop.GnomeAbrt.desktop.in',
  install: true,
  install_dir: join_paths(datadir, 'applications'),
  output: 'org.freedesktop.GnomeAbrt.desktop',
  po_dir: join_paths(meson.source_root(), 'po'),
  type: 'desktop'
)

gnome_abrt_main = configure_file(
  copy: true,
  input: 'gnome-abrt',
  install: true,
  install_dir: bindir,
  output: 'gnome-abrt',
)

subdir('gnome_abrt')
