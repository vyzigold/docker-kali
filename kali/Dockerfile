FROM kalilinux/kali-rolling:latest

RUN  echo "Acquire::https::Verify-Peer \"false\";" >> /etc/apt/apt.conf.d/01autoremove \
  && echo "Acquire::https::Verify-Host \"false\";" >> /etc/apt/apt.conf.d/01autoremove \
  && cat /etc/apt/apt.conf.d/* \
  && apt-get update \
  && apt-get install --no-install-recommends -y \
	 hydra-gtk \
	 ssh \
	 wordlists \
	 vim \
	 seclists \
	 masscan \
     curl \
     dnsutils \
     emacs \
     iputils-ping \
     netcat-openbsd \
     nmap \
     openssh-client \
     openssl \
     smbclient \
     traceroute \
     wget \
     libpcap-dev \
  && rm -rf /var/lib/apt/lists/*
