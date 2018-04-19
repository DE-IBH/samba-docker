FROM debian:stretch-slim

EXPOSE 445

RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install --no-install-recommends -y winbind libnss-winbind

ENTRYPOINT ["/usr/sbin/smbd"]
CMD ["-F", "-S"]
