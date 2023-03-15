This repo sets up and configures an OpenVPN server and an Certifivate Authority server on CentOS9
  - you should specify IPv4 address and path to both SSH private keys files in "hosts.txt" file for those servers
  - also you should specify your vars in "group_vars/all_hosts.yml", there are some additional comments to help
  - in "base.conf" file on the 42th line you should replace ip address to the ip address of your OpenVPN server
  - recomend to move "base.conf", "server.conf", "make_config.sh" to a separate directory, specified in the "group_vars/all_hosts.yml" file
  - playbooks should be run in the required sequence
  - after last step you will get a "client.ovpn" file that should be pass to command "sudo openvpn --config client1.ovpn" on client machine




