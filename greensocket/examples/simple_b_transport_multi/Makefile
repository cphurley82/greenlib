# enabling SystemC2.1 automatically changes 
# includes and compiler flags in Makefile.defs
#SYSTEMC21V1 = yes

CC     = g++
OPT    = -O3
DEBUG  = -g -Wall
OTHER  = -Wno-deprecated -I../common
CPPFLAGS = $(OPT) $(OTHER) 
# CPPFLAGS = $(DEBUG) $(OTHER)


MODULE = simple_b_transport_top
SRCS = $(wildcard ../common/*.cpp) $(wildcard ./*.cpp)
OBJS = $(SRCS:.cpp=.o)

-include ../Makefile.gspm
include ../Makefile.defs

all: $(EXE)

