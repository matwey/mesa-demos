# Copyright © 2010 Intel Corporation
#
# Permission is hereby granted, free of charge, to any person obtaining a
# copy of this software and associated documentation files (the "Software"),
# to deal in the Software without restriction, including without limitation
# the rights to use, copy, modify, merge, publish, distribute, sublicense,
# and/or sell copies of the Software, and to permit persons to whom the
# Software is furnished to do so, subject to the following conditions:
#
# The above copyright notice and this permission notice (including the next
# paragraph) shall be included in all copies or substantial portions of the
# Software.
#
# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.  IN NO EVENT SHALL
# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
# IN THE SOFTWARE.
#
# Authors:
#    Eric Anholt <eric@anholt.net>

# These programs aren't intended to be included with the normal distro.
# They're not too interesting but they're good for testing.

AM_CFLAGS = \
	$(DEMO_CFLAGS) \
	$(EGL_CFLAGS) \
	$(GLESV1_CFLAGS) \
	-I$(top_srcdir)/src/egl/eglut \
	-I$(top_srcdir)/src/util
AM_LDFLAGS = \
	$(DEMO_LIBS) \
	$(EGL_LIBS) \
	$(GLESV1_LIBS)

if HAVE_EGL
if HAVE_GLESV1
noinst_PROGRAMS = \
	bindtex \
	drawtex_screen \
	drawtex_x11 \
	es1_info \
	gears_screen \
	gears_x11 \
	msaa \
	pbuffer\
	render_tex \
	torus_screen \
	torus_x11 \
	tri_screen \
	tri_x11 \
	two_win
endif
endif

drawtex_screen_SOURCES = drawtex.c
gears_screen_SOURCES = gears.c
torus_screen_SOURCES = torus.c
tri_screen_SOURCES = tri.c

drawtex_x11_SOURCES = drawtex.c
gears_x11_SOURCES = gears.c
torus_x11_SOURCES = torus.c
tri_x11_SOURCES = tri.c

drawtex_screen_LDADD = ../eglut/libeglut_screen.la
gears_screen_LDADD = ../eglut/libeglut_screen.la
torus_screen_LDADD = ../eglut/libeglut_screen.la
tri_screen_LDADD = ../eglut/libeglut_screen.la

drawtex_x11_LDADD = ../eglut/libeglut_x11.la
gears_x11_LDADD = ../eglut/libeglut_x11.la
torus_x11_LDADD = ../eglut/libeglut_x11.la
tri_x11_LDADD = ../eglut/libeglut_x11.la