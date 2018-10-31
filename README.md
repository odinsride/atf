---
layout: default
---
# OOB Automated Testing [![Discord](https://img.shields.io/discord/289994252241338369.svg)](https://discord.gg/QaMwnGd) ![GitHub issues](https://img.shields.io/github/issues/jacebenson/x_8821_atf.svg) [![GitHub forks](https://img.shields.io/github/forks/jacebenson/x_8821_atf.svg)](https://github.com/jacebenson/x_8821_atf/network) [![GitHub stars](https://img.shields.io/github/stars/jacebenson/x_8821_atf.svg)](https://github.com/jacebenson/x_8821_atf/stargazers) 

OOB Automated Testing is a scoped app to 
capture tests for all the Out of Box 
servicenow applications.

## Installation

Due to this being a Scoped Application, to make this work with simplifying tests,
one modification must be made in Global Scope.  On 
`/sys_db_object.do?sysparm_query=name=sys_user_group`
under "Application Access", check "Can create", "Can update", "Can delete", and
save.

* servicenow instance London or newer
* Import `https://github.com/jacebenson/x_8821_atf.git` 
  to source control within Studio.

## Features

Tests will exist for and already exist for some of servicenow.

Below is the suite hierarcy.  If checked done.

- API Testing
  - [Agent Intelligence](https://github.com/jacebenson/x_8821_atf/issues/1) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/1.svg)](https://github.com/jacebenson/x_8821_atf/issue/1)
  - [Aggregate API](https://github.com/jacebenson/x_8821_atf/issues/2) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/2.svg)](https://github.com/jacebenson/x_8821_atf/issue/2)
  - [Application Service API](https://github.com/jacebenson/x_8821_atf/issues/3) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/3.svg)](https://github.com/jacebenson/x_8821_atf/issue/3)
  - [Attachment API](https://github.com/jacebenson/x_8821_atf/issues/4) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/4.svg)](https://github.com/jacebenson/x_8821_atf/issue/4)
  - [CI Lifecycle Mangement API](https://github.com/jacebenson/x_8821_atf/issues/5) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/5.svg)](https://github.com/jacebenson/x_8821_atf/issue/5)
  - [Clotho Time Series API](https://github.com/jacebenson/x_8821_atf/issues/6) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/6.svg)](https://github.com/jacebenson/x_8821_atf/issue/6)
  - [CMDB Instance API](https://github.com/jacebenson/x_8821_atf/issues/7) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/7.svg)](https://github.com/jacebenson/x_8821_atf/issue/7)
  - [CMDB Meta API](https://github.com/jacebenson/x_8821_atf/issues/8) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/8.svg)](https://github.com/jacebenson/x_8821_atf/issue/8)
  - [Email API](https://github.com/jacebenson/x_8821_atf/issues/29) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/29.svg)](https://github.com/jacebenson/x_8821_atf/issue/29)
  - [IdentifyReconcile API](https://github.com/jacebenson/x_8821_atf/issues/9) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/9.svg)](https://github.com/jacebenson/x_8821_atf/issue/9)
  - [Import Set API](https://github.com/jacebenson/x_8821_atf/issues/28) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/28.svg)](https://github.com/jacebenson/x_8821_atf/issue/28)
  - [Interaction Management API](https://github.com/jacebenson/x_8821_atf/issues/10) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/10.svg)](https://github.com/jacebenson/x_8821_atf/issue/10)
  - [Major Incident Management API](https://github.com/jacebenson/x_8821_atf/issues/11) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/11.svg)](https://github.com/jacebenson/x_8821_atf/issue/11)
  - [Performance Analytics API](https://github.com/jacebenson/x_8821_atf/issues/12) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/12.svg)](https://github.com/jacebenson/x_8821_atf/issue/12)
  - [Service Catalog API](https://github.com/jacebenson/x_8821_atf/issues/13) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/13.svg)](https://github.com/jacebenson/x_8821_atf/issue/13)
  - [Table API](https://github.com/jacebenson/x_8821_atf/issues/14) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/14.svg)](https://github.com/jacebenson/x_8821_atf/issue/14)
  - [Task Communication Management API](https://github.com/jacebenson/x_8821_atf/issues/15) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/15.svg)](https://github.com/jacebenson/x_8821_atf/issue/15)
  - [User Role Maintenance API](https://github.com/jacebenson/x_8821_atf/issues/16) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/16.svg)](https://github.com/jacebenson/x_8821_atf/issue/16)
- Customer Service Management
  - [Communities](https://github.com/jacebenson/x_8821_atf/issues/37) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/37.svg)](https://github.com/jacebenson/x_8821_atf/issue/37)
  - [Customer Service](https://github.com/jacebenson/x_8821_atf/issues/38) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/38.svg)](https://github.com/jacebenson/x_8821_atf/issue/38)
  - [Field Service](https://github.com/jacebenson/x_8821_atf/issues/39) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/39.svg)](https://github.com/jacebenson/x_8821_atf/issue/39)
- Governance, Risk , and Compliance (GRC)
  - [Audit](https://github.com/jacebenson/x_8821_atf/issues/25) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/25.svg)](https://github.com/jacebenson/x_8821_atf/issue/25)
  - [Policy and Compliance](https://github.com/jacebenson/x_8821_atf/issues/40) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/40.svg)](https://github.com/jacebenson/x_8821_atf/issue/40)
  - [Risk](https://github.com/jacebenson/x_8821_atf/issues/33) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/33.svg)](https://github.com/jacebenson/x_8821_atf/issue/33)
  - [Vendor Risk](https://github.com/jacebenson/x_8821_atf/issues/34) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/34.svg)](https://github.com/jacebenson/x_8821_atf/issue/34)
- HR Service Delivery
  - [Case and Knowledge](https://github.com/jacebenson/x_8821_atf/issues/41) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/41.svg)](https://github.com/jacebenson/x_8821_atf/issue/41)
  - [Employee Document](https://github.com/jacebenson/x_8821_atf/issues/42) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/42.svg)](https://github.com/jacebenson/x_8821_atf/issue/42)
  - [Employee Service Center](https://github.com/jacebenson/x_8821_atf/issues/43) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/43.svg)](https://github.com/jacebenson/x_8821_atf/issue/43)
  - [Enterpise Onboarding and Transistions](https://github.com/jacebenson/x_8821_atf/issues/44) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/44.svg)](https://github.com/jacebenson/x_8821_atf/issue/44)
  - [HR Integrations](https://github.com/jacebenson/x_8821_atf/issues/45) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/45.svg)](https://github.com/jacebenson/x_8821_atf/issue/45)
- IT Business Management
  - [Agile Development](https://github.com/jacebenson/x_8821_atf/issues/46) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/46.svg)](https://github.com/jacebenson/x_8821_atf/issue/46)
  - [Business Planning Portal](https://github.com/jacebenson/x_8821_atf/issues/47) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/47.svg)](https://github.com/jacebenson/x_8821_atf/issue/47)
  - [Cost](https://github.com/jacebenson/x_8821_atf/issues/48) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/48.svg)](https://github.com/jacebenson/x_8821_atf/issue/48)
  - [Enterprise Release Management](https://github.com/jacebenson/x_8821_atf/issues/49) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/49.svg)](https://github.com/jacebenson/x_8821_atf/issue/49)
  - [Financial](https://github.com/jacebenson/x_8821_atf/issues/50) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/50.svg)](https://github.com/jacebenson/x_8821_atf/issue/50)
  - [Project Portfolio](https://github.com/jacebenson/x_8821_atf/issues/51) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/51.svg)](https://github.com/jacebenson/x_8821_atf/issue/51)
  - [Scaled Agile Frameworkf (SAFe)](https://github.com/jacebenson/x_8821_atf/issues/52) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/52.svg)](https://github.com/jacebenson/x_8821_atf/issue/52)
  - [Test Management](https://github.com/jacebenson/x_8821_atf/issues/53) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/53.svg)](https://github.com/jacebenson/x_8821_atf/issue/53)
  - [Time Card](https://github.com/jacebenson/x_8821_atf/issues/54) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/54.svg)](https://github.com/jacebenson/x_8821_atf/issue/54)
- IT Operations Management
  - [Cloud Management](https://github.com/jacebenson/x_8821_atf/issues/55) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/55.svg)](https://github.com/jacebenson/x_8821_atf/issue/55)
  - [Discovery](https://github.com/jacebenson/x_8821_atf/issues/56) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/56.svg)](https://github.com/jacebenson/x_8821_atf/issue/56)
  - [Event Management](https://github.com/jacebenson/x_8821_atf/issues/57) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/57.svg)](https://github.com/jacebenson/x_8821_atf/issue/57)
  - [Operational Intelligence](https://github.com/jacebenson/x_8821_atf/issues/58) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/58.svg)](https://github.com/jacebenson/x_8821_atf/issue/58)
  - [Service Mapping](https://github.com/jacebenson/x_8821_atf/issues/59) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/59.svg)](https://github.com/jacebenson/x_8821_atf/issue/59)
- IT Service Management
  - [Asset](https://github.com/jacebenson/x_8821_atf/issues/30) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/30.svg)](https://github.com/jacebenson/x_8821_atf/issue/30)
  - [Benchmarks](https://github.com/jacebenson/x_8821_atf/issues/60) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/60.svg)](https://github.com/jacebenson/x_8821_atf/issue/60)
  - [Change](https://github.com/jacebenson/x_8821_atf/issues/19) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/19.svg)](https://github.com/jacebenson/x_8821_atf/issue/19)
  - [Continual Improvement](https://github.com/jacebenson/x_8821_atf/issues/61) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/61.svg)](https://github.com/jacebenson/x_8821_atf/issue/61)
  - [Contract](https://github.com/jacebenson/x_8821_atf/issues/62) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/62.svg)](https://github.com/jacebenson/x_8821_atf/issue/62)
  - [Expense Line](https://github.com/jacebenson/x_8821_atf/issues/63) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/63.svg)](https://github.com/jacebenson/x_8821_atf/issue/63)
  - [Incident](https://github.com/jacebenson/x_8821_atf/issues/17) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/17.svg)](https://github.com/jacebenson/x_8821_atf/issue/17)
  - [Incident Communications](https://github.com/jacebenson/x_8821_atf/issues/18) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/18.svg)](https://github.com/jacebenson/x_8821_atf/issue/18)
  - [ITSM Virtual Agent](https://github.com/jacebenson/x_8821_atf/issues/64) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/64.svg)](https://github.com/jacebenson/x_8821_atf/issue/64)
  - [On-call Scheduling](https://github.com/jacebenson/x_8821_atf/issues/65) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/65.svg)](https://github.com/jacebenson/x_8821_atf/issue/65)
  - [Problem](https://github.com/jacebenson/x_8821_atf/issues/20) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/20.svg)](https://github.com/jacebenson/x_8821_atf/issue/20)
  - [Procurement](https://github.com/jacebenson/x_8821_atf/issues/66) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/66.svg)](https://github.com/jacebenson/x_8821_atf/issue/66)
  - [Product Catalog](https://github.com/jacebenson/x_8821_atf/issues/67) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/67.svg)](https://github.com/jacebenson/x_8821_atf/issue/67)
  - [Release](https://github.com/jacebenson/x_8821_atf/issues/68) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/68.svg)](https://github.com/jacebenson/x_8821_atf/issue/68)
  - [Request](https://github.com/jacebenson/x_8821_atf/issues/21) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/21.svg)](https://github.com/jacebenson/x_8821_atf/issue/21)
  - [Service Catalog](https://github.com/jacebenson/x_8821_atf/issues/22) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/22.svg)](https://github.com/jacebenson/x_8821_atf/issue/22)
  - [Service Desk](https://github.com/jacebenson/x_8821_atf/issues/69) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/69.svg)](https://github.com/jacebenson/x_8821_atf/issue/69)
  - [Service Level](https://github.com/jacebenson/x_8821_atf/issues/70) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/70.svg)](https://github.com/jacebenson/x_8821_atf/issue/70)
  - [Service Portfolio](https://github.com/jacebenson/x_8821_atf/issues/71) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/71.svg)](https://github.com/jacebenson/x_8821_atf/issue/71)
  - [Vendor Performance](https://github.com/jacebenson/x_8821_atf/issues/72) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/72.svg)](https://github.com/jacebenson/x_8821_atf/issue/72)
  - [Walk-up Experience](https://github.com/jacebenson/x_8821_atf/issues/73) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/73.svg)](https://github.com/jacebenson/x_8821_atf/issue/73)
- Now Platform
  - [Agent Intelligence](https://github.com/jacebenson/x_8821_atf/issues/74) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/74.svg)](https://github.com/jacebenson/x_8821_atf/issue/74)
  - [CMDB](https://github.com/jacebenson/x_8821_atf/issues/75) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/75.svg)](https://github.com/jacebenson/x_8821_atf/issue/75)
  - [Compliance](https://github.com/jacebenson/x_8821_atf/issues/76) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/76.svg)](https://github.com/jacebenson/x_8821_atf/issue/76)
  - [Connect](https://github.com/jacebenson/x_8821_atf/issues/77) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/77.svg)](https://github.com/jacebenson/x_8821_atf/issue/77)
  - [Content Management System](https://github.com/jacebenson/x_8821_atf/issues/78) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/78.svg)](https://github.com/jacebenson/x_8821_atf/issue/78)
  - [Data Certification](https://github.com/jacebenson/x_8821_atf/issues/79) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/79.svg)](https://github.com/jacebenson/x_8821_atf/issue/79)
  - [Dependency Views](https://github.com/jacebenson/x_8821_atf/issues/80) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/80.svg)](https://github.com/jacebenson/x_8821_atf/issue/80)
  - [Flow Designer](https://github.com/jacebenson/x_8821_atf/issues/81) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/81.svg)](https://github.com/jacebenson/x_8821_atf/issue/81)
  - [IntegrationHub](https://github.com/jacebenson/x_8821_atf/issues/82) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/82.svg)](https://github.com/jacebenson/x_8821_atf/issue/82)
  - [Interaction Management](https://github.com/jacebenson/x_8821_atf/issues/83) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/83.svg)](https://github.com/jacebenson/x_8821_atf/issue/83)
  - [Knowledge Management](https://github.com/jacebenson/x_8821_atf/issues/84) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/84.svg)](https://github.com/jacebenson/x_8821_atf/issue/84)
  - [Live Feed](https://github.com/jacebenson/x_8821_atf/issues/85) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/85.svg)](https://github.com/jacebenson/x_8821_atf/issue/85)
  - [Managed Documents](https://github.com/jacebenson/x_8821_atf/issues/86) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/86.svg)](https://github.com/jacebenson/x_8821_atf/issue/86)
  - [MetricBase](https://github.com/jacebenson/x_8821_atf/issues/87) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/87.svg)](https://github.com/jacebenson/x_8821_atf/issue/87)
  - [Notifications](https://github.com/jacebenson/x_8821_atf/issues/88) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/88.svg)](https://github.com/jacebenson/x_8821_atf/issue/88)
  - [Notify](https://github.com/jacebenson/x_8821_atf/issues/89) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/89.svg)](https://github.com/jacebenson/x_8821_atf/issue/89)
  - [Orchestration](https://github.com/jacebenson/x_8821_atf/issues/90) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/90.svg)](https://github.com/jacebenson/x_8821_atf/issue/90)
  - [Password Reset](https://github.com/jacebenson/x_8821_atf/issues/91) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/91.svg)](https://github.com/jacebenson/x_8821_atf/issue/91)
  - [Service Administration](https://github.com/jacebenson/x_8821_atf/issues/92) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/92.svg)](https://github.com/jacebenson/x_8821_atf/issue/92)
  - [Service Portal](https://github.com/jacebenson/x_8821_atf/issues/93) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/93.svg)](https://github.com/jacebenson/x_8821_atf/issue/93)
  - [Subscription Management](https://github.com/jacebenson/x_8821_atf/issues/95) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/95.svg)](https://github.com/jacebenson/x_8821_atf/issue/95)
  - [Survey Management](https://github.com/jacebenson/x_8821_atf/issues/94) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/94.svg)](https://github.com/jacebenson/x_8821_atf/issue/94)
  - [Task Communication Management](https://github.com/jacebenson/x_8821_atf/issues/96) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/96.svg)](https://github.com/jacebenson/x_8821_atf/issue/96)
  - [Virtual Agent](https://github.com/jacebenson/x_8821_atf/issues/97) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/97.svg)](https://github.com/jacebenson/x_8821_atf/issue/97)
  - [Visual Task Boards](https://github.com/jacebenson/x_8821_atf/issues/98) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/98.svg)](https://github.com/jacebenson/x_8821_atf/issue/98)
  - [Workflow](https://github.com/jacebenson/x_8821_atf/issues/99) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/99.svg)](https://github.com/jacebenson/x_8821_atf/issue/99)
- Security Operations
  - [Configuration Compliance](https://github.com/jacebenson/x_8821_atf/issues/100) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/100.svg)](https://github.com/jacebenson/x_8821_atf/issue/100)
  - [Security Incident Response](https://github.com/jacebenson/x_8821_atf/issues/101) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/101.svg)](https://github.com/jacebenson/x_8821_atf/issue/101)
  - [Threat Intelligence](https://github.com/jacebenson/x_8821_atf/issues/102) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/102.svg)](https://github.com/jacebenson/x_8821_atf/issue/102)
  - [Trusted Security Circles](https://github.com/jacebenson/x_8821_atf/issues/103) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/103.svg)](https://github.com/jacebenson/x_8821_atf/issue/103)
  - [Vulnerability Response](https://github.com/jacebenson/x_8821_atf/issues/104) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/104.svg)](https://github.com/jacebenson/x_8821_atf/issue/104)
- Service Management
  - [Coaching Loops](https://github.com/jacebenson/x_8821_atf/issues/35) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/35.svg)](https://github.com/jacebenson/x_8821_atf/issue/35)
  - [Facilities](https://github.com/jacebenson/x_8821_atf/issues/36) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/36.svg)](https://github.com/jacebenson/x_8821_atf/issue/36)
  - [Finance](https://github.com/jacebenson/x_8821_atf/issues/105) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/105.svg)](https://github.com/jacebenson/x_8821_atf/issue/105)
  - [Legal](https://github.com/jacebenson/x_8821_atf/issues/106) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/106.svg)](https://github.com/jacebenson/x_8821_atf/issue/106)
  - [Marketing](https://github.com/jacebenson/x_8821_atf/issues/107) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/107.svg)](https://github.com/jacebenson/x_8821_atf/issue/107)
  - [Planned Maintenance](https://github.com/jacebenson/x_8821_atf/issues/108) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/108.svg)](https://github.com/jacebenson/x_8821_atf/issue/108)
  - [Structured Problem Analysis](https://github.com/jacebenson/x_8821_atf/issues/109) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/109.svg)](https://github.com/jacebenson/x_8821_atf/issue/109)
- [Software Asset Management](https://github.com/jacebenson/x_8821_atf/issues/26) [![Issue](https://img.shields.io/github/issues/detail/s/jacebenson/x_8821_atf/26.svg)](https://github.com/jacebenson/x_8821_atf/issue/26)
 

## Contributing

Pull requests are welcome. For major changes, 
please open an issue first to discuss what you 
would like to change.

I'd suggest starting on an [issue that seems well made](https://github.com/jacebenson/x_8821_atf/issues?q=is%3Aopen+is%3Aissue+label%3A%22good+first+issue%22).

However there are a lot of issues for everything I could find in servicenow.  If you know that application feel free to fill out the issue and comment on it.

### Setting up a pdi (personal developer instance)

Create an account on [https://developer.servicenow.com/](https://developer.servicenow.com/).
Than Request a Personal Developer Instance.

### Setting up the repo

Due to this being a Scoped Application, to make this work with simplifying tests,
one modification must be made in Global Scope.  On 
`/sys_db_object.do?sysparm_query=name=sys_user_group`
under "Application Access", check "Can create", "Can update", "Can delete", and
save.

1.  [Fork this project](https://github.com/jacebenson/x_8821_atf/fork)
2.  Log into your PDI
3.  Open Studio
4.  Import your Forked Repo's `https` url

### Actually Contributing

1.  Comment on the issue
2.  Ensure you're in the OOB Automated Testing application
3.  Create the tests and suites appropriate to test the application
4.  Put your tests in the appropriate suites
4.  Commit your repo
5.  Comeback onto github, and make a Pull Request from your repo.

## Resources

* If you need to `set fields` but cannot find 
  you're field, this script might be useful;
  ```js
  var gr = new GlideRecord('sys_atf_step');
  gr.get('f1a43c15db0123008096a455ca961915');
  var fields = gr.inputs.field_values.toString();
  gs.info(fields);
  fields = fields.replace('^EQ','^kb_knowledge_base=dfc19531bf2021003f07e2c1ac0739ab^EQ');
  gs.info(fields);
  gr.inputs.field_values = fields;
  gr.update();
  ```
