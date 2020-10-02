# Tech Committee - Tasks and Decisions Log

<small>The Tech Committee meetings documentation must follow the format of the [Tech Committee Log Entry Template](/tech-committee/tasks-and-decisions-log-entry-template.md)</small>

[ℹ️ See here for all Tech Committee tasks](https://github.com/django-cms/django-cms-mgmt/projects/1)

[ℹ️ See here for the live version](https://hackmd.io/ddhvq_aqS6my9gwhLddyPg)

## Friday 09.10.2020 (WiP, upcoming Meeting)
#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>
1. add new entry for next meeting from template
1. Guest intro
1. Varia: further points raised by Tech Committee members
   - Mario presents mid-/long-term roadmap (features / improvements) for publication on the website (for marcom / Nicolai)
   - Victor reports on 3.8 CMS testing
   - Victor / Andrew report on djangocms-url-manager / djangocms-link rewrite plans
   - Mario reports on django CMS v4 demo schedule
1. news & updates for MarCom
1. review log entry together, approve and post

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







