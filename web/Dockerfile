FROM nginx
COPY . /usr/share/nginx/html
RUN apt update && apt install openssh-server net-tools -y
COPY sshd_config /etc/ssh/sshd_config
RUN useradd -rg root -G sudo -p "$(openssl passwd -1 sshuserpw)" sshuser

RUN systemctl enable ssh
