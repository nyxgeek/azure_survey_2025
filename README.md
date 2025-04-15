# azure_survey_2025
results of scraping OneDrive from February 2022 - March 2025
***
For additional information, you can find the survey wordlists used here: https://github.com/nyxgeek/trontastic_usernames

My ShmooCon 20 talk (2025) can be found here: https://github.com/nyxgeek/shmoocon

## Contents
1. [General Statistics](#general-statistics)
   - [Overall Stats](#overall-stats)
   - [Fortune 500 Stats](#fortune-500-stats)
2. [ADFS Statistics](#adfs-statistics)
3. [User Statistics](#user-statistics)
   - [Initials](UPNs/initials.md)
   - [Nicknames](UPNs/nicknames.md)
   - [Numeric Usernames](UPNs/numeric.md)
   - [Service Accounts](UPNs/service_accounts.md)
   - [UPNs with digits appended (jsmith1, jsmith2)](UPNs/append_digits.md)
4. [Environments](#environments)
5. [Top TLDs](#top-tlds)
   - [Top TLDs by Number of Unique Domains](#top-tlds-by-domain-count)
   - [Maps - Total Domains per ccTLD](#top-country-code-tlds---total-domains)
   - [Top TLDs by Number of Users](#top-tlds-by-user-count)
   - [Maps - Total Users per ccTLD](#top-country-code-tlds---total-users)
6. [Bot Stats](#bot-stats)

---

## General Statistics



### Overall Stats
Some notes:
- "Live" refers to tenants or domains where users were identified
- The "OnMicrosoft" domain for a tenant is their default tenant domain (tenant_name.onmicrosoft.com).

  
```
Total Tenants:    4,033,132
Tenants with SharePoint Enabled:    1,946,381 (48%)
Tenants with OneDrive Enabled:     1,946,201 (48%)

Total Live Tenants:    1,032,350

Total Custom Domains: 7,053,874
Average Domains per Tenant: 1.74

Total domains identified with live users:    1,323,508
    Live   Custom    Domains:      1,177,674
    Live OnMicrosoft Domains:        145,834



Azure Environments - All Organizations
+----------------+----------+
| environment    |    COUNT | 
+----------------+----------+
| commercial     |  4017640 |
| china          |    13498 |
| gcc            |      298 |
| dod            |        7 |
+----------------+----------+


Azure Environments - Live Tenants
+----------------+----------+
| environment    |    COUNT | 
+----------------+----------+
| commercial     |  1031625 |
| china          |      498 |
| gcc            |      263 |
| dod            |        4 |
+----------------+----------+



Total Custom Domains per Tenant
-------------------------------
Max: 4999
Mean: 1.99
Mode: 1

*LIVE* Custom Domains per Tenant
-------------------------------
Max: 374
Mean: 1.2856
Mode: 2
```

![bar graph showing distribution of user population in domains 1.2m of the 1.3m have 1-100 usernames found](graphics/domains_user_count.png)


### Fortune 500 Stats

As noted, these numbers are from the 2024 Fortune 500 list. In this sample, the total number of tenant is differentiated from the total number of orgs because of the high prevalance of multi-tenant setups in large, Fortune 500 companies.

To reiterate:
- "Live" refers to tenants or domains where users were identified
- The "OnMicrosoft" domain for a tenant is their default tenant domain (tenant_name.onmicrosoft.com).


```
Total Organizations in Azure: 499 (99.8%)
  Total Tenants: 553
Organizations with multi-tenant config: 112 (22%)

Total Orgs with SharePoint: 431
  Total Tenants with SharePoint: 550
Total Orgs with OneDrive: 431
  Total Tenants with OneDrive: 550

Total Live Orgs: 427
  Total Live Tenants: 431

Total Custom Domains: 67,175
Average Domains per Org: 155
Average Domains per Tenant: 121
Average Tenants per Org: 1.11

Total Domains Identified with Live Users: 3,333 (5% of total custom domains)
    Live   Custom    Domains:      3,237
    Live OnMicrosoft Domains:         96

Total tenants identified with live users:    1,032,350
Total  unique tenant/domain combinations:    1,327,151


Azure Environments - All Organizations
+--------------+--------+
| environment  |  COUNT | 
+--------------+--------+
| commercial   |    488 |
| gcc          |     11 |
+--------------+--------+

Azure Environments - Live Tenants
+--------------+--------+
| environment  |  COUNT | 
+--------------+--------+
| commercial   |    430 |
| gcc          |      1 |
+--------------+--------+



Total Custom Domains per Tenant
-------------------------------
Max: 
Mean: 
Mode: 

*LIVE* Custom Domains per Tenant
-------------------------------
Max: 
Mean: 
Mode: 
```

#### Tenants per Organization - Count Sorted
```
Count   |  Number of Tenants
--------|-------------------
    387 |  1
     21 |  2
     10 |  4
      8 |  3
      3 |  7
      2 |  6
      1 |  9
      1 |  8
      1 |  10
```

#### Tenants per Organization - Ordered by Number of Tenants
```
Count   |  Number of Tenants
--------|-------------------
    387 |  1
     21 |  2
      8 |  3
     10 |  4
    N/A |  5
      2 |  6
      3 |  7
      1 |  8
      1 |  9
      1 |  10
```


---

## ADFS Statistics

### ADFS Popularity - Overall
```
Overall
Total Tenants: 939,706
    ADFS: 98,344 (10.4%)
    Managed: 841,362 (89.5%)
```
### ADFS Popularity - Overall
```
Fortune 500
Total Tenants: 499
    ADFS: 211 (42.3%)
    Managed: 288 (57.7%)
```

### Top External IDPs - Overall
```
71961 godaddy.com
5810 	okta.com
2551 	sso.duosecurity.com
1024 	secureserver.net
703 	onelogin.com
467 	google.com
203 	okta-emea.com
```

### Top External IDPs - Fortune 500
```
66	Okta
4	OneLogin
```

---

## User Statistics
*These are statistics on the usernames, or more appropriately, the UPNs (User Principal Names) which are unique identifiers in Entra ID.*

```
Total  usernames:    70,252,711    (2025.03.04)
Unique usernames:    14,410,943

Average users per domain: 59.65

Total days of  scraping:    1127
Usernames Found per Day:    62,336 usernames/day


Total Numeric Usernames  (1234, 12345, 123456):    10,405,919
Unique Numeric Usernames (1234, 12345, 123456):    4,066,717


Total Non-Numeric Usernames (jsmith, jsmith9):    59,799,886
Unique Non-Numeric Usernames (jsmith, jsmith9):    10,344,182

Total Usernames with Digit Appended  (jsmith9):    3,329,386
Unique Usernames with Digit Appended (jsmith9):    1,749,196

Unique base usernames (jsmith9 -> jsmith):    8,255,074

```
More user stats can be found within the UPNs folder.

#### Username Stats
- [Initials](UPNs/initials.md)
- [Nicknames](UPNs/nicknames.md)
- [Numeric Usernames](UPNs/numeric.md)
- [Service Accounts](UPNs/service_accounts.md)
- [UPNs with digits appended (jsmith1, jsmith2)](UPNs/append_digits.md)

---

## Environments

### Overall Stats - Users per Azure Environment
```
+----------------+----------+
| source         | count(*) |
+----------------+----------+
| onedrive       | 69847070 |
| onedrive_gcc   |   336642 |
| onedrive_dod   |    xxxxx |
| onedrive_china |    15551 |
+----------------+----------+
```


---

## Top TLDs

### Top TLDs by Domain Count

In this list, all unique domains were considered. This reflects the range of domain TLDs.

```
 939056 com
 124646 org
  36076 uk
  34657 no
  19449 au
  15723 net
  11919 ca
  11039 nl
   9734 de
   7511 fr
   4691 edu
   4558 gov
   4142 za
   4028 it
   3829 us
   3820 co
   3537 be
   3417 es
   3318 in
   3285 se
```

![Top domains by domain count - pie graph](graphics/top_domains_by_domain_count.png)
![Top domains by domain count - pie graph](graphics/top_domains_by_user_count.png)


### Top Country-Code TLDs - Total Domains

![chloropleth map showing number of domains found per TLD, such as .us or .uk](graphics/ccTLD_by_domain_world_numbers.png)

![chloropleth map showing number of domains found per TLD, such as .us or .uk](graphics/ccTLD_by_domain_europe.png)

![chloropleth map showing number of domains found per TLD, such as .us or .uk](graphics/ccTLD_by_domain_northamerica.png)

![chloropleth map showing number of domains found per TLD, such as .us or .uk](graphics/ccTLD_by_domain_southamerica.png)

![chloropleth map showing number of domains found per TLD, such as .us or .uk](graphics/ccTLD_by_domain_africa.png)

![chloropleth map showing number of domains found per TLD, such as .us or .uk](graphics/ccTLD_by_domain_asia.png)

![chloropleth map showing number of domains found per TLD, such as .us or .uk](graphics/ccTLD_by_domain_oceania.png)

Full list: [top_tld_by_domain_count.txt](TLDs/top_tld_by_domain_count.txt)


### Top TLDs by User Count

In this list, all unique usernames (UPNs) were considered. This reflects the number of users and their UPN TLDs.

```
35415789 com
 9640870 edu
 7785823 org
 3086671 gov
 2215033 net
 1968785 uk
 1623449 br
 1610670 au
  984496 no
  816149 us
  709805 ca
  412149 pe
  351209 nl
  271255 pl
  241629 co
  199007 mx
  178381 it
  175622 in
  159490 za
  158896 sa
```

### Top Country-Code TLDs - Total Users

![chloropleth map showing number of users found per TLD, such as .us or .uk](graphics/ccTLD_by_user_world_numbers.png)

![chloropleth map showing number of users found per TLD, such as .us or .uk](graphics/ccTLD_by_user_europe.png)

![chloropleth map showing number of users found per TLD, such as .us or .uk](graphics/ccTLD_by_user_northamerica.png)

![chloropleth map showing number of users found per TLD, such as .us or .uk](graphics/ccTLD_by_user_southamerica.png)

![chloropleth map showing number of users found per TLD, such as .us or .uk](graphics/ccTLD_by_user_africa.png)

![chloropleth map showing number of users found per TLD, such as .us or .uk](graphics/ccTLD_by_user_asia.png)

![chloropleth map showing number of users found per TLD, such as .us or .uk](graphics/ccTLD_by_user_oceania.png)


Full list: [top_tld_by_upn_count.txt](TLDs/top_tld_by_upn_count.txt)

---

## Bot Stats
```
Total machines employed over lifetime of project:    98
Average active machines:    33.64

Total machine-hours of scraping:    493,584
```

### Active Machines per Month
*Note: I only started tracking in March of 2023*
```
+---------+----------------+----------------------------------------------------------+
| month   | distinct_hosts |    1  <----------------------------------------->  49    |
+---------+----------------+----------------------------------------------------------+
| 2023-03 |    49          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX     |
| 2023-04 |    49          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX     |
| 2023-05 |    50          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX    |
| 2023-06 |    40          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX              |
| 2023-07 |    39          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX               |
| 2023-08 |    30          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXX                        |
| 2023-09 |    15          |    XXXXXXXXXXXXXXX                                       |
| 2023-10 |    15          |    XXXXXXXXXXXXXXX                                       |
| 2023-11 |    15          |    XXXXXXXXXXXXXXX                                       |
| 2023-12 |    15          |    XXXXXXXXXXXXXXX                                       |
| 2024-01 |    36          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX                  |
| 2024-02 |    42          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX            |
| 2024-03 |    30          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXX                        |
| 2024-04 |    33          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX                     |
| 2024-05 |    35          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX                   |
| 2024-06 |    33          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX                     |
| 2024-07 |    33          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX                     |
| 2024-08 |    32          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX                      |
| 2024-09 |    32          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX                      |
| 2024-10 |    33          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX                     |
| 2024-11 |    36          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX                  |
| 2024-12 |    48          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX      |
| 2025-01 |    45          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX         |
| 2025-02 |    45          |    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX         |
| 2025-03 |    11          |    XXXXXXXXXXX                                           |
+---------+----------------+----------------------------------------------------------+


```
