# GCP VPC Networking Lab

Hands-on lab from the Google Cloud Associate Cloud Engineer path: **Create and Configure VPC Networks** (Lab ID: CBL057, score 100/100).

## What I built
- An auto mode VPC (`mynetwork`) with firewall rules, converted to custom mode
- Two custom mode VPCs (`managementnet`, `privatenet`) with their own subnets and firewall rules
- Four Compute Engine VMs across three VPC networks and two regions
- An IAP firewall rule for SSH without exposing port 22 to the internet

## What I tested
- External IP pings worked across networks, because ICMP was allowed
- Internal IP pings worked only inside the same VPC, across regions
- Internal IP pings between different VPCs failed with 100% packet loss, because VPC networks are isolated by default

## Skills demonstrated
VPC design (auto vs custom mode) · Subnets and CIDR planning · Firewall rules · IAP TCP forwarding · gcloud CLI · Compute Engine · Network connectivity troubleshooting

## Full report
See [GCP_VPC_Networks_Lab_Report.pdf](GCP_VPC_Networks_Lab_Report.pdf) for the step-by-step walkthrough with screenshots.
