# dCA Tech Committee - Tasks and Decisions Log

###### tags: `meeting protocol`

<small>The Tech Committee meetings documentation must follow the format of the [Tech Committee Log Entry Template](/tech-committee/tasks-and-decisions-log-entry-template.md)</small>

- [Tech Committee task board](https://github.com/django-cms/django-cms-mgmt/projects/1)
- [this doc's hackmd url](https://hackmd.io/ddhvq_aqS6my9gwhLddyPg)
- [this doc's github repo url](https://github.com/django-cms/django-cms-mgmt/blob/master/tech-committee/tasks-and-decisions-log.md)
- [Process: Proposing large feature additions](https://github.com/django-cms/django-cms-mgmt/blob/master/contribution%20policy/contribution%20policy.md)

<strong>Policy: If there are no items on the agenda 30 minutes before the meeting, the meeting will be cancelled.</strong>

## dd.mm.2022

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - (Name) 
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
5. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
7. News & updates for / from dCA Board and MarCom
8. Review approve and post the meeting notes


## 25.02.2022 (NEXT)

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - (Name) 
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
5. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
7. News & updates for / from dCA Board and MarCom
8. Review approve and post the meeting notes

## 11.02.2022 (CURRENT)

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - Fabian 
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
   - Mario: ok to add the policy about version numbers to the official documentation: https://github.com/django-cms/django-cms/discussions/7149
   - Angelo: Seriously, Marketplace needs a redirect ;)
       - handled by Mario
   - Angelo: Django 3.2 support on Alias, URL Manager, Versioning
       - djangocms-alias - https://github.com/django-cms/djangocms-alias/pull/78
       -- djangocms-url-manager - https://github.com/django-cms/djangocms-url-manager/pull/66
       - djangocms-versioning - No PR here yet that I can see.
   - Fabian: Darkmode?
       - Andrew (djangocms-admin-style package)
       - new workgroup-darkmode (feel free to join on Slack)
6. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
7. News & updates for / from dCA Board and MarCom
    - From the dCA board: nominations for leadership positions
    - To MarCom: Pending RC 3.10
9. Review approve and post the meeting notes

## 28.01.2022

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - (Name) 
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
    - Mark: Automate cleanup of stale issues/PRs
        - https://github.com/actions/stale
        - How long before an issue/PR is considered stale?
        - Next Step: Mark to have a look at the bot settings and to come up with a proposal for how to configure the bot
    - Mark: New gulp pipeline & dependabot security updates to keep things up-to-date.
    - Mark: Python support for upcoming features.
        - Python 3.6 is [EOL](https://endoflife.date/python), 3.7 has 18mths left
        - Django 4 supports python >=3.8
        - Perhaps django-cms 3 & 4 get a minor release to bring in [python 3.10 support](https://github.com/django-cms/django-cms/pull/7126), then [django 4](https://github.com/django-cms/django-cms/pull/7184), while other packages in the dCA perhaps stay closer to semver and the django 4 support comes with a major version bump.
    - Jacob Rief: Replace model `menus.models.CacheKey` by wildcard deletion. In Redis this is a feature and for memcached there is a workaround.
    - Jacob Rief:
        - New permission to set page as HOME must be added.
        - Selecting a User and/or Group shall be handled by auto_complete fields.
        - Strange assumptions in some unit tests.
    - Angelo Dini:
        - Reminder to deprecate the django-cms marketplace end of January (https://marketplace.django-cms.org/)
        - Who will change the domain? Nicolai to ask Mario about next steps
5. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
7. News & updates for / from dCA Board and MarCom
    - new dCA member: [alwaysdata (hosting solution) ](https://www.alwaysdata.com/fr/marketplace/django-cms/)
9. Review approve and post the meeting notes

## 14.01.2022

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
   - Mario: version policy (dcms 3 / 4 compat policy for packages) - it's agreed upon but is there documentation (maybe a blog article?)
       - Mario to do a RFC
   - Andrew: Dark mode breakage dj3.2+ https://github.com/django-cms/djangocms-admin-style/issues/439
       - Andrew to assess what needs to be done to fix
6. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
7. News & updates for / from dCA Board and MarCom
    - Mario: Demo workgroup: the 60min demo project can now be recreated locally via new https://github.com/django-cms/django-cms-60min-demo-2021/
        - Simon to test the project and create issues in the repo. 
    - Announcement for new Platinum Member LWL (15k EUR p.a)
8. Review approve and post the meeting notes


## 17.12.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - (Name) 
4. Review agenda and add missing points 
6. Varia: further points raised by Tech Committee members:
    - (Andrew) Django 2.2 support in packages, change and release plan for django 4.x?
        - drop support for django==2.2 for the next django-cms 4 (4.2) and django-cms 3 (3.11) release, support 3.2 (LTS) on dcms 3, 4, recommend 3.2 (LTS) for all packages
        - use major version numbers for breaking changes on all packages in the ecosystem (i.e. version your package from x -> x+1 if changes contain dependency upgrades such as django 2.x -> 3.x or dcms 3.x -> 4.x)
        - Reminder: django CMS LTS Release 3.11 for end of Q1 2022 (must support django 3.2) until 2024
    - (Florian) Update 3.10 release 
    - (Jacob) Enhancement proposals:
        - https://github.com/django-cms/django-cms/discussions/7174
    - (Nicolai) [New project guide released](https://docs.django-cms.org/en/latest/contributing/guideline-for-django-cms-projects.html)
9. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
10. News & updates for / from dCA Board and MarCom
    - Announcement released: New [volunteer positions](https://www.django-cms.org/en/blog/2021/12/07/new-dca-volunteer-positions-available-in-2022/) available 
    - [django CMS Fellowship program](https://www.django-cms.org/en/fellowship-program/)
    - Announcement released: [django CMS Marketplace deprecated](https://www.django-cms.org/en/blog/2021/12/15/end-of-life-for-marketplace/)
11. Review approve and post the meeting notes

## 03.12.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - (Name) 
4. Review agenda and add missing points 
6. Varia: further points raised by Tech Committee members:
    - (Andrew) Divio Addon releases as part of the DCA release process?
        - The release process should be updated to include notifying Angelo / someone at Divio that a release to a package has been made and a Divio Cloud / Marketplace addon may need to be released.
    - (Jens-Erik) Legacy plugins: [cmsplugin-filer](https://github.com/divio/cmsplugin-filer) should link to David Bertrand’s [migration app](https://www.imagescape.com/blog/migrate-away-cmsplugin-filer-few-easy-steps/), based on an undocumented [Github gist](https://gist.github.com/wfehr/86ac31e8e263b872b746cc721662251e). I have made a [fork](https://github.com/MacLake/deprecate_cmsplugin_filer) and PR with some improvements.
        - cmsplugin-filer was transfered to dCA github org. Readme file will be changed by Nicolai accordingly. The migration app will be included in the next community news. 
    - (Jacob) Django filer PR https://github.com/django-cms/django-filer/pull/1264
        - We keep support for Python-3.6 and add a conditional to fix tests.
8. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
9. News & updates for / from dCA Board and MarCom
- dCA board is preparing the strategy for the dCA for 2022
11. Review approve and post the meeting notes

## 19.11.2021 

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - (Name) 
4. Review agenda and add missing points 
6. Varia: further points raised by Tech Committee members:
    - (Simon & Jens Erik) Related to [this GitHub issue](https://github.com/django-cms/django-cms/issues/7151) - We should maybe think about changing the default settings for djangocms-ckeditor so that empty `<i class="…"></i>` no longer disappear when used in the source view. Because it could lead to confusion.
        - The TC endorses this idea
    - (Angelo) deprecating https://marketplace.django-cms.org/en/ 
        - Next: Redirect URL, Nicolai to create blog post about deprecation 
        - The TC approves this motion
    - (Jens-Erik) After Nicolai’s survey: What about promoting the forum for support?
        - Feature forum on website more prominently as primary support channel 
        - Investigate: Install Greet Bot that welcomes every member and presents all support options (push towards forum)
    - (Andrew) Move djangocms core components to DCA
        - Angelo going to ask internally if it is ok to move core repos to dCA org and follow through accordingly
        - djangocms-versioning
        - djangocms-alias
        - djangocms-url-manager 
    - (Andrew) djangocms-snippet v4 release version number agreement, https://github.com/django-cms/django-cms/discussions/7149
        - Andrew to come up with a proposal which will be posted in discussion 
    - (Mark) I've made a start on automating releases; https://github.com/django-cms/django-classy-tags/pull/64 
        - You're da  man! Really cool effort Mark!
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
    - New tutorial video: [django CMS Quickstart](https://youtu.be/XJsP85ksvOo) by Simon 
10. Review approve and post the meeting notes


## 05.11.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - (Vadim) 
4. Review agenda and add missing points 
6. Varia: further points raised by Tech Committee members:
    - (Vinit) RFC: ready for voting? https://github.com/django-cms/django-cms/discussions/7125
        - TC encourages someone to try this on a new project where it doesn't create impact on the community and report back on the outcome
        - Mark: Would be worth mentioning my pre-commit PR. If people are happy with what I've included, we can spread this to the other repos; https://github.com/django-cms/djangocms-bootstrap4/pull/142
            - TC approves this as the preferred strategy regarding automated code formatting
    - (Andrew) new RFC "Package version number release scheme for django-cms 4.x packages"- please review: https://github.com/django-cms/django-cms/discussions/7149
        - TC follows Mark's suggestion to coordinate a sunset roadmap for django CMS 3 support from where on only minor version numbers would be used for django CMS v3 compatible versions and the next major version introduces django CMS 4 compatibility, from there on it can continue with major version number increments.
    - (Jens-Erik) Timezone and summer time issue - are we sticking to the current meeting time?
        - We keep it like this.
    - (Jacob) django-filer 2.1 (with SVG support) has been released. There have been some reports from one user wanting "reportlab" being optional. This library however is required  for SVG. And I don't want to make this just optional. SVG shall be a fundamentally supported image type.
        - TC follows Jacob's proposal to keep the reportlab package.
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
10. Review approve and post the meeting notes

## 22.10.2021 

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members:
    - (release management workgroup)
        - Situation: Since django-cms already supports 3.2 since the last release, we should release 3.2 support for the plugins asap. 
        - Proposal: Implement Auto release to pypi via github to projects (except django-cms). So that we can action something in github, and it'll be built & released to pypi. We'd likely not do this with django-cms itself. But it'd make all the other packages much easier to run. It's likely the action that would trigger a build & release would be tagging [a new version] after merging PRs. So the code gets reviewed, merged and then if the changes are significant enough to release, someone creates a release or a tag and then that triggers the build/release action.
        - Docs on releases; https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository
        - Benefits: We will reduce the load on the release manager and at the same time, remove the friction of releasing. However, we need to be really strict with the merging part. 
        - Questions: 
            - What does it take apply this method to django-cms?
            - What happens with projects that use readthedocs?
            - We probably need different tiers for different packages -> there's important package where the risk of messing up is too high 
    - (Jens-Erik) django-cms-column -> who has access?
        - move it to dCA umbrella and mark it as deprecated 
        - Documentation: 
            - Check deprecation process in the documentation 
            - How to remove djangocms-cms-colum -> multi-step process 
        - Blog post by Nicolai -> deprecated
    - (Nicolai) Please review: Guideline for projects under dCA umbrella: https://docs.google.com/document/d/17bPrkOSN6G73HoFzJW3FDbqKoQkqhCTBq6N6kVt2-yE/edit#heading=h.oylrpll48c27
    - (Nicolai) Jacob pls have a look at #workgroup-security thx 
    - (Florian) django CMS 3.10 RC1 release is currently blocked - I need help!
    - (Mario & Nicolai) Proposal: Change weekly meeting to bi-weekly - objections
        - Proposal to change time 3pm CEST  
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
10. Review approve and post the meeting notes




## 08.10.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members:
- (Andrew A) django-cms 4.0.x release number for django 3.x breaking changes
- [New discussion](https://github.com/django-cms/django-cms/discussions/7125#discussioncomment-1440169) about code formatter - please review and leave your feedback
- (Nicolai) django-cms 3.10 is just around the corner
    - Florian will create new release but cannot review and merge pending PRs
    - Time window is closing - review and merge now!
- (Mario) FYI - New aldryn-free-and-otherwise-simplified version of django CMS Template was published at https://github.com/django-cms/djangocms-template (thanks Victor, Sergey G. Andrew for reviewing)
- New workgroup: Security 
    - security@django-cms.org
    - #workgroup-security
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
- [User Guide 1.0 released](https://docs.google.com/document/d/1f5eWyD_sxUSok436fSqDI0NHcpQ88CXQoDoQm9ZXb0s/edit) 
- News extended support for 3.7 - what needs to be communicated?
10. Review approve and post the meeting notes

## 01.10.2021 

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - Update: [LTS for 3.7 ended in September 2021](https://www.django-cms.org/en/roadmap/)
        - As agreed before, proposal to sync django CMS LTS with django LTS
        - Next Django LTS Release is 3.2 end of Q1 2022 (until 2024)
        - Proposal to set django CMS LTS Release 3.11 for end of Q1 2022 (must support django 3.2) until 2024
        - Proposal to extend support for django CMS 3.7 LTS until end of Q1 2022
        - django CMS 3.10 will be released as planned in Q4 2021
    - Workgroup updates:
        - Simon is making progress with quickstart template
            - Suggestion: Two types of Quickstart 
                    - empty one / barebone 
                    - static template with getting started information
                - 2. demo type 
        - New documentation added 
            - How-To Multisite 
            - Installation Guide revised -> added docker
    - Suggestion: Launch security workgroup (Tech Brief)
        - Important: 
            - Private Workgroup 
            - Review security issue / Someone has to look at the email 
            - Communicate as soon as possible / Reply asap
            - Bounty Program? 
                - depending on the severity we will talk to you
            - Mario to give Nicolai access to security@django-cms.org and send email answer template 
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
    * [New case study released](https://www.django-cms.org/en/blog/2021/09/29/migrating-from-wordpress-to-django-cms/)
    * [Hacktoberfest has started](https://www.django-cms.org/en/blog/2021/10/01/we-celebrate-hacktoberfest-2021/)
    * [Guest blog published](https://www.django-cms.org/en/blog/2021/09/23/what-can-you-build-with-python/) 
    * Blog post -> Check link from Angelo 
10. Review approve and post the meeting notes


## 17.09.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - Mark - @all: Please review:
        - https://github.com/django-cms/django-cms/pull/7101 (help menu)
        - https://github.com/django-cms/django-cms/pull/7104 (flake8 fix)
    - Nicolai: Hello Bootstrap 5 - next steps? 
        - https://github.com/gl-agnx/djangocms-bootstrap5 
            - Nicolai to get in touch with author and ask if the dCA can take the plugin/package under its umbrella
            - Bootstrap4 plugin to be marked as deprecated
    - Mario: https://github.com/django-cms/django-cms-quickstart/tree/develop 
        - new branch "develop", where we can integrate experimental stuff
        - I updated to the latest Release Candidate of the new filer with native SVG support!
        - Also updated to bs5 (see above)
    - Mike: Ownership of Divio Cloud Addons
        - ALDRYN DJANGO CMS @ 4.0.0.15
        - DJANGO CMS ALIAS @ 0.0.12
        - DJANGO CMS MODERATION @ 1.0.27
        - DJANGO CMS TEXT CKEDITOR @ 4.0.0.DEV5
        - DJANGO CMS URL MANAGER @ 0.0.11
        - DJANGO CMS VERSIONING @ 0.0.29
        - DJANGO CMS VERSIONING FILER @ 0.0.14 (only required to version files)
            - Mario to work on making version 4.0 aldryn independent (-> pypi) 
    - Jacob: Proposal for simplifying django-filer using a JSONField to store meta-data: https://github.com/django-cms/django-filer/discussions/1256 
        - No objection from the team - Jacob can go forward with it  
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
    - Mario recorded a video tutorial "deploy djangocms template to divio": https://youtu.be/O2g5Wfoyp7Q 
10. Review approve and post the meeting notes


## 10.09.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
   - Jacob: Upgrade djangocms-quickstart and djangocms-template to [django-filer 2.1rc4](https://github.com/django-cms/django-filer/tree/2.1rc4) - Approved
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
9. Review approve and post the meeting notes

## 03.09.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
6. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
7. News & updates for / from dCA Board and MarCom
8. Review approve and post the meeting notes


## 27.08.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
   - Mario: Updated demo instructions on django-cms.org to use django-cms-quickstart project, updated django-cms-quickstart project with better docs (see [here](https://github.com/django-cms/django-cms-quickstart))
   - Mario: Updated djangocms-template project (pending PR) to work exclusively with pypi packages (removed all aldryn packages in favour of django-whitenoise), added divio deploy instructions. Please comment on the pending PR [here](https://github.com/django-cms/djangocms-template/pull/5)
   - Mario: Proposal to accept and add [Plugin Dependency Policies for django CMS Developers](https://github.com/django-cms/django-cms/discussions/7096) to the docs
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
10. Review approve and post the meeting notes

## 20.08.2021 CANCELLED

## 13.08.2021 CANCELLED

## 06.08.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - Update: Please review the following 2 PRs:
        - [Stop ignoring flake8 errors](https://github.com/django-cms/django-cms/pull/7104) 
        - [Help menu](https://github.com/django-cms/django-cms/pull/7101)
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
    - 2 new bronze members -> sunscrapers (Poland) and swansoft (India)
    - 3 interesting plugins 
        - [djangocms-algolia](https://pypi.org/project/djangocms-algolia/)
        - [django-frontify](https://github.com/lab360-ch/django-frontify)
        - [django check SEO](https://dev.to/corentinbettiol/django-check-seo-3ljk)
10. Review approve and post the meeting notes

## 30.07.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - No items added
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
10. Review approve and post the meeting notes

## 23.07.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - Please review & feedback
        - Proposal 1: [Add Help Button to toolbar by default](https://github.com/django-cms/django-cms/discussions/7094) 
        - Proposal 2: [Plugin Dependency Policies for django CMS Developers](https://github.com/django-cms/django-cms/discussions/7096)
        - Proposal 3: [Website Wireframes](https://miro.com/app/board/o9J_lATSwJ8=/) 
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
    - New plugin for django CMS - [djangocms-algolia](https://www.django-cms.org/en/blog/2021/07/21/improve-your-search-with-djangocms-algolia/)  
10. Review approve and post the meeting notes

## 16.07.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - Mario: Review [plugin strategy RFC](https://hackmd.io/j8srdcV6SMaZExecPG72Yw?view)
    - Nicolai: Please review [Feature proposal](https://github.com/django-cms/django-cms/discussions/7094)
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
    - Q2 dCA recap -> pls check your inbox  
10. Review approve and post the meeting notes



## 09.07.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - [Review Plugin list ](https://docs.google.com/spreadsheets/u/1/d/1kANl66x5CLoL3ZcL613Qz1sClfnDvh9jk8csrh9cSQM/edit#gid=397686173) 
    - New workgroup: Github Issue Management 
    - django CMS 4.0 [onboarding document](https://hackmd.io/5Sj6X5XhTJOmZgNj8e_KCw?view) updated 
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
10. Review approve and post the meeting notes



## 02.07.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - [Nicolai] [Article: How to encourage devs to contribute?](https://cacm.acm.org/magazines/2021/7/253459-why-computing-students-should-contribute-to-open-source-software-projects/fulltext) -> *Look for project issues marked as “Good first issue,” which indicate a project that is open to new contributors.*
        - Question: Who can help with that? Going through all issues (approx. 200) and assign the label "Good first issue"
        - Maybe start with 10 per week? At least to get a start on it...
        - Next step: Nominate a list of issues that are apt for beginners
        - Prioritize issues from other repos 
    - [Nicolai] Reminder: Please review Plugin list https://docs.google.com/spreadsheets/d/1kANl66x5CLoL3ZcL613Qz1sClfnDvh9jk8csrh9cSQM/edit#gid=397686173 and leave feedback. 
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
    * Published: django CMS 3.9.0 release announcement 
        * [Florian] next version will be 3.9.1 to fix a few bugs 
10. Review approve and post the meeting notes


## 25.06.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - (Nicolai) Update 4.0 work group: [Onboarding Document](https://hackmd.io/5Sj6X5XhTJOmZgNj8e_KCw)  
    - (Nicolai) New theme for [documentation](https://docs.django-cms.org/en/latest/)
        - New structure, extended contributor guidelines and some small changes will follow soon
        - Feedback in #workgroup-documentation
    - (Nicolai) django CMS 3.9 RC3 was released
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
    - Website Relaunch: Review of [wireframes](https://miro.com/app/board/o9J_lATSwJ8=/) with Luke 
    - Use website as an example project for migration to 4.0 
    - Nicolai to get in touch with Pavel regarding CKeditor contribution 
10. Review approve and post the meeting notes


## 18.06.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - [Gabriel Andrade](https://www.linkedin.com/in/gabrielcandradecg/)
    - [Marcelo Cordeiro Correia]([[https://](https://www.linkedin.com/in/marcelocordeirocorreia/))
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    * [Jacob] Proposal: In django-filer replace `AdminFolderFormField` and instead use autocomplete_fields as introduced in Django-2.2. Pull request: https://github.com/django-cms/django-filer/pull/1246
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
10. Review approve and post the meeting notes

## 11.06.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - Kaushal & Mohammed 
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - [Florian] I suggest to release 3.9.0 next week and start working toward 3.9.1 to address minor fixes.
        - any objections?
            - Yes. please check back with Florian: RC3 probably required because of pending issues according to Angelo
7. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
    - New blog article by Martin Cote ([django CMS vs. Wordpress](https://www.django-cms.org/en/blog/2021/06/10/django-cms-vs-wordpress/))
    - [Mario] Can / Should MarCom request for comments for Jacob's RFC? (task for Nicolai)
10. Review approve and post the meeting notes


## 04.06.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - Abdelrhman  ([LinkedIn](https://www.linkedin.com/in/bershawi/))
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - [Florian] Need full access to PyPi and made admin in Github organization. Any objections? 
        - Notes:
            - No objections from the TC 
            - Access was granted by Angelo
    - [Jacob] [Proposal: Add JSONFields to various django-CMS models](https://github.com/django-cms/django-cms/discussions/7074)
        - Notes:
            - Suggestion for next step: Make Proposal public (in [Discourse Forum](https://discourse.django-cms.org/c/feature-requests/6)) and ask for community feedback 
            - Advertise for the RFC
    - NPM and Python Versions are outdated on the django-cms.org GitHub Repository https://github.com/django-cms/django-cms.org
        - Nicolai is planning a django CMS relaunch 
        - Update: [See announcement](https://www.django-cms.org/en/blog/2021/06/03/call-to-arm-website-relaunch/)
        - Core team so far: Victor and Nicolai 
        - Will need help at Design & Implementation stage
6. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
7. News & updates for / from dCA Board and MarCom
    - New [Case Study](https://www.django-cms.org/en/case-studies/expertsnow/) published 
    - To be released soon: New WordPress vs. django CMS article by Martin (D-Modules) 
9. Review approve and post the meeting notes

## 28.05.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
3. Review agenda and add missing points
4. Varia: further points raised by Tech Committee members
    - [Marcel] Versions for new Projects, 3.x or 4.0 - LTS? 
        - There will be a 3.9 or 3.10 LTS version
6. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
7. News & updates for / from dCA Board and MarCom
    - (Nicolai is on vacation)
9. Review approve and post the meeting notes



#### Tasks & Initiatives

Please go to: https://github.com/django-cms/django-cms-mgmt/projects/1

## 21.05.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - Dimitri from https://yare.fr/  
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - [Jens-Erik] How to deal with legacy plug-ins in existing installations? Documentation needed.
       - Everyone is invited to create help documentation - please get in touch with Jens Erik to see where help is most needed
       - Suggestion: Add a link to the new repository in deprecated plugins 
       - New Task: Create a list of deprecrated plugins where a migration instruction is needed (Nicolai to create a task) 
    - [Florian] Changes to the PR process (already sent) 
        - No need to update [CHANGELOG.rst](https://github.com/django-cms/django-cms/blob/3.9.0rc2/CHANGELOG.rst) anymore
        - information for CHANGELOG.rst release will be directly pulled by the releases script
        - Now using conventionalcommits.org guidelines
        - scopes already implemented here (please comment): https://github.com/django-cms/django-cms/blob/develop/scripts/make-changelog#L10-L16
        - New Task: Add documentation to the developer documentation (i.e PR titles must start with one of the categories)
        - Suggestion: this has maybe the potential for a blog post?
    - [Florian] Path from 3.9.0rc2 to 3.9.0rc3? (or golden):
        - How long should the RC2 validation time be?
        - What are the requirements to declare a new RC (RC3)?
        - Can we start moving issues into the 3.9.0 milestone to define completion for 3.9.0?
        - What is the test requirement to promote 3.9.0rcx to 3.9.0?
        - Are the current tests sufficient on the code base, if not can we define what is missing?
        - Suggestions: Let's branch this out and have a separate call with Angelo 
    - [Florian] Issue / PR house keeping:
        - There is (at the time of writing) more than 200 open issues, some of which are more than 3 years old
        - What can be done to lower this number?
        - What actions should we take regarding PR that are too old to merge? (how do we determine which one are?)
        - Next task: Let's branch this out and have a separate call with Nicolai 
        - [Issue / PR Templates](https://hackmd.io/@fverde/H1WTZoaIu) 
        - Suggestion: Let's find and propose an automated solution (bot) that can comment and give notice before closing old / stale stuff.
    - [Florian] Plans for 3.9.x/4.x:
        - Can we make 3.9.x the LTS version till 4.0 is ready (only new bugfixes gets in 3.9.x)?
            - [Angelo] let's align with the LTS policy of django (it appears we can't drop django 2.2 yet, therefore)
            - [Angelo] the next LTS version should be 3.10 and it should just include dropped features and dropped compatibility (deprecate old python and django versions)
            - Suggestion: End of 2021 - 3.10 same setup as django (but without django 2.2) & support until 2014
        - New features would go in 4.x
    - [Florian] Plans for `release/4.0.x` / `develop-4.x`
        - Currently a customer is using release/4.0.x as base to evaluate 4.0.x, (but it isn't released yet)
        - Do we know how this customer is currently pulling/updating their codebase?
        - 4.x would need its own develop branch:
            1. `release/4.0.x` becomes the new develop-4.x branch `git branch mv release/4.0.x develop-4`
            2. we then branch again from here: `git checkout develop-4; git checkout -b release/4.0.x`
            3. => this allows continuity from `develop` (the origin of `release/4.0.x` to `develop-4.x`)
            4. at some point, `develop` dies, and will be replaced by `develop-4.x` for default branch
        - We can then start cherrypicking features/upgrades from 3.x to 4.x into `develop-4`
        - 4.0.0rc1 should be released off that new branch later (not disturbing the customer evaluation)
        - New Task: a `develop-4` branch will be created by Florian 
    - [Florian] What are the requirements (goals) to meet to create 4.0.0rc1?
        - how do define the proper test environment?
            - we have https://github.com/django-cms/django-cms-quickstart/tree/support/cms-4.0.x
        - What roadmap should be defined?
            - Roadmap https://hackmd.io/5Sj6X5XhTJOmZgNj8e_KCw
        - Can we derive a plan of action?
            - Next step is: testing and creating tickets here: https://github.com/django-cms/django-cms/projects/2
    - [Florian] Creation of the pluginability workgroup: https://hackmd.io/0qQ2ZCsFS_2DzPzp7ZDV_Q?both
        - Quick alignment on goals
        - Definition of PR scope and approval
        - [Mario] would suggest to quickly sync with Andrew who has already spent some time thinking about a "hook"-based architecture to plug in different functionality in a decentralized way (i.e. plugin to plugin)
        - Task: Let's setup a RFC process (Nicolai & Vinit) ->django enhancement proposal
6. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
8. News & updates for / from dCA Board and MarCom
    - [3.9.0 RC1](https://www.django-cms.org/en/blog/2021/05/19/django-cms-3-9-0-rc1-released/) is now available 
    - [3.9.0 RC2] has followed (today) as a result of a critical bug found, and fixed
9. Review approve and post the meeting notes

#### Tasks & Initiatives

Please go to: https://github.com/django-cms/django-cms-mgmt/projects/1


## 14.05.2021 (Cancelled)

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
6. Review Tasks
7. News & updates for / from dCA Board and MarCom
9. Review approve and post the meeting notes

#### Tasks & Initiatives

Please go to: https://github.com/django-cms/django-cms-mgmt/projects/1


## 30.04.2021 (Today)

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
6. Review Tasks
7. News & updates for / from dCA Board and MarCom
    - General Assembly of the dCA, Friday 7th of May, 2pm CEST 
    - Tech Talk: djangocms-cascade intro, Tuesday 11th of May, 5pm CEST [Link to event](https://www.django-cms.org/en/events/techtalk-djangocms-cascade-introduction/)
9. Review approve and post the meeting notes

#### Tasks & Initiatives

Please go to: https://github.com/django-cms/django-cms-mgmt/projects/1



## 23.04.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - [Florian] (https://www.linkedin.com/in/floriandelizy/) (optional)
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - **django-filer** has a permission system. If enabled, one can choose a folder and change the permissions. That editor seems to by broken, both from its layout and its functionality. I need some clarification on how to proceed. (Jacob)
        - Please raise a ticket in the respective django filer repository @jacob
     - Update: Github Action Migration
         - All repos ported except
             - [djangocms-moderation](https://github.com/django-cms/djangocms-moderation)
        - Kudos to the team Vinit, Simon, Mark, Narender, Andrew
    - **Help needed**: New django CMS Release (Q1 Release)
        - Video tutorial (53mins): [django CMS release process](https://drive.google.com/file/d/1KiJBrKVvBvJMGVCYHqyz9cRbO8qTqpR5/view?usp=sharing)
        - [#workgroup-release-management](https://django-cmsworkspace.slack.com/archives/C01H0QA97HN)
        - One volunteer (release owner) to help with release
    - Ask Angelo what needs to be done for the release 
7. Review Tasks
8. News & updates for / from dCA Board and MarCom
    - Update: Tech Talk presented by dCA 
        - [djangocms-cascade](https://www.django-cms.org/en/events/techtalk-djangocms-cascade-introduction/) the swiss army knife of django CMS
        - Speaker: Jacob Rief
        - Date: 11th of May 2021, start 17:00 - end 18:30 (CEST) 
10. Review approve and post the meeting notes

#### Tasks & Initiatives

Please go to: https://github.com/django-cms/django-cms-mgmt/projects/1

## 16.04.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - [Robert](https://www.linkedin.com/in/robertu/) 
    - [Nishant](https://www.linkedin.com/in/nishant-nawarkhede-9b213923/)
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - Mario Colombo via Mark Walker: Proposes policy to dropping EOL python versions from tests - very specifically 2.7. and 3.5 (Mario)
        - No objections from the TC
    - sample/template website, for reuse by anyone who wants a quick start. I'd like to make it and support it. Question: 4.0.x as the base or too early? (Andrzej)
    - Update: Issue & PR Review group 
        - Who can help? Add labels to [issues / PRs](https://github.com/django-cms/django-cms/issues): Please add the following labels if applicable:
            - Needs contribution
            - Needs more info
            - Priority: low, mid, high
6. Review Tasks
7. News & updates for / from dCA Board and MarCom
    - General Assembly at Friday 7th of March 2pm - postpone TC? (Nicolai)
9. Review approve and post the meeting notes

#### Tasks & Initiatives

Please go to: https://github.com/django-cms/django-cms-mgmt/projects/1



## 09.04.2021 (Today)

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - ([Florian](https://www.linkedin.com/in/floriandelizy/))
    - ([Robert](https://www.linkedin.com/in/robertu/))
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - Update: Todos and Ticket management in Github now  https://github.com/django-cms/django-cms-mgmt/projects/1 (Nicolai)
    - Update: Github Action Migration / django cms unblocked (Nicolai)
        - Migration to main repo is finished 
        - Almost all important repos are ported 
        - Next steps:
            - 3.7 & 3.8 need to be backported 
    - Update: Github Issue / PR Review Group (Nicolai)
        - who are senior reviewers and who can merge pull requests
    - [v4 release plan discussion](https://github.com/django-cms/django-cms/projects/2) (Andrew)
        - Is it sane to release an alpha version to 4? 
        - Who is interested in helping Andrew creating an end-to-end release plan?
6. Review Tasks
7. News & updates for / from dCA Board and MarCom
    - Anything to broadcast to the community?
        - (Github Action Migration)
9. Review approve and post the meeting notes

#### Tasks & Initiatives

Please go to: https://github.com/django-cms/django-cms-mgmt/projects/1

## 02.04.2021 (No meeting due to holiday)

## 26.03.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
3. Review agenda and add missing points
4. Varia: further points raised by Tech Committee members 
   - django CMS v4 Workgroup update: You can now post a note with your django CMS v4 feedback here: https://github.com/django-cms/django-cms/projects/2 
   - django CMS CI update: There is an initial proof-of-concept on the Github Actions. Read more and/or join us in our efforts here: https://django-cmsworkspace.slack.com/archives/C01G6A0T16H/p1616750583004300 (Mario)
       - Andrzej to assign someone to help with CI migration and v4 quickstart. Introduce that person to slack channel for coordination
   - No TC Meeting next week (Easter)
   - Django CMS registered trademark? (Andrzej)
       - Who runs django-cms marketplace https://www.django-cms-themes.com/ ? (Andrzej)
       - Nicolai to check and to make a proposal 
6. Review Tasks
7. News & updates for / from dCA Board and MarCom
8. Review approve and post the meeting notes

#### Tasks & Initiatives

https://github.com/django-cms/django-cms-mgmt/projects/1

- [ ] Present the PR's about MenuRenderer & ModalDialog to PR Review (Jacob)
- [ ] Test CMS with django-filer https://pypi.org/project/django-filer/2.1rc3/ (all)
- [ ] django CMS develop documentation - copy the latest accross to v4 (Mario)
- [ ] port manual installation instructions from django cms 4 migration project to quickstart project (Andrew)
- [ ] django-treebeard 4.5.1 fix released in 3.7 and 3.8 (**blocked**)
- [x] Github Action for django-cms repo: Proof of concept (Mario)
- [x] Test Dash and to present results (Vinit)
- [ ] Submit pull request to documentation of Dash project (Vinit)
- [ ] Create communication about first cms v4 milestone to cause buzz once quickstart is finished (Nicolai) 
- [x] Set up "projects" for django CMS repository (Nicolai & Mario)



## 19.03.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
3. Review agenda and add missing points
4. Varia: further points raised by Tech Committee members 
    - v4 Workgroup - question: where should v4 tickets go? Mario propopes to create a separate board for v4 and connect it to the django-cms repo, in the django-cms repo v4 issues should be labelled with v4 to distinguish them
        - Proposal to use Github projects was approved by all present
        - Next step: Set up project (Mario & Nicolai) 
    - 4.0.x installer without Docker (Andrzej)
    - Dedicated, visible support channels and instructions for newbies? (Andrzej)
    - Update: Support PR work group announcement released
        - Volunteers so far: Mark, Anatolly, Simon and Francesco 
        - Next: Kick off call / peridical meeting
        - Who leads the group? 
        - Reach out to Iacopo and ask him to lead the group
    - it was decided to set up django CMS readthedocs account and make sure there is a version for the latest v3 versions and v4 
5. Review Tasks
6. News & updates for / from dCA Board and MarCom
7. Review approve and post the meeting notes

#### Tasks & Initiatives

- [x] Django CMS 4.0 Quickstart project working branch (Andrew)
- [x] Nicolai to post an announcement about us looking for support with github issues periodical review, cleanup and organization, as a part of PR workgroup (Nicolai)


## 12.03.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - Wojciech Szydlo (@easyembedded.co.uk)
    - Andrzej Szydlo (@easyembedded.co.uk)
    - Sankar 
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - Update: Github Action (Andrew & Vinit)
        - https://github.com/SocialSchools/django-cms/runs/2094803750?check_suite_focus=true
        - https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/
        - Set up a call with Mario, Vinit, Andrew and Andrzej to document process 
    - Update:  djangocms-blog - Jens-Erik needs support
        - djangocms-blog is maintained by Nephila
        - Jens-Erik to create a ticket at nephila/djangocms-blog repository 
    - Django CMS 4.0 Quick Start package with examples for newbies to encourage to 4.0 instead of 3.x? (Andrew S)
        - Create branch (support/cms-4.0.x)
        - Wojciech to assist with onboarding of new users 
    - Andrew would like to discuss cms Test Matrix findings at the end of the meeting
        - Andrew would like to discuss if the divio ReadTheDocs org should be replaced withour own org or maybe there is a different solution alltogether. We could host the django-CMS documentation directly as a menu inside the site promoting django-CMS itself (https://www.django-cms.org). Jacob wrote a plugin to do that.
6. Review Tasks
7. News & updates for / from dCA Board and MarCom
    - Nicolai to post an announcement about us looking for support with github issues periodical review, cleanup and organization, as a part of PR workgroup
    - Announcement django CMS 4.0 milestone 
        - I need more infos here
9. Review approve and post the meeting notes

#### Tasks & Initiatives
- [ ] Nicolai help to provide clear instructions for integrating PRs / contributing code (i.e. step by step instructions like 1. adhere to rules for PRs, 2. look for a buddy, 3....) also see jazzband.co
- [ ] Django CMS 4.0 Quickstart project working branch (Andrew)
- [ ] Have a workgroup django filer call to discuss django-parler and "upload empty files" (Jacob)
- [ ] Present the PR's about MenuRenderer & ModalDialog to PR Review (Jacob)
- [x] Provide demo pictures for django filer
- [ ] Test CMS with django-filer https://pypi.org/project/django-filer/2.1rc3/ (all)
- [ ] Vinit to test Dash and to present results
- [ ] Shall djangocms-admin-style be mandatory? We don't use and need it, but this can cause issues. Requires some research (Jacob)
- [ ] Create communication about first v4 milestone to cause buzz after quickstart is finished (Nicolai) 
- [ ] django-treebeard 4.5.1 fix released in 3.7 and 3.8 (blocked) 
- [ ] Nicolai to post an announcement about us looking for support with github issues periodical review, cleanup and organization, as a part of PR workgroup (Nicolai)


## 05.03.2021
#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
3. Review agenda and add missing points
4. Varia: further points raised by Tech Committee members 
    - [Nicolai & Victor] proposition - review the github issues backlog periodically (eg once per month)
        - Andrew was managing PR workgroup when he could, but he needs support
        - We agree that we need a periodic call
        - Nicolai to post an announcement about us looking for support with github issues periodical review, cleanup and organization. As a part of PR workgroup.
6. Review Tasks
7. News & updates for / from dCA Board and MarCom
8. Review approve and post the meeting notes

#### Tasks & Initiatives
- [ ] Announce Testing & QA Contribution Program for service providers (Nicolai)
- [ ] Nicolai to organize design / ux direction 
- [ ] set up testing log (google spreadsheet?) (Nicolai)
- [ ] Create a survey for the project template workgroup (Nicolai & Victor)
- [ ] Enhance contributing guidelines based on jazzband.co (Nicolai help to provide clear instructions)
- [ ] Django CMS 4.0 Quickstart project working branch (Andrew)
- [ ] Have a workgroup django filer call to discuss django-parler and "upload empty files" (Jacob)
- [ ] Present the PR's about MenuRenderer & ModalDialog to PR Review (Unknown owner??)
- [ ] Vinit to test Dash and to present results
- [ ] Provide demo pictures for django filer (all who is all?)
- [ ] Test CMS with django-filer https://pypi.org/project/django-filer/2.1rc3/ (all)
- [x] Django CMS Demo - fix the deployment (Victor & Angelo)
- [ ] Shall djangocms-admin-style be mandatory? We don't use and need it, but this can cause issues. Requires some research (Jacob)
- [ ] Create communication about first v4 milestone to cause buzz (Nicolai)
- [ ] django-treebeard 4.5.1 fix released in 3.7 and 3.8

## 26.02.2021 

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - (Deniz) (workgroups: TBA)
    - Paul (workgroups: v4 & Django 3.2)
    - Francesco (workgroups: v4 & Django 3.2)
    - Anatolly
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee 
    - Info Update: Next TC meeting - Nicolai absence - Who can lead the meeting? -> Andrew  
7. Review Tasks
8. News & updates for / from dCA Board and MarCom
    - Milestone: Working v4 project - boot up and test 
10. Review approve and post the meeting notes

#### Tasks & Initiatives
- [x] django CMS 4.0 Quickstart project working branch 
- [x] Create new workgroup for Django 3.2 (Nicolai)



## 19.02.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - Marcel 
    - Anatolly
    - Francesco
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - Update: Treebeard issue (Andrew)
            - main concern: content being lost (fundamental flaw in the cms) / not a problem of v4 
        - What are our learnings? 
            - keep the branches up to date (maintenance)
            - CMS CI high priority / speed up Github Action -> Vinit will proceed
    - Update: Release 3.9 - What needs to be done?
        - Video Tutorial "[How to do a release](https://drive.google.com/drive/folders/1j7yLnLpWGl-s-q4drVSkwoyq6KVebs_t)" by Angelo 
        - #workgroup-release-management 
7. Review Tasks
8. News & updates for / from dCA Board and MarCom
    - Announcing EOL for django CMS 3.6
9. Review approve and post the meeting notes

#### Tasks & Initiatives
- [x] Nicolai to adjust issue templates for better issue management 



## 12.02.2021 

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest intro
    - Mahmud
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - Update Contributor Onboarding / Issue Management (Mario, Vinit, Victor, Nicolai)
        - we should improve the workgroup description and move the details into tech briefs where possible
        - we will improve the issues templates
        - we need to assign responsible people for the tickets review, eg as part of the #workgroup-pr-review
            - we also can better issue labels, eg "needs-volunteers"  
        - Notes:
            - Issue Triage necessary
            - Ask dCA members for contribution 
6. Review Tasks
7. News & updates for / from dCA Board and MarCom
    - django CMS demo is not working (Victor and Angelo are working on the fix)
    - Wagtail Sprint event as an example for open source events 
9. Review approve and post the meeting notes

#### Tasks & Initiatives
- [x] Share Google doc to blog article with TC team on Slack (Nicolai)
- [x] Fork quickstarter project on Github (Vinit)



## 05.02.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest intro
    - Vel (https://github.com/vkuberan)
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - Update: Help us improve [django CMS vs Wagtail article ](https://www.django-cms.org/en/blog/2021/02/03/django-cms-vs-wagtail-which-cms-is-best-for-your-website/)
        - Notes:
            - Share google doc with tc team on Slack  
            - Who is the target the audience? Developer or people who evaluate? Maybe we need two comparison articles 
    - Update django filer (Jacob)
        - In django-filer, shall we allow to upload empty files?
        - Notes: 
            - Jacob: "Not allow it, because it makes no sense" 
        - How to handle fields containing human readable strings for multilingual installations. Shall we depend on django-parler?
        - Notes:
            - Discuss in a separate call 
        - We must update django-filer's docs. For this we need demo images to create screenshots using the new SVG based icons.
        - Notes: 
            - Daniele has no capacities to write documentation atm 
            - Find community help for documentation 
            - Proposal by Andrew: Define what is required / a list of things that need to be changed )
    - Update Github Action (Vinit)? 
        - Next Steps: 
            - dCA to fork it 
            - Keep aware of upstream changes 
    - Update: Possibility to Sphinx generated documentation inside django CMS instance -> please reach out to jacob for more information 
7. Review Tasks
8. News & updates for / from dCA Board and MarCom 
9. Review approve and post the meeting notes

#### Tasks & Initiatives
workgroup to get a decision on how to move forward with it (Jacob) 
- [x] Coordinate a follow up call with people who're interested in the multisite and its use cases, that would be - Mario, Victor, Jacob, Iacopo (Nicolai)
- [x] Idea to create a repo "RFC" and transfer workgroup spreadsheets to issues - run idea past Mario (Nicolai) 
- [x] Reasearch how to upload docs to Dash (popular offline documentation browser) (Vinit) 
- [x] Transfer Divio Quickstarter to django CMS repository (Daniele)
- [ ] Create a survey for the project template workgroup (Nicolai & Victor)
- [x] Nicolai to get in touch with Iacpopo to discuss status of "djangocms-blog - improve admin"-workgroup and to help onboard new contributor 




## 29.01.2021

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest intro
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - Onboarding new contributors - what's the best way?
        - Multisite workgroup kick off 
            - Notes: According to Victor, only documentation work is needed here. We can do a follow up call with people who're interested in the multisite and its use cases, that would be - Mario, Victor, Jacob, Iacopo
        - djangocms-blog - improve admin workgroup
            - Notes: Nicolai to get in touch with Iacopo to get update about the workgroup
        - Revisit of [workgroup spreadsheet](https://docs.google.com/spreadsheets/d/1gfI8IKz84u-YvE61eePCD-lAbn1haghOiqkvSdO-1yg/edit#gid=1074764488) ?!
            - Notes: Spreadsheet clean up - better descriptions. Idea to move workgroup to issues in a RFC repository.
    - Update: Outcome documentation session
        - Simplify documentation and remove redundant or outdated content 
        - Focus on development topics
    - Update: [First video of django CMS 4.0 video series released](https://www.youtube.com/watch?v=72SficeO9N4)
6. Review Tasks
7. News & updates for / from dCA Board and MarCom
8. Review approve and post the meeting notes

#### Tasks & Initiatives
- [x] Record django CM 4 demo video (Andrew)
- [x] Mario / Andrew to add code to v4 demo project repo (Mario & Andrew)
- [x] set up "search" workgroup and onboard workgroup members (proposal: focus on https://github.com/divio/djangocms-internalsearch for django CMS 4?) (Nicolai& Andrew)
- [x] Nicolai to organize Documentation Session 
- [x] Jean-Baptiste and Andrew to investigate Travis issue 
- [x] Jacob asks if MenuRenderer can be configurable.
- [x] Jacob asks if width of ModalDialog can be configurable.


## 22.01.2021 

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest intro
    - Simon 
    - Jens-Erik (https://passiv.de) - member of the dCA 
4. Review agenda and add missing points
5. Varia: further points raised by Tech Committee members 
    - Update: Iacopo on sick leave
    - Update: New [Discord Server](https://discord.gg/PGEDT44h8A)  
        - Introduce: Extend permissions  
    - Update: ["Call for arms" Campaign](https://www.django-cms.org/en/become-community-hero)
    - Update: Pull Requests - who can help?
        - [The slugs of child pages are built incorrectly and return a 404 error when a user adds a custom slug for another language of the parent page #6622](https://github.com/django-cms/django-cms/issues/6622#issuecomment-763574095)
        - [pagetree search results are foldable #6961](https://github.com/django-cms/django-cms/pull/6961) 
        - [Cache not invalidated when using a PlaceholderField outside the CMS #6912 #6956](https://github.com/django-cms/django-cms/pull/6956)
        - [Updated Documentation](https://github.com/django-cms/django-cms/pull/6964)
        - Note: Update Testing Documenation, Documentation Writing Session (2-3 people) -> Nicolai 
    - Update: [Documentation Workshop](https://www.django-cms.org/en/blog/2021/01/22/3-learnings-from-our-documentation-workshop/)  
7. Review Tasks
8. News & updates for / from dCA Board and MarCom 
9. Review approve and post the meeting notes

#### Tasks & Initiatives
- [x] Send a summary to the community with quick wins / 1-2-3 docs 



## 15.01.2021 

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest intro
3. Review agenda and add missing points
4. Varia: further points raised by Tech Committee members
    - [Announcement: New Tech Committee Members](https://github.com/django-cms/django-cms-mgmt/blob/master/tech-committee/about.md) 
        - Approved by Tech Committee 
        - Notes: Decision to give an update on how to become a TC member to the other regular TC weekly guests that were not on the call 
    - If time left: [Review demo script](https://hackmd.io/fLGKNjtLTpu70k_xUV0r7A) (Andrew) 
        - Notes: Nicolai to give feedback on the script and have a follow up meeting with Andrew to help with video recording etc. 
6. Review Tasks
7. News & updates for / from dCA Board and MarCom
    - Andrew released a 3to4 migration script - community call for testing (Nicolai) 
    - Daniele held a documentation workshop - send a summary to the community with quick wins / 1-2-3 docs instructions 
9. Review approve and post the meeting notes

#### Tasks & Initiatives
- [x] Give Vinit access to github org (Nicolai)
- [x] Mario to review https://jazzband.co/ and report on standardization strategies in next TC (Mario)
- [X] Andrew to release 3to4 script in repo (Andrew) 
- [X] Nicolai to onboard 2 devs from Compound Partners into v4 workgroup (Nicolai) 
- [x] search result workgroup to create a test link (Jean-Baptiste)
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

