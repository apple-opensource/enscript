#
# Makefile for scripts directory.
# Copyright (c) 1996, 1997 Markku Rossi
#
# Author: Markku Rossi <mtr@iki.fi>
#

#
# This file is part of GNU enscript.
#
# This program is free software; you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation; either version 2, or (at your option)
# any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program; see the file COPYING.  If not, write to
# the Free Software Foundation, 59 Temple Place - Suite 330,
# Boston, MA 02111-1307, USA.
#

man_MANS = diffpp.1 sliceprint.1

bin_SCRIPTS = diffpp sliceprint

diffpp: $(srcdir)/diffpp.in
	sed 's%@PERLPROG@%@PERL@%g' $(srcdir)/diffpp.in >diffpp

sliceprint: $(srcdir)/sliceprint.in
	sed 's%@PERLPROG@%@PERL@%g' $(srcdir)/sliceprint.in >sliceprint

EXTRA_DIST = diffpp.in sliceprint.in $(man_MANS)

CLEANFILES = diffpp sliceprint
