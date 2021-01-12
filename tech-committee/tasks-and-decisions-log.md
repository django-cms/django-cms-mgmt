# Tech Committee - Tasks and Decisions Log

<small>The Tech Committee meetings documentation must follow the format of the [Tech Committee Log Entry Template](/tech-committee/tasks-and-decisions-log-entry-template.md)</small>

- [Tech Committee task board](https://github.com/django-cms/django-cms-mgmt/projects/1)
- [this doc's hackmd url](https://hackmd.io/ddhvq_aqS6my9gwhLddyPg)
- [this doc's github repo url](https://github.com/django-cms/django-cms-mgmt/blob/master/tech-committee/tasks-and-decisions-log.md)

## 15.01.2021 (Next Meeting)

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest intro
3. Review agenda and add missing points
4. Varia: further points raised by Tech Committee members
    - Approval of TC membership applications
    - What template format the developers would need (Victor) - it was meant for "Varia"
        - we could aim to provide
            - a CLI
            - a project example as djangocms-template
            - both CLI and a project example?
            - a project example with cookiecutter
        - adding it to a general community survey could be a good idea
        - tech brief draft - https://hackmd.io/@django-cms/workgroup-project-template
6. Review Tasks
7. News & updates for / from dCA Board and MarCom
8. Review approve and post the meeting notes

#### Tasks & Initiatives
- [ ] Give Vinit access to github org (Mario)
- [ ] Record basic demo videos/a series of django CMS 4.0 to recruit volunteers for the workgroup (Andrew)
- [ ] Mario to review https://jazzband.co/ and report on standardization strategies in next TC
- [ ] Mario / Andrew to add code to v4 demo project repo
- [ ] Andrew to release 3to4 script in repo
- [ ] announce Testing & QA Contribution Program for service providers (for Nicolai)
- [ ] Nicolai to onboard 2 devs from Compound Partners into v4 workgroup
- [ ] Nicolai to organize design / ux direction (initially for django-filer svg enhancement, but with a bigger perspective in the mid term for django CMS v4 Community Release and headless django CMS initiatives
- [ ] set up testing log (google spreadsheet?) - Nicolai
- [ ] Formally phase out python 3.5 for `develop` branch (for upcoming v3.9) (Jacob Rief)
- [ ] Provide db/media dump to Jacob Rief (Jacob Rief to ask Victor)
- [ ] Set up CI/CD Pipeline (Jacob Rief) for PR and branch test servers
- [ ] set up "search" workgroup and onboard workgroup members (proposal: focus on https://github.com/divio/djangocms-internalsearch for django CMS 4?) (Nicolai/Andrew)
- [ ] search result workgroup to create a test link (Jean-Baptiste)
- [x] Invite django CMS 4 developers to documenation workshop (Andrew) 


## 08.01.2021 

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest intro
3. Review agenda and add missing points
4. Varia: further points raised by Tech Committee members
   - Andrew: Progress update from CI workgroup kick-off call
   - Nicolai: Request admin access to djangocms github org for Vinit for setting up github actions
   - Nicolai: Update PR Review workgroup - Information needed (Tech Brief etc.) - I nominate Iacopo as workgroup lead 
   - Mario: switch django CMS Slack org to use google meet for calls (slack call is disabled anyways due to free plan restrictions)
   - Andrew: django CMS 4 Migration
5. Review Tasks
6. News & updates for / from dCA Board and MarCom
   - Mario: [django CMS Roadmap / Vision / Strategy 2021 Update from the dCA board](https://docs.google.com/presentation/d/1P-CObPTKt6dodqYhYJKNBFE4mb3jv0jVr17iOfBBcl0/)
8. Review approve and post the meeting notes

#### Tasks & Initiatives
- [x] Create a PR review workgroup (Nicolai)
- [x] Write copy for documentation and send to Daniele for merging into production (Nicolai)

## 18.12.2020

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest intro
3. Review agenda and add missing points
4. Varia: further points raised by Tech Committee members
    * Update from search result workgroup (Jean-Baptiste)
        * A PR has been submitted this morning for review. I still have some tests to write and update translation files (need help on these topics) but I would like to get some feedbacks about changes introduced by this new feature
        * Notes: Provide test link 
    * Update from CKeditor5 workgroup (Victor)
        * Alex has pushed an example ckeditor5 demo plugin to the PR and the stage server :tada:  - https://django-cms-ckeditor5-stage.us.aldryn.io/en/ (login/password - test@django-cms.org/test@django-cms.org)
        * we discussed several ways of integrating the ckeditor5 plugins into the main djangocms-text-ckeditor package and documented it in the brief
        * we set up another call on Monday to specify djangocms-url-manager integration 
    * PR code review process (Iacopo)
        * is any workgroup responsible for this or do we need a dedicated workgroup?
        * How do we handle features proposed by the community?
        * Should they all be brought in the TC for discussion or only when deemed necessary during the code review? 
     * django CMS documentation (Daniele)
6. Review Tasks
7. News & updates for / from dCA Board and MarCom
8. Review approve and post the meeting notes

#### Tasks & Initiatives
- [x] Update Vinit about Github Actions and schedule kick off meeting for next steps together Jacob 


## 11.12.2020 

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest intro
3. Review agenda and add missing points
4. Varia: further points raised by Tech Committee members 
   - (Mario) Travis has paused its OSS program indefinitely. I suggest the new CI workgroup try Github Actions.
       - consenus to try Github Actions. Next steps: Update Vinit about Github Actions and schedule kick off meeting for next steps together Jacob 
   - (Mario)Release Management Update
       - Proposal was approved 
   - Adopting autoformatted code style (pre-commit + black) (for v4+ only)
       - Stay consistent, agreed as a group that a package should keep the package readable. Ideally we would use Flake8.  
   - (Victor) djangocms-text-ckeditor versioning + dropping the in-text plugins backward compatibility
       - Angelo is in favor of creating a new package
       - Andrew wouldn't like to tie it to a specific ckeditor version (eg 5), since that kills the default migration path
       - We might have a naming issue, since we can't just name it djangocms-text-ckeditor-new
       - We will review it and come back with several propositions in the future, there's no rush at the moment
   - (Iacopo)PR code review process:
           - is any workgroup responsible for this or do we need a dedicated workgroup?
           - How do we handle features proposed by the community?
           - Should they all be brought in the TC for discussion or only when deemed necessary during the code review? 
6. Review Tasks
7. News & updates for / from dCA Board and 
    - Releases about 3.x -> put on roadmap / announcem 
8. Review approve and post the meeting notes

#### Tasks & Initiatives


- [x] Unlock sponsorshop for TravisCI / Github Actions (Mario) 
- [x] get sponsorship for a VPS for the CI/CD pipeline on gitlab (Jacob Rief)
- [x] Proposal for move to Github Action (Vinit)


## 04.12.2020

#### Agenda Points

1. Add new entry for next meeting from template
2. Guest intro
    - Vinit Kunar
3. Review agenda and add missing points
4. Varia: further points raised by Tech Committee members
    - Workgroup updates (Nicolai)
    - dcmsv4 demo report (Andrew) - working demo: https://django-cms-40x-community-demo-stage.us.aldryn.io/ (ask andrew@django-cms.org or mario@what.digital to get access)
    - Update django-cms documenation (Iacopo)
    - Update workgroup "release" to find scope for 3.9
    - Update testing checklist (Nicolai) - https://www.notion.so/CMS-core-a90e440827294064a4dc380e3edd9dc5
    - [New directory of active contributors](https://docs.google.com/spreadsheets/d/1TRwb65boIPt80Q4JJ6isgz9x8aeoz6dah6jzm5ixamU/edit#gid=0)  
    - Bounty program was launched - Update?
    - Drop python 3.5 support (Jacob Rief)
6. Review Tasks
7. News & updates for / from dCA Board and MarCom
   - from the dCA Board: https://github.com/django-cms/django-cms-mgmt/blob/master/association/tasks-and-decisions-log.md  
   - from TC: announce Testing & QA Contribution Program for service providers (for Nicolai)
9. Review approve and post the meeting notes

#### Tasks & Initiatives
- [x] document list of core dependencies (LTS 3.7 scope) to be defined (it already exists, Angelo has it) for the setup of django CMS v3 demo project (Nicolai)
- [x] document testing checklist (let's make it available) - Nicolai
- [x] Nicolai to check with Angelo on 3.9 release scope
- [x] Nicolai to present the directory of active contributors
- [x] Workgroup updates - let's organize some for next TC meeting - Nicolai

## 27.11.2020

#### Agenda Points

1. Add new entry for next meeting from template
2. Guest intro
3. Varia: further points raised by Tech Committee members
   - think about QA / PM resourcing: We'll be making a lot of changes as the project gets busier. Need to make sure we're testing adequately to protect dependent packages / projects.
       - Describe the sanity check after major upgrade
       - there is a testing checklist (let's make it available) 
       - on top of that - describe user stories, testing procedures and tasks
       - the dcmsv4 workgroup is working on a demo project for v4 (Andrew)
       - we have a djangocms-template for v3 which we can use based on 3.7 LTS core packages
       - Set up a CI/CD Release Apps pipeline
           - also for dependencies (packages)?
       - Testing & QA Contribution Program for service providers
   - define next 3.9 scopes
       - Jacob: drop python 3.5 support (py3.5 is End Of Live)?
       - Nicolai to check with Angelo on further points
   - workgroup updates - let's organize some for next TC meeting (Nicolai?)?
5. Review Tasks
6. News & updates for / from dCA Board and MarCom
    - from Nicolai: Bounty Program Update
8. Review approve and post the meeting notes

#### Tasks
- [x] merge and release https://github.com/django-cms/djangocms-admin-style/pull/426
    - Released: https://github.com/django-cms/djangocms-admin-style/commit/ff21ae56bdcfbaa546b6c36e7e294edb56fc5d9a
- [x] think about QA / PM resourcing
   - CI - quickly spin up a testing instance. There is a django CMS demo org where we can set up projects in arbitrary configuration for testing / QA) - ask mario@django-cms.org
- [x] Nicolai will create a directory of DCA members and volunteers and sign people up.



## 20.11.2020 

#### Agenda Points

1. Add new entry for next meeting from template
1. Guest intro
    - welcome Mike (Compound Partners)
3. Varia: further points raised by Tech Committee members
    - Pages admin Workgroup update: Search results improvements in admin interface  (Mehdi)
    - Andrew: [djangocms-internalsearch rewrite](https://github.com/divio/djangocms-internalsearch) (haystack is only Elastic search <= 2.5 compatible)
    - Jean-Baptiste: allow deactivating unsorted uploads in django filer
    - Victor: a directory of DCA members and volunteers, eg on discourse.django-cms.org or a spreadsheet, which would help anyone to know a bit more about each other - decision: yes, we do this.
    - 3.8.0 readme is missing http://docs.django-cms.org/en/latest/upgrade/ (Nicolai), issue: https://github.com/django-cms/django-cms/issues/6948, assigned to Iacopo
6. news & updates for / from dCA Board and MarCom - none
7. Review approve and post the meeting notes - done

#### Tasks
- [ ] Updates on next steps regarding django CMS installer from Iacopo
- [ ] Nicolai to organize design / ux direction (initially for django-filer svg enhancement, but with a bigger perspective in the mid term)
       - django CMS v4 Community Release
       - headless django CMS (tentative / proposal)

#### Decisions


## 12.11.2020

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
1. Guest intro
3. Varia: further points raised by Tech Committee members
    - FYI - Workgroup update: django CMS v4 Roadmap has been created: https://hackmd.io/5Sj6X5XhTJOmZgNj8e_KCw
    - Victor: CKEditor5 workgroup
        - do we want to implement the url rest api within the core?
            - from Andrew: analyze further the importance of the existing in-text plugins, whether we can replace them with ckeditor5 es6 plugins
        - do we want to use the 3.X branch
            - we can spec it out and then decide, but probably yes since we don't want to wait for 4.0
            - Victor to create a follow up call with Alex and Andrew, points:
                - Victor to write a rough set of specs in a github ticket for the call that we can discuss together
    - "How to contribute to the documentation"-Training (Nicolai)
        - Everyone who is involved in django CMS development has to write documentation and should be trained in how to do it
        - Offer training for documentation tools and documentation writing 
        - Create documentation training workshop 
            - 1h sessions / once a week / 4 weeks
            - only dCA members 
            - record on video (?)
        - Schedule follow up meeting -> documentation workgroup 
    - Somebody contact wants to create their own versioning on top of django CMS. Can we use any synergies.
5. news & updates for dCA MarCom
    - djangocms Pypi is now up and running - key fact: as of now more people can release django cms packages on pypi and updates on github will be published on pypi much faster, this is great news for anyone using pypi (which is, everyone) - see https://pypi.org/user/djangocms/
    - if there are packages you would like to move under the umbrella of the pypi djangocms user or there are updates to packages already under control of djangocms on pypi pleaes get in touch with the Tech Committee <contact>credentials here</contact>
        - "keep it in good shape" - high visibly on Google 
7. review log entry together, approve and post

#### Tasks
- [x] Mario to create pypi@django-cms.org and django CMS pypi account, ask Angelo to add pypi packages to it, invite TC members to it.
- [x] Mario to ask travis-ci.org for open source sponsorship
- [x] Mario to work with Andrew on roadmap for django CMS v4 (10.11.2020)
- [x] Nicolai to complete workgroup roadmap process
- [x] Nicolai to build an overall django CMS ecosystem roadmap based on the workgroup roadmaps with the following big picture


## Thursday 05.11.2020 (WiP, upcoming Meeting)

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Guest intro
3. Varia: further points raised by Tech Committee members
    - 30 packages on pypi: TC members should be able to manage pypi. How? User permissions on pypi.
    - Discuss options/plans for adding/maintaining/improving documentation
    - Why are we using Travis: Andrew / Angelo: We currently use Travis because it allows to ignore specific tests for simplicity. 
    - Jacob Rief on django-filer: asking for testing feedback.
    - Jacob Rief to ask about UX / Design direction
5. news & updates for dCA MarCom
6. review log entry together, approve and post

#### Tasks
- [x] Discuss in the meeting the PyPi packages access to accounts, should probably be a DCA account. Angelo and Andrew to discuss.
- [x] Discuss future security defect patching and the process
- [x] Organise milestones on github from the Django cms issues (Andrew)
- [ ] Iacopo about get_translatable_content enquiry: https://github.com/django-cms/django-cms/commit/b1d1d50fac1532dfa650fe7ea2dfa8e85727fec0 - (add Andrew for django CMS 4 vision, also ask Paulo). - Iacopo to follow up on this outside the scope of the TC meeting
- [x] Andrew to add Iacopo to the discussions regarding cms v4 with Mario


#### Decisions
- 


## Friday 30.10.2020 (WiP, todays Meeting)

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
1. Guest intro
3. Varia: further points raised by Tech Committee members
    - Victor stated that Mario will be taking control of Victors responibilities in the workgroups due to work load. 
    - Andrew presented a list of milestones added to categorise issues remaining that can be allocated to the relevant workgroups
        - Requires workgroup allocation: https://github.com/django-cms/django-cms/milestone/65
        - Requires validation: https://github.com/django-cms/django-cms/milestone/66
        - Requires documentation improvements, could be seperated into relevant workgroups: https://github.com/django-cms/django-cms/milestone/67
    - Iacopo raised interest in undertanding the changes in V4 and what would be required in various packages for compatibility. 
5. news & updates for dCA MarCom
6. review log entry together, approve and post

#### Tasks
- [x] Nicolai to give Narender an intro into workgroups and how to contribute
- [x] take a decision regarding the fate of AAA and BBB (epic issues to be completed by Andrew) - do we want to have them on our roadmap? If yes, please name the workgroups.
 https://github.com/django-cms/django-cms/milestone/65
- [x] Nicolai to organize leaders for workgroups
- [x] Nicolai to get roadmaps for each workgroup from the workgroup leaders
- [ ] Nicolai to build an overall django CMS ecosystem roadmap based on the workgroup roadmaps with the following big picture
   - django CMS v4 Community Release
   - headless django CMS (tentative / proposal)
       - Next Steps
           - Carry over to next meeting due to not getting feedback required by the workgroup members.
- [ ] Nicolai to create a workgroup and add team members to it: Iacopo about get_translatable_content enquiry: https://github.com/django-cms/django-cms/commit/b1d1d50fac1532dfa650fe7ea2dfa8e85727fec0 - (add Andrew for django CMS 4 vision, also ask Paulo)
        - Next steps
            - Awaiting feedback from Paulo regarding why the feature was removed. Carried over to the next meeting. 

#### Decisions
- Various tasks carried over to the next meeting due to delays on dependant tasks.


## Friday 23.10.2020

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. add new entry for next meeting from template
1. Guest intro
    - Narender
1. Varia - further points raised by Tech Committee members
    - Go or No Go: Release 3.8.0 (Victor has it in production on several websites) 
    - Review of Assignment: Andrew and Nicolai to look at and clarify left-over PRs and propose workgroups from them
    - Review of Assignment: Mario presents proposal for mid-/long-term roadmap (features / improvements) for publication on the website (for marcom / Nicolai)
    - django CMS 4 workgroup setup & announcement 
    - Update Iacopo about get_translatable_content enquiry: https://github.com/django-cms/django-cms/commit/b1d1d50fac1532dfa650fe7ea2dfa8e85727fec0 - Nicolai to create a workgroup and add team members to it
1. news & updates for dCA MarCom (Board / Community)
   - django CMS 3.8
   - Workgroups
3. review log entry together, approve and post


#### Decisions
- decision to release 3.8.0 this Wednesday / Thursday, Angelo will do the release, Nicolai will do the blog post, Andrew will monitor SO / Discourse / Github Issues
- Decision to close one outdated epic (an issue that reference other issues) on django-cms github. Andrew will close it.


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
        - Next steps
            - Nicolai to check whether to add another scenario to the template that fits to the example case (ask Andrew)
    - Review of Assignment: Victor reports on 3.8 CMS testing, Victor to onboard Lisa for testing
        - djangocms 3.8 & django 3.0 has been deployed to 3 projects on the last week
            - the codebase utilized
                - https://gitlab.com/effective-altruism/ea-cms-template
                - https://gitlab.com/what-digital/djangocms-template
        - Next steps
            - Nicolai to help onboard Lisa in order to upgrade django-cms demo to 3.8
    - Review of Assignment: Victor / Andrew report on djangocms-url-manager / djangocms-link rewrite plans (3.7 compatibility is confirmed) -> Nicolai to create workgroup(s) with Andrew / Victor on it.
        - Next steps
            - Andrew: to attach a link to a working cms 4 server
            - Victor: to share a url to a public server with djangocms-link-all
                - we created a new channel on slack `workgroup-new-link-plugin` - the details are there
    - Review of Assignment: Andrew to do an intro with his contact for a django CMS 4 demo. Mario reports on django CMS v4 demo schedule
        - Next steps
            - Demo scheduled to be presented to Victor 
    - django CMS 3.8.0 release schedule
        - Next steps
            - TC to give Go for Gold Release next TC meeting. Release scheduled for Wednesday after TC meeting
    - New feature request: Iacopo updates regarding a feature request (export / import of page trees) from a client
        - Next steps
            - Victor: to invite Vlad to dca slack channel, create a workgroup channel for it, ask him to find the existing codebase
            - Iacopo to update TC on feature request after more exploration/analysis
    - Support enquiry regarding get_translatable_content removed in https://github.com/django-cms/django-cms/commit/b1d1d50fac1532dfa650fe7ea2dfa8e85727fec0
        - Next steps
            - Iacopo will get in contact with the person who closed the PR and report back next TC meeting. 
    - Feedback on guest post topics https://docs.google.com/spreadsheets/d/1jNCtIUDmsj-qZZPe7yq73umR7FGra_3H39hqTjgvyAQ/edit#gid=1394201430
        - No feedback 
4. news & updates for dCA MarCom
        - Workgroup announcement next week 
6. review log entry together, approve and post


## Friday 09.10.2020 
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

