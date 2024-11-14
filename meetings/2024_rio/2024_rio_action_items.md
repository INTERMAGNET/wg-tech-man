# Report of meeting of GIN Subcommittee during INTERMAGNET Rio-de-Janeiro meeting, 7th and 8th  November 2024

## Attendees
- Stephan Bracke
- Chris Turbitt
- Jürgen Matzka
- Andrew Lewis

# INTERMAGNET Technical Manual Subcommittee, November 2024

Subcommittee Members: Stephan Bracke (chair), Chris Turbitt (deputy), ,
Andrew Lewis, Jürgen Matzka

## TM Subcommittee agenda, November 2024

1.  Review of may 2023 actions items

2.  Release of Technical Manual 5.1.0

3.  Technical Manual

    a.  DOI and how to work with it

    b.  Start a collaborated work on it

        i.  reviews on development branch

        ii. new chapters on seperated branches

    c.  IYFV 1.03

```{=html}
<!-- -->
```
1.  

```{=html}
<!-- -->
```
4.  WEB

    a.  Links to data format in the Technical Manual

    b.  Other links to/from the web site

    c.  discussion on where to find what for data downloads

    d.  FAQ maintenance

5.  Plan next release in phases

6.  Need for new members

**1. Review of may 2023 actions items**

Report on the completion of action items from the subcommittee meeting
in may 2023.

## Action items from may 2023 meeting 

+--------+-----------+--------------------------+---------------------+
| **Nu   | Re        | Description              | **tatus Green       |
| mber** | sponsible |                          | completed; Orange   |
|        |           |                          | ongoing; Red not    |
|        |           |                          | started**           |
+--------+-----------+--------------------------+---------------------+
| **     | JM        | Generate a DOI for the   | SB send pdf and     |
| TM.1** |           | next release in RST      | look into           |
|        |           | format for the Technical | possibilities of    |
|        |           | Manual V-5.1.0.          | automate DOI        |
|        |           |                          | creation linked     |
|        |           |                          | with release tags   |
+--------+-----------+--------------------------+---------------------+
| **     | SB        | Publish TM V-5.1.0 once  | Complete            |
| TM.2** |           | the new collaboration    |                     |
|        |           | environment is available |                     |
|        |           | on GitHub.               |                     |
+--------+-----------+--------------------------+---------------------+
| **     | SB        | Configure a dedicated    | Complete            |
| TM.3** |           | environment to           |                     |
|        |           | INTERMAGNET for the TM   |                     |
|        |           | on GitHub.               |                     |
+--------+-----------+--------------------------+---------------------+
| **     | SB        | Configure a dedicated    | Complete            |
| TM.4** |           | environment to           |                     |
|        |           | INTERMAGNET for the TM   |                     |
|        |           | on ReadTheDocs.          |                     |
+--------+-----------+--------------------------+---------------------+
| **     | SB        | Complete the conversion  | Complete            |
| TM.5** |           | of the current version   |                     |
|        |           | of the manual to RST     |                     |
|        |           | (only 3 pages left).     |                     |
+--------+-----------+--------------------------+---------------------+
| **     | TM        | Install the new          | Ongoing (saturday)  |
| TM.6** | sub       | development tools        |                     |
|        | committee | locally and experiment   |                     |
|        |           | with them.               |                     |
+--------+-----------+--------------------------+---------------------+
| **     | CT        | Look at TN and FAQs for  | Not started         |
| TM.7** |           | QD information to be     |                     |
|        |           | added to the TM.         |                     |
+--------+-----------+--------------------------+---------------------+
| **     | JM        | Description on the use   | Complete            |
| TM.8** |           | of DOIs for              |                     |
|        |           | data/metadata            |                     |
|        |           | publication in           |                     |
|        |           | INTERMAGNET.             |                     |
+--------+-----------+--------------------------+---------------------+
| **     | DD        | Provide text for the TM  | Still to do         |
| TM.9** | sub       | on the use of flags as a |                     |
|        | committee | separate metadata field  |                     |
|        |           | (ref. DD31) if this is   |                     |
|        |           | to be adopted in CDF     |                     |
|        |           | format.                  |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | BSL       | Modify Technical Manual  | Completed           |
| M.10** |           | references to the 90%    |                     |
|        |           | rule to state that this  |                     |
|        |           | can be interpreted as    |                     |
|        |           | either 90% of the values |                     |
|        |           | or 90% of the weight of  |                     |
|        |           | the filter. To be        |                     |
|        |           | included in V-5.1.0      |                     |
|        |           | release.                 |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | GIN       | Flagging of data -- how  | Still to do         |
| M.11** |           | to preserve data rather  |                     |
|        | sub       | than deleting it using a |                     |
|        | committee | separate flag data       |                     |
|        |           | field. Is this only for  |                     |
|        |           | CDF or also for other    |                     |
|        |           | formats?                 |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | SB & CB   | Configure URL            | Completed           |
| M.12** |           | intermagnet.org for      |                     |
|        |           | GitHub and ReadTheDocs.  |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | BSL       | Page 5 par 2 ...         | Completed           |
| M.13** |           | recognized format --     |                     |
|        |           | could add a pointer to   |                     |
|        |           | the section in the       |                     |
|        |           | document that describes  |                     |
|        |           | that. Section 6.1.1. To  |                     |
|        |           | be included in V-5.1.0   |                     |
|        |           | release.                 |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | BSL       | In Chapter 2 - not clear | Completed           |
| M.14** |           | what the definitions of  |                     |
|        |           | the data types are --    |                     |
|        |           | add pointer to           |                     |
|        |           | definition/relevant      |                     |
|        |           | text.                    |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | JM        | Section 2.3.9 -- add     | Completed           |
| M.15** |           | text describing where    |                     |
|        |           | the gp ratio is used. To |                     |
|        |           | be included in V-5.1.0   |                     |
|        |           | release.                 |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | BSL       | Page 13 column 1,        | Completed           |
| M.16** |           | paragraph 1 -- It makes  |                     |
|        |           | no sense to me to use    |                     |
|        |           | the examples of means    |                     |
|        |           | here within a section on |                     |
|        |           | one-second data. Replace |                     |
|        |           | with filtered values. To |                     |
|        |           | be included in V-5.1.0   |                     |
|        |           | release.                 |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | JM        | Data quality: proofread  | Completed           |
| M.17** |           | the guide to the process |                     |
|        |           | of despiking data.       |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | SB        | Incorporate              | Completed           |
| M.18** |           | suggestions/corrections  |                     |
|        |           | from the proofread of    |                     |
|        |           | the development V-5.0.0  |                     |
|        |           | to V-5.1.0 release.      |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | GIN       | Validate the following   | Need to be reviewed |
| M.19** | Sub       | information: "1-second   |                     |
|        | committee | data: Available to users |                     |
|        |           | within 30 seconds\" !=   |                     |
|        |           | (6.2.3 page 31) at the   |                     |
|        |           | end \"IMO may not make   |                     |
|        |           | more than 1440 uploads   |                     |
|        |           | per day\"                |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | SB        | Replace the description  | Completed           |
| M.20** |           | on p 47 part of toolkit  |                     |
|        |           | used to create the       |                     |
|        |           | website with the tool    |                     |
|        |           | used on the new GitHub   |                     |
|        |           | environment. Describe    |                     |
|        |           | the various formats (RST |                     |
|        |           | and PDF) and how to      |                     |
|        |           | propose changes for      |                     |
|        |           | external contributors    |                     |
|        |           | etc.                     |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | BSL       | Incorporate changes      | Completed           |
| M.21** |           | proposed by JM to        |                     |
|        |           | include IRDS and replace |                     |
|        |           | CD, DVD and USB with IPM |                     |
|        |           | where appropriate. To be |                     |
|        |           | included in version      |                     |
|        |           | V-5.1.0.                 |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | CT        | Appendix A-1: Many of    | To be done          |
| M.22** |           | the definitions are      |                     |
|        |           | specific to either       |                     |
|        |           | IMFV1.22 or satellite    |                     |
|        |           | transmission data        |                     |
|        |           | formats e.g. "time       |                     |
|        |           | stamp" and "flags". Add  |                     |
|        |           | general terminology      |                     |
|        |           | definitions.             |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | DD        | Issues related the       | Redefinition done   |
| M.23** | Sub       | yearmean files and       | IYV1.03 done        |
|        | committee | IYFV1.01 data format     |                     |
|        |           | including the definition |                     |
|        |           | of the "I -- incomplete" |                     |
|        |           | flag. Do we need a new   |                     |
|        |           | format version?          |                     |
|        |           | Information to be        |                     |
|        |           | provided by the DD       |                     |
|        |           | subcommittee.            |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | BSL       | Appendix C-1: Change use | Not relevant        |
| M.24** |           | of deltaF for "G"        | anymore             |
+--------+-----------+--------------------------+---------------------+
| **T    | JM        | Appendix C-1:            | To be done          |
| M.25** |           | Orientation of "UVZ" has |                     |
|        |           | no definition in Section |                     |
|        |           | 6.1.3 Generate a table   |                     |
|        |           | of the various           |                     |
|        |           | orientations for the     |                     |
|        |           | Technical Manual.        |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | CT        | Appendix C-4: Needs to   | We will delete this |
| M.26** |           | be updated to reflect    | section             |
|        |           | this is software         |                     |
|        |           | supplied on CDs          |                     |
|        |           | 1991-???? and has been   |                     |
|        |           | since been superseded by |                     |
|        |           | imcdview (as described   |                     |
|        |           |                          |                     |  
| **Nu   | Re        | Description              | **tatus Green       |
| mber** | sponsible |                          | completed; Orange   |
|        |           |                          | ongoing; Red not    |
|        |           |                          | started**           |
+--------+-----------+--------------------------+---------------------+
| **     | JM        | Generate a DOI for the   | SB send pdf and     |
| TM.1** |           | next release in RST      | look into           |
|        |           | format for the Technical | possibilities of    |
|        |           | Manual V-5.1.0.          | automate DOI        |
|        |           |                          | creation linked     |
|        |           |                          | with release tags   |
+--------+-----------+--------------------------+---------------------+
| **     | SB        | Publish TM V-5.1.0 once  | Complete            |
| TM.2** |           | the new collaboration    |                     |
|        |           | environment is available |                     |
|        |           | on GitHub.               |                     |
+--------+-----------+--------------------------+---------------------+
| **     | SB        | Configure a dedicated    | Complete            |
| TM.3** |           | environment to           |                     |
|        |           | INTERMAGNET for the TM   |                     |
|        |           | on GitHub.               |                     |
+--------+-----------+--------------------------+---------------------+
| **     | SB        | Configure a dedicated    | Complete            |
| TM.4** |           | environment to           |                     |
|        |           | INTERMAGNET for the TM   |                     |
|        |           | on ReadTheDocs.          |                     |
+--------+-----------+--------------------------+---------------------+
| **     | SB        | Complete the conversion  | Complete            |
| TM.5** |           | of the current version   |                     |
|        |           | of the manual to RST     |                     |
|        |           | (only 3 pages left).     |                     |
+--------+-----------+--------------------------+---------------------+
| **     | TM        | Install the new          | Ongoing (saturday)  |
| TM.6** | sub       | development tools        |                     |
|        | committee | locally and experiment   |                     |
|        |           | with them.               |                     |
+--------+-----------+--------------------------+---------------------+
| **     | CT        | Look at TN and FAQs for  | Not started         |
| TM.7** |           | QD information to be     |                     |
|        |           | added to the TM.         |                     |
+--------+-----------+--------------------------+---------------------+
| **     | JM        | Description on the use   | Complete            |
| TM.8** |           | of DOIs for              |                     |
|        |           | data/metadata            |                     |
|        |           | publication in           |                     |
|        |           | INTERMAGNET.             |                     |
+--------+-----------+--------------------------+---------------------+
| **     | DD        | Provide text for the TM  | Still to do         |
| TM.9** | sub       | on the use of flags as a |                     |
|        | committee | separate metadata field  |                     |
|        |           | (ref. DD31) if this is   |                     |
|        |           | to be adopted in CDF     |                     |
|        |           | format.                  |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | BSL       | Modify Technical Manual  | Completed           |
| M.10** |           | references to the 90%    |                     |
|        |           | rule to state that this  |                     |
|        |           | can be interpreted as    |                     |
|        |           | either 90% of the values |                     |
|        |           | or 90% of the weight of  |                     |
|        |           | the filter. To be        |                     |
|        |           | included in V-5.1.0      |                     |
|        |           | release.                 |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | GIN       | Flagging of data -- how  | Still to do         |
| M.11** |           | to preserve data rather  |                     |
|        | sub       | than deleting it using a |                     |
|        | committee | separate flag data       |                     |
|        |           | field. Is this only for  |                     |
|        |           | CDF or also for other    |                     |
|        |           | formats?                 |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | SB & CB   | Configure URL            | Completed           |
| M.12** |           | intermagnet.org for      |                     |
|        |           | GitHub and ReadTheDocs.  |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | BSL       | Page 5 par 2 ...         | Completed           |
| M.13** |           | recognized format --     |                     |
|        |           | could add a pointer to   |                     |
|        |           | the section in the       |                     |
|        |           | document that describes  |                     |
|        |           | that. Section 6.1.1. To  |                     |
|        |           | be included in V-5.1.0   |                     |
|        |           | release.                 |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | BSL       | In Chapter 2 - not clear | Completed           |
| M.14** |           | what the definitions of  |                     |
|        |           | the data types are --    |                     |
|        |           | add pointer to           |                     |
|        |           | definition/relevant      |                     |
|        |           | text.                    |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | JM        | Section 2.3.9 -- add     | Completed           |
| M.15** |           | text describing where    |                     |
|        |           | the gp ratio is used. To |                     |
|        |           | be included in V-5.1.0   |                     |
|        |           | release.                 |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | BSL       | Page 13 column 1,        | Completed           |
| M.16** |           | paragraph 1 -- It makes  |                     |
|        |           | no sense to me to use    |                     |
|        |           | the examples of means    |                     |
|        |           | here within a section on |                     |
|        |           | one-second data. Replace |                     |
|        |            | in Section 6.4.3.4). To  |                     |
|        |           | be include in version    |                     |
|        |           | V-5.1.0.                 |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | SB & JM   | Add DOI links for all    | To be done SB       |
| M.27** |           | Technical Manual         |                     |
|        |           | versions on the          |                     |
|        |           | INTERMAGNET GitHub WEB   |                     |
|        |           | site.                    |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | CT        | Production of QD-Data;   | Not done            |
| M.28** |           | incorporate JM's         |                     |
|        |           | proposal from the        |                     |
|        |           | updated FAQ (June 2020)  |                     |
|        |           | into the Technical       |                     |
|        |           | Manual or a combination  |                     |
|        |           | of the essentials and    |                     |
|        |           | some references to the   |                     |
|        |           | FAQ.                     |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | TM        | Add a section on Auto    | Status to be        |
| M.29** | Sub       | D&I and Auto Baseline.   | checked             |
|        | committee |                          |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | AL        | Add conditions of use    | Not started         |
| M.30** |           | CC-BY-NC 4.0.            |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | TM        | Check and update all     | Done                |
| M.31** | Sub       | links on the Technical   |                     |
|        | committee | Manual and GitHub WEB    |                     |
|        |           | Site (especially for the |                     |
|        |           | data formats to point to |                     |
|        |           | the TM). To be included  |                     |
|        |           | in V-5.1.0 release.      |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | SB        | Distribute an            | Ongoing             |
| M.32** |           | instruction document on  |                     |
|        |           | "how to submit changes"  |                     |
|        |           | for the INTERMAGNET      |                     |
|        |           | members and also a       |                     |
|        |           | document for external    |                     |
|        |           | submissions.             |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | SB        | Organize video           | Ongoing             |
| M.33** |           | conferences as needed    |                     |
|        |           | for the Technical Manual |                     |
|        |           | subcommittee.            |                     |
+--------+-----------+--------------------------+---------------------+
| **T    | OPSCOM    | Provide decision on new  | Need to be adapted  |
| M.34** |           | members/org chart. To be | to new structure    |
|        |           | included in V-5.1.0      |                     |
|        |           | release.                 |                     |
+--------+-----------+--------------------------+---------------------+

## 

## 

## New items to be added 

##  

+----------------------+-----------------------+-----------------------+
| **TM.35**            | SB                    | Include mqtt/Seedlink |
+----------------------+-----------------------+-----------------------+
| **TM.36**            | SB                    | Delete cd rom         |
|                      |                       | software chapter      |
+----------------------+-----------------------+-----------------------+
| **TM.37**            | AL                    | Include Data Checkers |
|                      |                       | in acknowledgment     |
+----------------------+-----------------------+-----------------------+
| **TM.38**            | TM subcomittee        | Review website and    |
|                      |                       | look if there are     |
|                      |                       | possibilities to more |
|                      |                       | integation with       |
|                      |                       | website               |
+----------------------+-----------------------+-----------------------+
| **TM. 39**           | SB                    | Provide standards on  |
|                      |                       | commit names etc      |
|                      |                       |                       |
|                      |                       | define how to proceed |
|                      |                       | with reviews of pull  |
|                      |                       | requests              |
+----------------------+-----------------------+-----------------------+
| **TM. 40**           | SF                    | Add information of    |
|                      |                       | usage and download    |
|                      |                       | possibility of        |
|                      |                       | definitive data via   |
|                      |                       | the DOIs and specifiy |
|                      |                       | the differences       |
+----------------------+-----------------------+-----------------------+

