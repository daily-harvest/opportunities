# Introduction

Thank you for your interest in Daily Harvest! As the next step in our interview process, please complete the coding exercise below. This is a simplified instance of the Infrastructure as Code we use at Daily Harvest. We look forward to reviewing how you solve the challenge. Enjoy!

# Challenge

At Daily Harvest, we want to make it as easy as possible for our customers to get healthy food that they enjoy. In DevOps, we want to ensure that our infrastructure supports that goal, one of the ways we do that is to ensure that our infrastructure is consistent, revisioned, and repeatable as possible. Hashicorp Terraform is part of that solution.

In this challenge we would like you to create a basic web stack using Infrastructure as Code. You can choose to build your stack in GCP or AWS, either is fine with us. You can use modules, the registry, or write your own code, just add comments as you see fit. 

Good luck! We hope that you enjoy completing this challenge and look forward to seeing your approach to the problem.

# Requirements

* Your code should include the provider (but no keys)
* Create a VPC with two subnets in two different availability zones.
* Create necessary components to support external communication, such as a route table, Internet Gateway, etc.
* Create a private DNS zone called smoothiemachine.local
* Create an external Load Balancer (ALB or ELB is fine in AWS or Public HTTPS Load Balancer in GCP).
* Create two Ubuntu/Debian instances that are configured with the following:
    * An instance should be created on each availability zone
    * Each instance will have a 10G root drive.
    * Each instance will be tiny (t3.micro/e2-micro).
    * Each instance should run a script that does the following:
        * Installs, enables, starts Nginx
        * Replaces the index.html with a single line:  <p> Smoothie Power! </p> 

* Create a Security Group/Firewall Rules that allows port 80 Only from 0.0.0.0/0. The rule should be applied to the instances/vms and/or load balancer.
* Create a dns record for both hosts and the load balancer as such:
    * Hosts:
        * web0.smoothiemachine.local
        * web1.smoothiemachine.local
    * Load Balancer
        * dh.smoothiemachine.local 
 
# End Goal

Using your code, we can add keys/key.json and stand up infrastructure in AWS or GCP.
We should be able to access the load balancer IP on port 80 and get a page that says "Smoothie Power!"

# Notes

* Feel free to create resources in AWS or GCP (we use GCP here at Daily Harvest).
* Keep your code as clean and readable as possible.
* No need to create ssh or keypairs as there is no need to log into the instances.
