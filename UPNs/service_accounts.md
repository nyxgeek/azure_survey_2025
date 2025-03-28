# Statistics on Service Accounts

### Big Picture - Overview

- Total Domains tested for service accounts: 5,880,777

- Total Domains with Service Accounts: 1,079,217

- Total Domains Overall with Live Users: 1,323,508

- Percent of Live Domains with service accounts identified: 82% (1079217 / 1323508)

---

### admin vs administrator
```
nyxgeek@GIBSON# cat latest_emails.txt | grep '^administrator@' | wc -l
47363
nyxgeek@GIBSON# cat latest_emails.txt | grep '^administrator@' | grep '.onmicrosoft.com$' | wc -l
8570
nyxgeek@GIBSON# cat latest_emails.txt | grep '^admin@' | wc -l
340748
nyxgeek@GIBSON# cat latest_emails.txt | grep '^admin@' | grep '.onmicrosoft.com$' | wc -l
125689
```
**Winner: admin (88%)**

- Of the **admin** accounts, 125689 / 340748 (37%) were located on the organization's ```.onmicrosoft.com``` default domain, versus a custom domain.
- Of the **administrator** accounts, 8570 / 47363 (18%) were located on the organization's ```.onmicrosoft.com``` default domain, versus a custom domain.

---

### Top 100 Service Accounts

```
 348392 info
 340748 admin
  74797 support
  68776 sales
  47363 administrator
  46788 hr
  43742 marketing
  37559 contact
  35339 accounts
  34349 reception
  28906 it
  28811 accounting
  26814 finance
  23883 noreply
  23754 helpdesk
  23406 test
  19061 office
  14558 scanner
  13311 itsupport
  12810 testuser
  12215 conference
  11578 ap
  11544 training
  10815 no-reply
  10587 careers
  10166 service
  10129 payroll
   9465 maintenance
   8945 post
   8548 webmaster
   8328 boardroom
   8234 security
   8212 orders
   7968 warehouse
   7951 mail
   7893 intern
   7871 events
   7794 shipping
   7624 invoices
   7538 operations
   7149 production
   6619 scan
   6345 frontdesk
   5959 purchasing
   5565 customerservice
   5245 accountspayable
   5133 jobs
   5110 backup
   5009 hello
   5002 servicedesk
   4903 legal
   4849 media
   4793 team
   4600 receptionist
   4365 logistics
   4288 tech
   4263 recruitment
   4254 design
   4254 compliance
   4185 guest
   4116 dispatch
   4004 voicemail
   4002 sysadmin
   3720 chef
   3481 dev
   3224 crm
   3144 accueil
   3073 ithelpdesk
   2625 audit
   2451 sharepoint
   2318 admin1
   2169 ops
   2035 supervisor
   2009 qa
   1867 user
   1823 db
   1771 av
   1742 feedback
   1724 apple
   1704 administrador
   1680 spadmin
   1679 email
   1611 information
   1603 recruiting
   1574 testaccount
   1573 globaladmin
   1396 cloud
   1358 docs
   1357 reservas
   1354 order
   1251 studio
   1248 netadmin
   1204 webadmin
   1103 training1
   1058 care
   1056 privacy
    995 rt
    993 monitoring
    910 consultant
    893 jira
    812 conf
```
