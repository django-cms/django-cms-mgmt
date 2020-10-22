# Tech Committee - Tasks and Decisions Log

<small>The Tech Committee meetings documentation must follow the format of the [Tech Committee Log Entry Template](/tech-committee/tasks-and-decisions-log-entry-template.md)</small>

[ℹ️ See here for all Tech Committee tasks](https://github.com/django-cms/django-cms-mgmt/projects/1)

[ℹ️ See here for the live version](https://hackmd.io/ddhvq_aqS6my9gwhLddyPg)

## Friday 23.10.2020 (WiP, upcoming Meeting)
#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. add new entry for next meeting from template
1. Guest intro
    - Narender 
1. Varia: further points raised by Tech Committee members
    - Go or No Go: Release 3.8.0
    - Review of Assignment: Andrew and Nicolai to look at and clarify left-over PRs and propose workgroups from them
    - Review of Assignment: Mario presents proposal for mid-/long-term roadmap (features / improvements) for publication on the website (for marcom / Nicolai)
    - django CMS 4 workgroup setup & announcement
    - Update Iacopo regarding get_translatable_content enquiry
1. news & updates for dCA MarCom
1. review log entry together, approve and post


## Friday 16.10.2020 (WiP, current Meeting)
#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. add new entry for next meeting from template
1. Guest intro
    - Alex 
        - Nicolai to sent Alex follow up email and guide him through the next steps
3. Varia: further points raised by Tech Committee members
    - Review all proposed [workgroups](https://docs.google.com/spreadsheets/d/1gfI8IKz84u-YvE61eePCD-lAbn1haghOiqkvSdO-1yg/edit#gid=1074764488) together in this TC meeting. Also check [workgroups documentation](https://github.com/django-cms/django-cms-mgmt/blob/master/work%20contribution/work%20groups.md)
        - Approved by everyone present
    - [Update PR closing process](https://docs.google.com/document/d/1TaJ0dIBuA_8_k2FphOFatNkQjhNSKj9qSFZ_rSEOJj0/edit) -> [Example](https://github.com/django-cms/django-cms/pull/6758#event-3756117723)
        - Next steps: Nicolai to check whether to add another scenario to the template that fits to the example case (ask Andrew)
    - Review of Assignment: Victor reports on 3.8 CMS testing, Victor to onboard Lisa for testing
        - djangocms 3.8 & django 3.0 has been deployed to 3 projects on the last week
            - the codebase utilized
                - https://gitlab.com/effective-altruism/ea-cms-template
                - https://gitlab.com/what-digital/djangocms-template
        - Next steps: Nicolai to help onboard Lisa in order to upgrade django-cms demo to 3.8
    - Review of Assignment: Victor / Andrew report on djangocms-url-manager / djangocms-link rewrite plans (3.7 compatibility is confirmed) -> Nicolai to create workgroup(s) with Andrew / Victor on it.
        - Next steps:
            - Andrew: to attach a link to a working cms 4 server
            - Victor: to share a url to a public server with djangocms-link-all
            - we created a new channel on slack `workgroup-new-link-plugin` - the details are there
    - Review of Assignment: Andrew to do an intro with his contact for a django CMS 4 demo. Mario reports on django CMS v4 demo schedule
        - Next steps: Demo scheduled to be presented to Victor 
    - django CMS 3.8.0 release schedule
        - Next steps: TC to give Go for Gold Release next TC meeting. Release scheduled for Wednesday after TC meeting
    - New feature request: Iacopo updates regarding a feature request (export / import of page trees) from a client
        - Next steps:
            - Victor: to invite Vlad to dca slack channel, create a workgroup channel for it, ask him to find the existing codebase
            - Iacopo to update TC on feature request after more exploration/analysis
    - Support enquiry regarding get_translatable_content removed in https://github.com/django-cms/django-cms/commit/b1d1d50fac1532dfa650fe7ea2dfa8e85727fec0
        - Next steps
         - Iacopo will get in contact with the person who closed the PR and report back on the status to the next TC meeting. 
    - Feedback on guest post topics https://docs.google.com/spreadsheets/d/1jNCtIUDmsj-qZZPe7yq73umR7FGra_3H39hqTjgvyAQ/edit#gid=1394201430
        - No feedback 
4. news & updates for dCA MarCom
        - Workgroup announcement 
6. review log entry together, approve and post


## Friday 09.10.2020 (WiP, current Meeting)
#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>
1. add new entry for next meeting from template
1. Guest intro
    - Samuel: specific painpoints > Nicolai to set up workgroups and appoint TC members
        - caching issues (docs / using django cache) Iacopo would like to join
        - page tree page in django admin scalability issues and broken search for sub-pages (Jacob Rief has insights here regarding scalability, we need to ask him to join this workgroup, Andrew has done a lot of pagetree changes incl. SQL optimisations for dCMS v4 and could advise on this as well)
1. Varia: further points raised by Tech Committee members
   - review areas of responsibility and fill in : https://docs.google.com/document/d/1UPnQ81s0EaXfOJ3gggj31U-TLGmMUv33aFecEcf0nag/edit
   - Group discussion: How do we organize volunteers / contributors?
       - contribution process
           - welcome contributors and show the "clubhouse" > Nicolai
           - show them the different workgroups
           - use existing google spreadsheet as workgroup directory
           - one person of each workgroup should come to the TC meeting every once in a while (TBD)
       - workgroups examples:
           - pressing issues (ready for implementation) 
               - workgroup "xy"
           - django CMS v4 review workgroup
           - headless market research workgroup
           - ...
1. news & updates for dCA MarCom
   - discourse.django-cms.org setup is finished and can officially be launched
1. review log entry together, approve and post
1. django CMS 3.8.0 release schedule

<small>After the meeting, create and link tasks and update the entry</small>

#### Decisions taken
<small>Any other decisions taken during the meeting are documented here, since all decisions must be actionable, a task must be created from it.</small>
- ...
- ...


## Friday 02.10.2020

#### Agenda Points
1. add new entry for next meeting from template
1. Guest intro
1. tasks to review
1. Varia: further points raised by Tech Committee members
   - 3.8 RC testing
   - proposal to accept guests in TC meetings
   - looking for owners for the following areas of responsibilities:
      - Release mgmt & QA
      - PR expert assignment
      - django-cms.org improvements
      - django CMS demo maintenance + improvements
      - technical support (SO, discourse, github issues)
      - Discourse
   - Nicolai: Populate roadmap with features
   - Mario: remove PR and feature requests / issues from the agenda points
   - Victor: Can I djangocms-links and djangocms-picture?
1. news & updates for MarCom
   - areas of ownership: some filled, for some we need call for volunteers
1. review log entry together and approve

#### Tasks to review
- [ ] [respond to open merge requests on the core](https://github.com/django-cms/django-cms-mgmt/issues/1)
- [ ] [create a definition of what changes are required in v4 to switch community efforts to v4 and abandon v3](https://github.com/django-cms/django-cms-mgmt/issues/2)


#### Decisions taken
- Victor volunteered to do RC 3.8 testing next week
- TC guests and guest process approved
- Victor to be owner of area of responsibility "django CMS demo maintenance + improvements"
- deprecate and phase out Google mailing list
- officially announce discourse.django-cms.org
- areas of ownership approved as per Varia
- Andrew to be owner of area of responsibility "technical support (SO, discourse, github issues)" and "PR expert assignment"
- Approved: remove PR and feature requests / issues from the agenda points
- Regarding Victor's request: djangocms-link is part of LTS, any change to it must be backward compatible, Victor & Andrew to sync on djangocms-url-manager, to report on it.
- Regarding Victor's request: djangocms-picture is part of LTS, any change to it must be backward compatible.

## Friday 25.09.2020
#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>
1. add new entry for next meeting from template
2. tasks to review
3. pull requests to process
4. feature requests and issues to process
5. Varia: further points raised by Tech Committee members
   - Mario: to conduct a survey about the headless proposal
6. review log entry together, approve and post

#### Tasks to review
- [ ] [respond to open merge requests on the core](https://github.com/django-cms/django-cms-mgmt/issues/1)
- [ ] [create a definition of what changes are required in v4 to switch community efforts to v4 and abandon v3](https://github.com/django-cms/django-cms-mgmt/issues/2)

#### Decisions taken
<small>Any other decisions taken during the meeting are documented here, since all decisions must be actionable, a task must be created from it.</small>
- set up forum at discourse.django-cms.org
- process for feature requests (including UX / Design guidelines) to be documented (volunteers needed)
- conduct survey on django CMS headless proposal


## Friday 17.09.2020
#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>
1. add new entry for next meeting from template
2. tasks to review
3. pull requests to process
4. feature requests and issues to process
5. Varia: further points raised by Tech Committee members
   - RFP / Feature request process: Propose to use discourse and [discourse voting plugin](https://meta.discourse.org/t/discourse-voting/40121) - this would completely replace the [Fider setup](https://gitlab.com/what-digital/django-cms-association/-/issues/184)
      - all feature requests that are posted as issues on the respective repositories would be tagged as feature requests, a discourse topic would be opened and the link referenced in the issue, the issue would be tentatively closed in the repo, and a discussion period would start on discourse, in which everyone would participate, including members of the tech committee. The tech committee then would review the results from the discussion period and would then either discard or accept into the roadmap.
6. review log entry together, approve and post

<small>After the meeting, create and link tasks and update the entry</small>
#### Tasks to review
- [ ] [respond to open merge requests on the core](https://github.com/django-cms/django-cms-mgmt/issues/1) - postponed
- [ ] [create a definition of what changes are required in v4 to switch community efforts to v4 and abandon v3](https://github.com/django-cms/django-cms-mgmt/issues/2) - postponed
#### New Pull Requests
- This is for the moment handled via the pending cleanup task
#### Feature Requests and Issues
- We will postpone issue mgmt to after we've cleaned up the pending PRs.
#### Decisions taken
- we will set up Discourse with a voting plugin for feature voting
- we will abandon the idea to use fider since Discourse can do that well via feature voting plugin
- moving meeting back to 14:00 because Divio team members already have weekly meetings at 15:00


## Friday 11.09.2020
#### Tasks to review
- [x] Mario to create the markdown structure of the wiki on wiki github repo
#### Decisions taken
- we want to gather feedback for all open PRs from all TC members and the PR creator, to either close, fix or reassign PRs
- wiki format is approved and will be used from now on


## Friday 04.09.2020
#### Decisions taken
- move gitlab board to new github project board for dCA activities
- Mario to create the markdown structure of the wiki on wiki github repo
- review https://github.com/divio/django-cms/pulls and propose the easy ones to merge for 3.8
- get free slack account for django CMS Association
- create a definition of what changes are required in v4 to switch community efforts to v4 and abandon v3.
- Andrew to look at two pending PRs on django CMS core

