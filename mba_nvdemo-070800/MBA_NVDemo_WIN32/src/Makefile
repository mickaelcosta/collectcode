#############################################################################
# Makefile for building mba_nvdemo
# Generated by tmake at 12:05, 2000/07/08
#     Project: ENVMAP
#    Template: app
#############################################################################

####### Compiler, tools and options

CC	=	gcc
CXX	=	g++
CFLAGS	=	-pipe -Wall -W -O2
CXXFLAGS=	-pipe -Wall -W -O2
INCPATH	=	-I../include -I../glpng/include -I/usr/X11R6/include
LINK	=	g++
LFLAGS	=	
LIBS	=	-L../glpng/lib -L/usr/X11R6/lib -lGL -lGLU -lglut -lglpng -lXi -lXmu -lXext -lX11 -lm
MOC	=	$(QTDIR)/bin/moc

TAR	=	tar -cf
GZIP	=	gzip -9f

####### Files

HEADERS =	RglPrims.h \
		room.h \
		reflect.h \
		mmath.h \
		main.h
SOURCES =	RglPrims.cpp \
		room.cpp \
		reflect.cpp \
		mmath.cpp \
		main.cpp
OBJECTS =	RglPrims.o \
		room.o \
		reflect.o \
		mmath.o \
		main.o
SRCMOC	=	
OBJMOC	=	
DIST	=	
TARGET	=	mba_nvdemo

####### Implicit rules

.SUFFIXES: .cpp .cxx .cc .C .c

.cpp.o:
	$(CXX) -c $(CXXFLAGS) $(INCPATH) -o $@ $<

.cxx.o:
	$(CXX) -c $(CXXFLAGS) $(INCPATH) -o $@ $<

.cc.o:
	$(CXX) -c $(CXXFLAGS) $(INCPATH) -o $@ $<

.C.o:
	$(CXX) -c $(CXXFLAGS) $(INCPATH) -o $@ $<

.c.o:
	$(CC) -c $(CFLAGS) $(INCPATH) -o $@ $<

####### Build rules

all: $(TARGET)

$(TARGET): $(OBJECTS) $(OBJMOC) 
	$(LINK) $(LFLAGS) -o $(TARGET) $(OBJECTS) $(OBJMOC) $(LIBS)

moc: $(SRCMOC)

tmake: Makefile

Makefile: ENVMAP.pro
	tmake ENVMAP.pro -o Makefile

dist:
	$(TAR) ENVMAP.tar ENVMAP.pro $(SOURCES) $(HEADERS) $(DIST)
	$(GZIP) ENVMAP.tar

clean:
	-rm -f $(OBJECTS) $(OBJMOC) $(SRCMOC) $(TARGET)
	-rm -f *~ core
	-rm -f *.bck

####### Compile

RglPrims.o: RglPrims.cpp \
		RglPrims.h \
		mmath.h \
		winstuff.h

room.o: room.cpp \
		room.h \
		mmath.h \
		winstuff.h \
		RglPrims.h

reflect.o: reflect.cpp \
		reflect.h \
		winstuff.h \
		RglPrims.h \
		mmath.h

mmath.o: mmath.cpp \
		mmath.h \
		winstuff.h

main.o: main.cpp \
		winstuff.h \
		main.h \
		mmath.h \
		room.h \
		reflect.h

