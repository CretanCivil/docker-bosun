FROM alpine:3.4
RUN mkdir /lib64 && ln -s /lib/libc.musl-x86_64.so.1 /lib64/ld-linux-x86-64.so.2
ADD bosun /opt/bin/bosun
ADD bosun.toml  /etc/bosun/bosun.toml
ADD dev.sample.conf  /etc/bosun/dev.sample.conf
ENV PATH /opt/bin:$PATH
CMD ["bosun"]