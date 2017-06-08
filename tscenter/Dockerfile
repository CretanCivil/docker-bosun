FROM alpine:3.4
RUN mkdir /lib64 && ln -s /lib/libc.musl-x86_64.so.1 /lib64/ld-linux-x86-64.so.2
ADD tscenter /opt/bin/tscenter
ENV PATH /opt/bin:$PATH
CMD ["tscenter"]


#docker run --rm -it -v "$PWD":/usr/src/myapp -w /usr/src/myapp alpine:3.4 sh