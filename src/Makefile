CFLAGS = -O3 -march=native
LDLIBS = -lm -lpng -ljpeg -ltiff -lX11

OBJ = jmgs.o iio.o ftr.o
BIN = jmgs
EMS = jmgs.html

$(BIN) : $(OBJ)

clean : ; rm -f $(BIN) $(OBJ) $(EMS)

EMSOPT = -s SINGLE_FILE=1 -s ALLOW_MEMORY_GROWTH=1
%.html : %.c ftr_emscripten.c
	emcc $(EMSOPT) $^ -o $@
