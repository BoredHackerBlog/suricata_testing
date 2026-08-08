# suricata_testing
for testing suricata rules

Based on this: https://medium.com/@blue_e/pcap-analysis-with-suricata-88e1b13a1b0d


Install suricata. `apt install suricata` on ubuntu works.

make sure the rules have `alert http any any -> any any ` 

edit the suricata.yaml file to point to folder where suricata.rules is or put your suricata.rules file in /tmp

run `suricata -c suricata.yaml -r yourpcap.pcap` 

check eve.json file
