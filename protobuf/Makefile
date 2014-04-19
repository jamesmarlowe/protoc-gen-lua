SRC=pb.c

TARGET=pb.so
CFLAGS=`pkg-config --cflags /usr/local/openresty/luajit/lib/pkgconfig/luajit.pc`  -std=gnu99
LDFLAGS=`pkg-config --libs /usr/local/openresty/luajit/lib/pkgconfig/luajit.pc`

all:$(TARGET)

$(TARGET):$(SRC)
	gcc -O3 -shared -fPIC $(SRC) $(CFLAGS) $(LDFLAGS) -o $@
