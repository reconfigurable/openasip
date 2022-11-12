FROM debian:11

RUN apt-get -y update
RUN apt-get -y upgrade

RUN apt-get install -y libwxgtk3.0-gtk3-dev libboost-all-dev tcl8.6-dev libedit-dev libsqlite3-dev sqlite3 libxerces-c-dev g++ make latex2html libffi-dev autoconf automake libtool subversion git cmake graphviz 

WORKDIR /root

RUN git clone https://github.com/cpc/openasip.git openasip

RUN cd openasip/openasip && tools/scripts/install_llvm_14.sh $HOME/local

#RUN cd /root && git clone https://github.com/riscv-collab/riscv-gnu-toolchain riscv-gnu-toolchain

#RUN apt-get install -y gawk ftp texinfo build-essential bison

#RUN cd /root/riscv-gnu-toolchain && ./configure --prefix=/opt/riscv --with-arch=rv32im
#RUN cd /root/riscv-gnu-toolchain && make && make install

#RUN cd /root && git clone https://github.com/sifive/elf2hex.git
#RUN cd elf2hex && autoreconf -i && ./configure --prefix=/opt/riscv --target=riscv32-unknown-elf && make && make install

CMD while true; do sleep 10; done;
