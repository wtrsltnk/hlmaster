## Makefile for hlmaster
## Copyright (C) 2001 Silvan Minghetti
##
## This program is free software; you can redistribute it and/or modify
## it under the terms of the GNU General Public License as published by
## the Free Software Foundation; either version 2, or (at your option)
## any later version.
##
## This program is distributed in the hope that it will be useful,
## but WITHOUT ANY WARRANTY; without even the implied warranty of
## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
## GNU General Public License for more details.
##
## You should have received a copy of the GNU General Public License
## along with this program; if not, write to the Free Software
## Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA
## 02111-1307, USA.
##
## Process this file with automake to produce Makefile.in

bin_PROGRAMS = hlmaster
hlmaster_SOURCES = main.cpp \
                   HLMaster.cpp \
                   HLServerList.cpp \
                   HLServerFilterList.cpp \
                   HLInfoList.cpp


CXXFLAGS = -O2 -Wall
INCLUDES = -I../include -I../lib/pfc++/include

hlmaster_LDFLAGS = -s
hlmaster_LDADD = ../lib/pfc++/src/libpfc++.a
