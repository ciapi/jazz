
# Problem

Providing a 100% available, elastic and resource efficient Jenkins cluster is a challenge. Hence JaaS = Jenkins as a Service.

#Goal

JaaS when complete would be an API first installable with containers as first class citizens.

![JaaS - Logo](https://raw.githubusercontent.com/ciapi/jaas/master/docs/design/JaaS-High-Level-Design.png)

#Tutorial

<a href="http://www.youtube.com/watch?feature=player_embedded&v=OVHMULHB7CE
" target="_blank"><img src="http://img.youtube.com/vi/OVHMULHB7CE/0.jpg" 
alt="Basic Intro to Jenkins and Backups" width="80%" height="80%" border="10" /></a>

#Motivation

eBay had solved this problem https://youtu.be/VZPbLUJnR68 using Mesos. However Mesos's components are prone to failure and eBay's solution is not open sourced when this document was created.

This project would be an open source API first JaaS experience for enterprises to install and maintain, with following attributes

1. Elastic
2. Reliable
3. Efficient

## Elastic - How?

Using Mesos + Aurora to spin off Jenkins containers [Docker for now] with a click of a button

## Reliable - How?

MAZ (Mesos+Aurora+Zookeeper) would provide Jenkins Resilience
MAZ on Kubernetes will provide MAZ Resilience.

## Efficient - How?

If a Jenkins instance isn't building anything, it would be hibernated and the resources allocated to that instance would be re-purposed to spin off another.


#NOTES

British Gov seems to have blogged about cloud-tech. [Blog & Comment](https://gdstechnology.blog.gov.uk/2015/10/27/looking-at-open-source-paas-technologies/#comment-52911) 

https://github.com/eBayClassifiedsGroup/PanteraS sounds interesting
