# meeting TM subcommittee, online 05/26

## Attendees
- Stephan Bracke (SB)
- András Csontos (AC)
- Seiki Asari (SA) 
- Andrew Lewis (AL)
- Chris Turbitt (CT)


## TM Subcommittee agenda

* need of backup admin for readthedocs (CT and AL ?)
* need a person to follow up the DD committee (SA or AC) 
  * every communication with the DD committee:
    * DD.11 : Development of a new version IBFV base line format to account for manual and automatic measurements
    * DD.10 :	Update Technical Manual - Data checking 1-minute (cookbook)
    * flagging chapter
* plan next major release 6.0 
  * Add chapter on MQTT (SB/SF)
  * Add the definition of IYFV 1.03 to the TM (AL)
* Review of particular action items from previous meeting
* Review action items from previous meeting

## Review of particular action items from previous meeting

* TM.01: Add the definition of IYFV 1.03 to the TM (AL/SB)
  * create branch TM01_ADD_NEW_VERSION_IYFV_1.03 : change archive data format title (remove version number and make two subsections 1.02, 1.03)
  * examples of formula can be found here : [calc pillar diff](https://tech-man.intermagnet.org/stable/chapters/absmeasurements/calcdiffpillar.html) or
  [def data calc](https://tech-man.intermagnet.org/stable/chapters/submitdata/defdatacalc.html)
  * reminder on header policies see [rst headers](../../docs/rst_headers.md)
    * reference pdf can be found [here](./doc/IYFV_AL-20240702bw.pdf)

* TM.04: Appendix C-1: Orientation of “UVZ” has no definition
   * see [issue 9](https://github.com/INTERMAGNET/wg-tech-man/issues/9)
   * replace UVZ with ABZ.
   * action to be taken new Action Item: create a section or add it Section 6.1.3 to on the explanation of SGEVAB in the TM.
     and also link it in the faq.
* TM.17 : to be able to make links to the TM from within the FAQ we needed to restructure the FAQ section and reformat it  into plain markdown.
  * done see https://github.com/INTERMAGNET/intermagnet.github.io/tree/master/faq

* New item on confusion of what reported data is because the definition says that the data is not baseline corrected,
  but intermagnet expects that the data send is at least baseline corrected.
  * so while in different locations on site and in TM we say that reported data can be send we mean reported data with baseline correction
  * mails were send to discuss on that issue some conclusions:.
    * We will retain the definition of “reported” data to avoid confusion and allow for the possibility of future variation stations. 
      Hence IMOs need to submit baseline corrected real-time data as “adjusted” data. A note will be send (12 month delay between notifying IMOs and making the change)
    * Review and updates need to be made to the TM/web site to reflect this change and avoid confusion (AL ?)

* New item : everyone reviews tm and looks at outdated chapters that could be removed or updated.



| Code | Description                                                                                                                                                            |
|:----:|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|  X   | North Component. The strength of the magnetic field vector in the geographic north direction (southerly values are --ve).                                              |
|  Y   | East component. The strength of the magnetic field vector in the geographic east direction (westerly values are –ve).                                                  | 
|  Z   | Vertical intensity. The strength of the magnetic field vector in the vertical direction. Z is upward positive downwards and hence negative in the southern hemisphere. |
|  H   | Horizontal intensity. The strength of the magnetic field vector in the horizontal plane along the magnetic meridian.                                                   |
|  D   | Declination or variation. The angle between the magnetic vector and true north positive east.                                                                          |
|  I   | Inclination. The angle between the magnetic vector and the horizontal plane, in degrees of arc, positive above the horizontal.                                         |
|  F   | Total field intensity. The geomagnetic field strength, calculated from and consistent with XYZ or HDZ field elements.                                                  |
|  S   | Scalar field intensity. The geomagnetic field strength, measured using an instrument that is independent from that used to measure the vector field values.            |
|  G   | Delta-F. Delta-F is defined as F(vector)--S(scalar) in nT. When calculating values for the G element, if F(vector) is missing, G is set to --S (scalar)                |
|  E   | A field strength in the horizontal plane perpendicular to 'H'. 'E' is only valid for data that is not baseline corrected.                                              |
|  V   | The field strength along the direction of the inclination.                                                                                                             |
|  A   | NW component.                                                                                                                                                          |
|  B   | NE component, 'B' is perpendicular to 'A'.                                                                                                                             |




## Action items from September 2025 meeting

|  Number   |       Responsible       | Description                                                                                                                                                                      | Status       |
|:---------:|:-----------------------:|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------|
| **TM.01** |          AL/SB          | Add the definition of IYFV 1.03 to the TM                                                                                                                                        | Not Started  |
| **TM.02** |           CT            | Production of QD-Data; incorporate JM’s proposal from the updated FAQ (June 2020) into the Technical Manual or a combination of the essentials and some references to the FAQ.   | Ongoing      |
| **TM.03** |           SB            | Appendix C-1: G represents ΔF (see description below) but description hard to find                                                                                               | see TM 4     |
| **TM.04** |          SB/AC          | Appendix C-1: Orientation of “UVZ” has no definition in Section 6.1.3 Generate a table of the various orientations for the Technical Manual.                                     | Ongoing      |
| **TM.05** |          JM/SB          | Generate a DOI for the current release V-5.3.0  (SB send PDF)                                                                                                                    | DONE         |
| **TM.06** |           SB            | Add links to previous version via DOI on the website publications                                                                                                                | Recurring    |
| **TM.07** |           SB            | transform documentation made to contribute into MD locally and remote                                                                                                            | PDF enough ? |
| **TM.08** |           AL            | update organisational structure in TM to align with website                                                                                                                      | DONE         |
| **TM.09** |           SB            | organise video intermediate videoconferences                                                                                                                                     | Recurring    |
| **TM.10** |     DD subcomittee      | Provide text for the TM on the use of flags as a separate metadata field (ref. DD31) (also in CDF)                                                                               | Not Started  |
| **TM.11** |     DD subcomittee      | Add a section on Auto D&I and Auto Baseline.                                                                                                                                     | Not Started  |
| **TM.12** |     GIN subcomittee     | Provide input for  a chapter on MQTT                                                                                                                                             | Ongoing      |
| **TM.13** |     TM subcomittee      | review web site and suggest needed corrections and better integration with TM                                                                                                    | Recurring    |
| **TM.14** |           AL            | Update contact info in appendices                                                                                                                                                | Done         |
| **TM.15** |           AC            | Update his name                                                                                                                                                                  | Done         |
| **TM.16** |           AL            | Check for broken links on website                                                                                                                                                | Ongoing      |
| **TM.17** |          SB/CT          | Update the FAQ                                                                                                                                                                   | Ongoing      |
| **TM.18** |     SA/SB/CT            | Add doi to document explaining the needs for correct 1 sec data, delete appendix F1                                                                                              | Not Started  |
| **TM.19** |           CT            | Talk to ashley Smith to see what to do with VirES request                                                                                                                        | Not Started  |      
| **TM.20** |           SF            | when bulk data download is done include the data condition of use to it                                                                                                          | Not Started  |                  
| **TM.21** |           CT            | integrate links to the WDC for yearbooks                                                                                                                                         | Not Started  |  
| **TM.22** |           SB            | permanently delete yearbooks on intermagnet site                                                                                                                                 | Not Started  |     
| **TM.23** |     TM subcommittee     | Everybody invest in looking for other existing solutions to store docs,pdfs, photos etc on the internet                                                                          | Not Started  |                   
| **TM.24** |     TM subcommittee     | study how to maximise use of git compared to document archive                                                                                                                    | Not Started  |                   




### Need for more info on how to produce intermagnet 1 sec data

SA makes a valuable remark that in the TM there is no definition on how to produce 1 sec data that applies to the Intermagnet standard for 1 sec data.
He refers to the appendix F.2 that has the title "Filter Coefficients to Produce One Second Value" but the coefficients where never mentioned.
CT explains that there is a lot more to that then simple list of filter coefficients, he however mentions that there are some documents that explain it 
more in detail but it can be specific for the type of variometer. As action point we should at least delete this F.2 appendix title.
As extra we can make references to all other existing documents that defines these specifications. CT will provide if possible doi or link to these documents.

### Release Planning

As already discussed previously we will go for an yearly official release with DOI around the time of the next meeting.
Version numbers will be treated as followed major.minor.cor: 

* Major Release : a new subject is introduced into the manual
  * example :  MQTT for near real time data
* Minor Release : a significant change to the content without introducing new concepts or the yearly release with a specific DOI
  * example : new version of an already existing standard
* Corrections  (cor) :
  * Typically language errors , errors in formula, etc



