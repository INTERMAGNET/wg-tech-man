# meeting TM subcommittee, October 2026

## Attendees
- Stephan Bracke (SB)
- András Csontos (AC)
- Seiki Asari (SA) 
- Andrew Lewis (AL)
- Chris Turbitt (CT)


## TM Subcommittee agenda, October 2026

* Review of actions items may 2026
* Keep WEB and TM in sync (maximize links with TM)
* Technical Manual
  * rewriting of chapter 6 (originally include explanation mqtt into the TM)
  * closure and needed cleaning on definition uvw in sensor orientation and components
  * New items for future release
* WEB
  * review of open issues
  * work with links to the Technical Manual
  * reduce space usages by replacing year books with links to the World Data Center
  * FAQ maintenance
  
## Recap of taken decisions during online meeting

### responsibilities

  * CT and AL added as administrators on Read the docs
  * SA will follow up of needed new requirements coming from the DD ex
    * DD.12 : Development of a new version IBFV base line format to account for manual and automatic measurements
    * DD.10/11 :	Update Technical Manual - Data checking 1-minute (cookbook)
    * flagging chapter (is it still ongoing)

### UVZ orientation

UVZ is mentioned in the IYVF (yearly means) and the IAF (binary archives) formats as a possible sensor orientation.
We distinguish between sensor orientation and components as components are values measured in nT or degrees in case of D and I
We found article on the internet where uvz was used as being  two horizontal axes are oriented ±45° from local meridian.

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
|  V    |  The field strength along the direction of the inclination.  **_'V' is only valid for data that is not baseline corrected._** |
|  A    |  **_magnetic_** NW component. |
|  B    |   **_magnetic_** NE component, 'B' is perpendicular to 'A'. |

* E and V as this definition is only defined in IAGA2002 and not in intermagnet standards 
* The whole table with exception of A, B is indicated as valid values for CDF
* Do we need to add  S,G,E,V to our current component explanation.
* A B is never mentioned as component
* Is for everyone the direction of the inclination clear ?

What is missing is a vector sensor orientation table

Fluxgate variometers usually have 3 orthogonal fluxgate sensors. These sensors can be oriented in various ways.

| Code  |  Description    |
|:-----:|---------------|
|  UVW    | rondom oriented instrument need of two angles to be able to transpose it to defined coordinate system   |
|  DHZ    | two horizontal sensors are oriented towards magnetic north (H) and east, the third is vertical  |
|  XYZ   |  two horizontal sensors are oriented towards geographic north and east, the third is vertical |
|  DIF    | one sensor is oriented along the field vector (F), one sensor horizontal towards magnetic east, and one sensor perpendicular to the other two sensors  |
|  ABZ    | two horizontal sensors are oriented towards magnetic north west (A) and north east, the third is vertical   |


ACTION TO BE TAKEN : review of baseline calculation DHZ explained in 6.5


exception :

in the IBF it is mentioned as component. AL has processed and searched IBF files but didn't find any example of this. 
As it is in a component it meas that it conflicts withe the iaga definition of V component (nT along F vector)



## Action items from September 2025 meeting

|  Number   |       Responsible       | Description                                                                                                                                                                      | Status       |
|:---------:|:-----------------------:|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------|
| **TM.01** |          AL/SB          | Add the definition of IYFV 1.03 to the TM | Done  |
| **TM.02** |           CT            | Production of QD-Data; incorporate JM’s proposal from the updated FAQ (June 2020) into the TM or a combination of the essentials and some refs to the FAQ | Ongoing|
| **TM.03** |           CT            | ADD explanation  of SGEVAB (UV) in the TM accompagnied with a illustration in the same style as the explanations of XYZHDI in Section 6.1.3       | not started    |
| **TM.04** |           SB            | Add links to previous version via DOI on the website publications| Recurring    |
| **TM.05** |           SB            | transform documentation made to contribute into MD locally and remote | not started |
| **TM.06** |           SB            | organise video intermediate videoconferences | Recurring    |
| **TM.07** |     DD/SA      | Provide text for the TM on the use of flags as a separate metadata field (ref. DD31) (also in CDF) |Not Started  |
| **TM.08** |     DD/SA      | Add a section on Auto D&I and Auto Baseline. |Not Started  |
| **TM.09** |     GIN/SB     | Provide input for  a chapter on MQTT |Ongoing|
| **TM.10** |     TM subcomittee      | review web site and suggest needed corrections and better integration with TM | Recurring    |
| **TM.11** |           AL            | Check for broken links on website | Ongoing      |
| **TM.12** |          CT          | Update the FAQ with links to TM if possible | Ongoing      |
| **TM.13** |     SA/SB/CT            | Add doi to document explaining the needs for correct 1 sec data, delete appendix F1 | Not Started  |
| **TM.14** |           CT/JM            | Talk to ashley Smith to see what to do with VirES request/widen up the discussion on higher level  about adding links to external data providers |ongoing |
| **TM.15** |           SF            | when bulk data download is done include the data condition of use to it | Not Started  |
| **TM.16** |           CT            | integrate links to the WDC for yearbook| investigating|
| **TM.17** |           SB            | permanently delete yearbooks on intermagnet site| Not Started  |
| **TM.18** |     TM subcommittee     | Everybody invest in looking for other existing solutions to store docs,pdfs, photos etc on the internet| Not Started  |
| **TM.19** |     TM subcommittee     | study how to maximise use of git compared to document archive | Not Started  |
| **TM.20** |     AL     |  revisit definition of reported and adjusted data / update what is needed for intermagnet| Not Started  |
| **TM.21** |     DD/CT   | need of extra metadata when GNSS is used for mark azimuth determination | Not Started  |
| **TM.22** |    TM subcommittee  | review TM  look at outdated chapters that could be removed or updated. |Not Started  |
| **TM.23** |      TM subcommittee     | study how to maximise use of git compared to document archive  | Not Started |



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


     
###  Next Release : 
  



