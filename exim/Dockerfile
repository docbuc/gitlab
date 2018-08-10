FROM alpine:3.7
RUN apk --no-cache add exim
COPY docker-exim.conf /etc/exim/exim.conf
EXPOSE 25
ENTRYPOINT ["/usr/sbin/exim"]
CMD ["-bdf", "-q15m"]
