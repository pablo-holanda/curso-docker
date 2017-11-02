FROM nginx:stable

# Packages
RUN apt-get update && \
  DEBIAN_FRONTEND=noninteractive apt-get install -y \
    locales \
    certbot \
&& rm -r /var/lib/apt/lists/*

# To further increase security, you should also generate a strong Diffie-Hellman group.
# Generate a 2048-bit group

RUN openssl dhparam -out /etc/ssl/certs/dhparam.pem 2048

RUN touch /usr/share/locale/locale.alias && echo "pt_BR.UTF-8 UTF-8" > /etc/locale.gen && locale-gen

ENV LANG=pt_BR.UTF-8
ENV LANGUAGE=pt_BR:pt
ENV LC_ALL=pt_BR.UTF-8
