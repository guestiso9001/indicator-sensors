plugindir = $(libdir)/$(PACKAGE)/plugins/nvidia

INCLUDES = \
	-I$(top_srcdir) 	\
	$(GLIB_CFLAGS)		\
	$(GTK_CFLAGS)		\
	$(APPINDICATOR_CFLAGS)	\
	$(LIBPEAS_CFLAGS) 	\
	$(NVIDIA_CFLAGS)

plugin_LTLIBRARIES = libnvidia.la

libnvidia_la_SOURCES = \
	is-nvidia-plugin.h		\
	is-nvidia-plugin.c

libnvidia_la_LDFLAGS = $(PLUGIN_LIBTOOL_FLAGS)
libnvidia_la_LIBADD  = 	\
	$(GLIB_LIBS)		\
	$(GTK_LIBS) 		\
	$(APPINDICATOR_LIBS)	\
	$(LIBPEAS_LIBS) 	\
	$(NVIDIA_LIBS)

plugin_DATA = nvidia.plugin

EXTRA_DIST = $(plugin_DATA)
