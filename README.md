# pihole-kubernetes
Install k3s
curl -sfL https://get.k3s.io | sh -

Create directories:
mkdir -p /app/pihole/etc
mkdir /app/pihole/dnsmasq.d

Copy pihole.yml to /app/pihole

Change external IP to be that of host running k3s

In /app/pihole/ deploy by running
kubectl apply -f pihole.yml
