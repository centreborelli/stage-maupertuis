CFLAGS = -O3 -march=native
LDLIBS = -lm -lpng -ljpeg -ltiff -lX11

OBJ = jmgs.o iio.o ftr.o
BIN = jmgs

$(BIN) : $(OBJ)

clean : ; rm -f $(BIN) $(OBJ)
