gtk2_dep = dependency('gtk+-2.0', required: get_option('gtk2'))

if gtk2_dep.found()
  shared_library('kime-gtk2',
    '../gtk3/src/gtk.c',
    '../gtk3/src/immodule.c',
    '../gtk3/src/str_buf.c',
    dependencies: [gtk2_dep, kime_engine_dep],
    install: true,
    install_dir: get_option('libdir') / 'gtk-2.0' / '2.10.0' / 'immodules',
  )
endif
