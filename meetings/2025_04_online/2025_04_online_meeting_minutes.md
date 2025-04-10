# Report of online meeting of TM Subcommittee, 10 April 2025

## Attendees
 
- Stephan Bracke (SB)
- Jürgen Matzka (JM) (partial)
- Seiki Asari (SA) (partial)
- Andrew Lewis (AL)
- Chris Turbitt (CT)

## Agenda

1. Review/Recap work and evolution of  website intermagnet.org (repo: intermagnet.github.io) 
2. Review/Recap work and release planning on technical manual (repo: imag-tech-man)
3. Overview and update status of action points

## intermagnet.org

During the overview of the website we agreed on :
 
+ We will delete the telephone numbers on the contact page (also on the technical manual same for fax numbers)
+ For the issue of the space limit recommended by GIT (https://github.com/INTERMAGNET/intermagnet.github.io/issues/92)
  - CT will check if BGS already stores the yearbooks ( they take up half a gigabyte)
  - We could also make a separate repo for the yearbooks and reference them (to be decided on next meeting)
+ Everybody will see look for opportunities to avoid double work and reference to the technical manual instead of recreating a page on the website


## tech-man.intermagnet.org

+ New changes done and accepted on the main/master stream : A new version will be released shortly after the meeting (5.2.0) and will get a new DOI (JM confirmed this)
+ On the read the docs https://about.readthedocs.com/?ref=readthedocs.org you can create an account (free community edition). 
  - We can link it with the github account
  - When done SB will add you to the maintainers list of the read the docs
+ There is a problem on the readthedocs site when commiting a lot of changes the automated generation doesn't  update the PDF version immediately 
  - SB created a ticket for this but it isn't resolved yet
+ Also the contact page has fax and telephone numbers this will be cleaned up by AL and SB will give support if needed

## Status of action items

All status were evaluated and updated.
An overview can be found here https://github.com/INTERMAGNET/wg-tech-man/blob/main/meetings/2024_11_rio/2024_11_rio_meeting_minutes.md








## Work methods on GIT 

1. Any enhancements, ideas, changes needed, etc can quickly be documented by a creation of an issue on the work group,https://github.com/INTERMAGNET/wg-tech-man/issues 
2. Any Changes on the imag-tech-man **ALWAYS** need to be done on a separate branch **NEVER** on the main branch and integrated via a pull request (always reviewed).
3. Big changes to the www.intermagnet.io are **preferably** done on a separate development branch, although we can accept small changes/spelling corrections directly on the main branch.
4. In the wg-tech-man repository changes can be done directly on the main branch.

### Remarks

During normal use we don't risk to have many conflicts because we rarely will change the same file.
Pull requests via a  own branch separates the work and garantees a review which is necessary for any change on the technical manual. 
The issues list is there to quickly note something down that can be treated later on.
SB can always do a personal online meeting when in need of extra support or guidelines 
