FROM alpine:3.4
RUN mkdir /lib64 && ln -s /lib/libc.musl-x86_64.so.1 /lib64/ld-linux-x86-64.so.2
ADD tsdbrelay /opt/bin/tsdbrelay
ENV PATH /opt/bin:$PATH
CMD ["tsdbrelay","-b bosun:8101 -t opentsdb:4243"]
