# meeting TM subcommittee, September 2025

## Attendees
- Stephan Bracke (SB)
- András Csontos (AC)
- Seiki Asari (SA) 
- Andrew Lewis (AL)
- Chris Turbitt (CT)


## TM Subcommittee agenda, September 2025

* Welcome to the new members
* Review of november 2024 actions items 
* Keep WEB and TM in sync ( p.ex members Intermagnet )
* Technical Manual
  * Plan content of next release with DOI
  * Discussion on release planning
  * New items for future release
* WEB
  * review of open issues
  * work with links to the Technical Manual
  * reduce space usages by replacing year books with links to the World Data Center
  * FAQ maintenance
    * real time data update with mqtt and seedlink


## Action items from September 2025 meeting

|  Number   |   Responsible   | Description                                                                                                                                                                     | Status      |
|:---------:|:---------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------|
| **TM.01** |      AL/SB      | Add the definition of IYFV 1.03 to the TM                                                                                                                                       | Not Started |
| **TM.02** |       CT        | Production of QD-Data; incorporate JM’s proposal from the updated FAQ (June 2020) into the Technical Manual or a combination of the essentials and some references to the FAQ.  | Ongoing     |
| **TM.03** |       SB        | Appendix C-1: G represents ΔF (see description below) but description hard to find                                                                                              | Ongoing     |
| **TM.04** |    SB/AC        | Appendix C-1: Orientation of “UVZ” has no definition in Section 6.1.3 Generate a table of the various orientations for the Technical Manual.                                    | Ongoing     |
| **TM.05** |      JM/SB      | Generate a DOI for the current release V-5.3.0  (SB send PDF)                                                                                                                   | Not Started        |
| **TM.06** |       SB        | Add links to previous version via DOI on the website publications                                                                                                               | Recurring   |
| **TM.07** |       SB        | transform documentation made to contribute into MD locally and remote                                                                                                           | Not Started |
| **TM.08** |       AL        | update organisational structure in TM to align with website                                                                                                                    | Not Started        |
| **TM.09** |       SB        | organise video intermediate videoconferences                                                                                                                                    | Recurring     |
| **TM.10** | DD subcomittee  | Provide text for the TM on the use of flags as a separate metadata field (ref. DD31) (also in CDF)    | Not Started |
| **TM.11** | DD subcomittee  | Add a section on Auto D&I and Auto Baseline.                                                                                                                                    | Not Started |
| **TM.12** | GIN subcomittee | Provide input for  a chapter on MQTT                                                                                                                                            | Ongoing     |
| **TM.13** | TM subcomittee  | review web site and suggest needed corrections and better integration with TM                                                                                                   | Recurring    |
| **TM.14** |       AL        | Update contact info in appendices                                                                                                                                               | Ongoing     |
| **TM.15** |       AC        | Update his name                                                                                                                                                                 | Not Started     |
| **TM.16** |       AL        | Check for broken links on website                                                                                                                                              | Ongoing     |
| **TM.17** |      SB/CT      | Update the FAQ                                                                                                                                                                  | Ongoing     |
| **TM.18** |       SA/SB/CT        | Add doi to document explaining the needs for correct 1 sec data, delete appendix F1                                                                                                                 | Not Started |
| **TM.19** |      CT     | Talk to ashley Smith to see what to do with VirES request    | Not Started     |      
| **TM.20** |      SF     | when bulk data download is done include the data condition of use to it    | Not Started     |                  
| **TM.21** |      CT     | integrate links to the WDC for yearbooks   | Not Started     |  
| **TM.22** |      SB     | permanently delete yearbooks on intermagnet site  | Not Started     |     
| **TM.23** |      TM subcommittee     | Everybody invest in looking for other existing solutions to store docs,pdfs, photos etc on the internet   | Not Started     |                   
| **TM.24** |      TM subcommittee     | study how to maximise use of git compared to document archive   | Not Started     |                   
| **TM.25** |      ?     | Review and update chapter 6.4.3.2 Definitive 1 Minute data there is overlap with appendix C  | Not Started     |                   


## Discussions during meeting

###  Problem of keeping in sync the different sources

Currently there are three places which have an overlap of certain items :

* git repository www.intermagnet.org
* git repository tech-man.intermagnet.org
* document archive at BGS

To limit the duplications we will try to maximise the work with links. 

For what the team members list is concerned we need to monitor it ourself and whenever we see inconcistency we should update the other source as well.
The problem comes when someone updates the table directly on the master branch to the website. We will not be warned by mail of these changes. SB will
try to monitor this more closely. So we will be able to synchronise it almost immediately with the technical manual.
AL will update the member table in the technical manual TM.08.

The document archive is a private archive and only maintainable by CT. CT will see if there are items we can move to GIT so everybody can maintain this content.

Related to this issue SB will restructure the FAQ section and reformat it  into plain markdown. It will make it simple to maximize answers to the FAQ with links to the technical manual instead
of introducing the same content two times.



### Define UVZ variometer orientation

Currently in the TM there is sometimes a mention of UVZ orientation but this orientation is not documented in the TM.
It is mentioned 12 times in the appendices in intermagnet format definition IBF and IAF.
AC found an article on the internet https://onlinelibrary.wiley.com/doi/10.1155/2018/1804092 
It mentions  *decided to orient the sensor to the “UVZ” orientation. This means that the two horizontal axes are oriented ±45° from local meridian*
AC will search and try to find correct information. 
During the discussion Jean Rasson was mentioned and SB will try to find out if he has some clean definition on that one.

CT send  a almost complete table of all components used with their standardized Indication

| Code  |  Description    |
|:-----:|---------------|
|  X    |  North Component. The strength of the magnetic field vector in the geographic north direction (southerly values are --ve). |
|  Y    | East component. The strength of the magnetic field vector in the geographic east direction (westerly values are –ve). | 
|  Z    |  Vertical intensity. The strength of the magnetic field vector in the vertical direction. Z is upward positive downwards and hence negative in the southern hemisphere. |
|  H    |  Horizontal intensity. The strength of the magnetic field vector in the horizontal plane along the magnetic meridian. |
|  D    |  Declination or variation. The angle between the magnetic vector and true north positive east. |
|  I    |  Inclination. The angle between the magnetic vector and the horizontal plane, in degrees of arc, positive above the horizontal. |
|  F    |  Total field intensity. The geomagnetic field strength, calculated from and consistent with XYZ or HDZ field elements. |
|  S    |  Scalar field intensity. The geomagnetic field strength, measured using an instrument that is independent from that used to measure the vector field values. |
|  G    |  Delta-F. Delta-F is defined as F(vector)--S(scalar) in nT. When calculating values for the G element, if F(vector) is missing, G is set to --S (scalar) |
|  E    |  A field strength in the horizontal plane perpendicular to 'H'. 'E' is only valid for data that is not baseline corrected. |
|  V    |  The field strength along the direction of the inclination. |
|  A    |  NW component. |
|  B    |  NE component, 'B' is perpendicular to 'A'. |

WYZHDIF are mentioned and shown with a drawing in 6.1.3. The other ones are derived or slightly variants but should also be included and defined in the TM on a central place.

For UVZ we will have a problem because V will end up with two different meanings.
No clear decision was made during this meeting but AC and SB will try to go into more detail and find out how to integrate it in the TM.

During investigation SB find out that there is a overlap with chapter 6.4 and appendix C so he added TM.25 that needs to be assigned to someone during the next online meeting.

 
### Need for more info on how to produce intermagnet 1 sec data

SA makes a valuable remark that in the TM there is no definition on how to produce 1 sec data that applies to the Intermagnet standard for 1 sec data.
He refers to the appendix F.2 that has the title "Filter Coefficients to Produce One Second Value" but the coefficients where never mentioned.
CT explains that there is a lot more to that then simple list of filter coefficients, he however mentions that there are some documents that explain it 
more in detail but it can be specific for the type of variometer. As action point we should at least delete this F.2 appendix title.
As extra we can make references to all other existing documents that defines these specifications. CT will provide if possible doi or link to these documents.

### Reduce space usage of the www.intermagnet.org repository

This item was discussed in issue [92](https://github.com/INTERMAGNET/intermagnet.github.io/issues/92)
Currently used space is 1,5 GB. Guidelines of GIT advise to not go over 5 GB.
While pointing the yearbooks with a link to the yearbooks on the WDC site we will gain already 503MB which is 33 % of the current usage.
For the moment these links are not available but CT will follow this up.(TM.23)
This is for the moment enough but other solutions (a public ducument archive) to further reduce the disk space should be investigated (TM.24)

### Release Planning

As already discussed previously we will go for an yearly official release with DOI around the time of the next meeting.
Version numbers will be treated as followed major.minor.cor: 

* Major Release : a new subject is introduced into the manual
  * example :  MQTT for near real time data
* Minor Release : a significant change to the content without introducing new concepts or the yearly release with a specific DOI
  * example : new version of an already existing standard
* Corrections  (cor) :
  * Typically language errors , errors in formula, etc
     
###  Next Release : 5.3.0

Next release will be done shortly after the meeting in RIO.

* action items from rio TM01, TM03,TM05, TM22, TM09 see [Rio Action Items](https://github.com/INTERMAGNET/wg-tech-man/blob/main/meetings/2024_11_rio/2024_11_rio_meeting_minutes.md)
* Corrected formula remarked by Marcos (6.5) issue[ #14](https://github.com/INTERMAGNET/imag-tech-man/issues/14)
* Updated members table TM.08
  

### Not handled during meeting

* Extra admins for readthedocs
* New items for future release :
  * DD.11 : Development  a new version IBFV base line format to account for manual and automatic measurements
  * DD.10 		Update Technical Manual - Data checking 1-minute


