
EOS_WARN_FLAGS = -Wall -Wuninitialized -Wwrite-strings
EOS_OPT_FLAGS =

AM_CFLAGS = $(EOS_WARN_FLAGS) $(EOS_OPT_FLAGS)
INCLUDES = \
	-I$(top_srcdir)/config \
	-I$(top_srcdir)/include \
	-I$(top_srcdir)/include/utils

INCLUDES += -I$(includedir) -I$(includedir)/eos -I$(includedir)/eut

# Makefile for the erm executable file
bin_PROGRAMS = select

#############################################################
select_SOURCES = \
        main.c

select_LDFLAGS = -static -L$(libdir)
select_LDADD = \
	-lsocket -lsys \
	-lutils -leut -leos \
	-lz -lpthread
	
