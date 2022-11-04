# dCA Tech Committee - Tasks and Decisions Log

###### tags: `meeting protocol`

<small>The Tech Committee meetings documentation must follow the format of the [Tech Committee Log Entry Template](/tech-committee/tasks-and-decisions-log-entry-template.md)</small>

- [Tech Committee task board](https://github.com/django-cms/django-cms-mgmt/projects/1)
- [this doc's hackmd url](https://hackmd.io/ddhvq_aqS6my9gwhLddyPg)
- [this doc's github repo url](https://github.com/django-cms/django-cms-mgmt/blob/master/tech-committee/tasks-and-decisions-log.md)
- [Process: Proposing large feature additions](https://github.com/django-cms/django-cms-mgmt/blob/master/contribution%20policy/contribution%20policy.md)

<strong>Policy: If there are no items on the agenda 30 minutes before the meeting, the meeting will be cancelled.</strong>

## dd.mm.2022 TEMPLATE

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Participants: 
3. Guest(s) intro
    - (Name) 
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
6. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
    - V3: https://github.com/orgs/django-cms/projects/1
    - V4: https://github.com/orgs/django-cms/projects/2
7. News & updates for / from dCA Board and MarCom
8. Review approve and post the meeting notes


## 18.11.2022 TEMPLATE

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Participants: 
3. Guest(s) intro
    - (Name) 
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
6. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
    - V3: https://github.com/orgs/django-cms/projects/1
    - V4: https://github.com/orgs/django-cms/projects/2
7. News & updates for / from dCA Board and MarCom
8. Review approve and post the meeting notes

## 04.11.2022 Today

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Participants: Mario, Fabian, Jacob, Mark, Nicolai, Jens-Erik, Mark and Ebenezer
3. Guest(s) intro
    - Ebenezer
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
    - Managing: Visibility of child pages of unpublished pages. 
    - Overall result of discussion: Default behavior is to reflect visibility of individual pages only (independently of parent pages). If there should be a use-case for marking pages as "waiting to be published as soon as parents are published", only then create a setting that could enable this behavior.
6. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
    - V3: https://github.com/orgs/django-cms/projects/1
    - V4: https://github.com/orgs/django-cms/projects/2
7. News & updates for / from dCA Board and MarCom
8. Review approve and post the meeting notes

## 21.10.2022

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Participants: Fabian, Marcel, Luis, Jens-Erik, Jacob , Nicolai
3. Guest(s) intro
    - (Name) 
4. Review agenda and add missing points 
5. Varia: further points raised by Tech Committee members:
6. Review Tasks
    - dCA: https://github.com/django-cms/django-cms-mgmt/projects/1
    - V3: https://github.com/orgs/django-cms/projects/1
    - V4: https://github.com/django-cms/django-cms/projects/2
    - Suggestion by Nicolai: Remove inactive workgroups from website & Slack. Focus only on a few groups
7. News & updates for / from dCA Board and MarCom
    - https://www.neofluxe.com/ 
9. Review approve and post the meeting notes


## 07.10.2022
#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Participants: <br />Luis, Marcel, Jens-Erik, Mark, Andrew, Mike, Jacob, Fabian
4. Review agenda and add missing points 
5. Varia: further points raised by Tech Committee members:
    - (Fabian) Introduce a minimal linter for Django templates for all dca repos. Users have identified hiddeous bugs in templates which use `{{ page.id }}`, e.g. in attributes or javascript. This needs to be `{{ page.id|unlocalized }}` to avoid **breaking a site with page pks of 1000 or more in languages that introduce a thousands separator**. A linter run on pushes will identify these issues. See also https://github.com/django-cms/django-cms/pull/7188. 
        - Decision: No general linter
        - Use `{% localize off %}` template tag at the appropriate place in the template.
        - Reminder: Reviewers need to check for this to avoid reintroducing such a bug
    - (Jacob) For all 3rd party packages dependent on django-CMS we have the problem of versioning. Some packages are compatible with version 3, some with version 4 and some with both. So how shall we handle version numbers? Python offers a solution for this, it's named [epoch](https://peps.python.org/pep-0440/#version-epochs) numbers. By using them we could distinguish, if a plugin is suitable for version 3 or 4. It also would not mess around with the current version numbers.
        - Avenue 1: Make packages universally support v3 and v4 (e.g., ckeditor)
        - Avenue 2: Make new package to become version compatible (e.g., snippets), potentially with epochs
        - Jacob takes discussion to github discussions.
    - (Jacob) `CMS.settings` overwritten when color scheme is switched. That lets the broswer "forget" which side frame is open, which parts of the page tree are folded out. 
        - There's a fix for this needing review: https://github.com/django-cms/django-cms/pull/7407
6. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
    - V3: https://github.com/orgs/django-cms/projects/1
    - V4: https://github.com/django-cms/django-cms/projects/2
7. News & updates for / from dCA Board and MarCom
8. Review approve and post the meeting notes



## 23.09.2022 

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - Luis, Jens-Erik (from Porto), Marcel Wyser, Fabian
3.  Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
    - (Luis) Report Luis' initial work and first commits made to the docs.
    - (Marcel) Update on CMS v4. Marcel inquired on status of CMS v4 and especially on implemtation of search functionality. For running projects it will be important which 3.x version will be LTS.
5. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
    - https://github.com/django-cms/django-cms/projects/2
6. News & updates for / from dCA Board and MarCom
7. Review approve and post the meeting notes

## 09.09.2022

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
    - (Luis) RFC: I would like to share a proposal for updating and improving the documentation. It is available here: https://docs.google.com/document/d/1hPctyKOoxPkWbfqpc_uRVDV4JN-4xWA73RbOlD97SkM/edit?usp=sharing
        - Luis to continue getting familiar with the 3.11 documentation to get started and implement first quick wins, but at the same time already be involved in the 4.0 workgroup. The goal is to create a new documentation for 4.0 in the long run
    - (Jacob) RFC: I would like to change a page in the documentation:
https://docs.django-cms.org/en/latest/how_to/namespaced_apphooks.html
      The current docs refer to outdated 3rd party packages and do not make clear what's their purpose.
      For one of my projects I created a much simpler AppHookConfig and could use that to better explain it.
      (This proposal has been accepted during the meeting).
6. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
    - https://github.com/django-cms/django-cms/projects/2
7. News & updates for / from dCA Board and MarCom
9. Review approve and post the meeting notes

## 26.08.2022

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - Luis Navarro: https://www.linkedin.com/in/luisfnavarro/
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
    - Django CMS user Luis Navarro is interested in volunteering as the Documentation Lead
        - Welcome Luis! Nicolai to give Luis a introduction to the documentation workgroup
    - (Andrew / Mark) - Create a new 4.1 release branch to distance the code from the sponsors releases. Gives a clear break from 4.0. We can justify this because the sponsor requires 4.0 for themselves. Using 4.0.x creates conflicts.  
5. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
    - https://github.com/django-cms/django-cms/projects/2
6. News & updates for / from dCA Board and MarCom
8. Review approve and post the meeting notes


## 29.07.2022

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - (Name) 
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
    - Jacob raised point that v4 may find it useful to implement a library such as django-tree-queries:
    https://github.com/matthiask/django-tree-queries
6. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
    - https://github.com/django-cms/django-cms/projects/2
7. News & updates for / from dCA Board and MarCom
8. Review approve and post the meeting notes


## 01.07.2022

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - Patrick
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
    - (Andrew) Useful tutorials / guides for v4, just port v3 tutorials or more?
        - How do we go about documentation? 
        - Who is going to contribute to it? 
        - Next steps: Reach out to Daniele and ask for direction / draw a plan / we just need guidance 
    - (Andrew) Code repository plan B if GitHub is "Cancelled" for https://www.theregister.com/2022/06/30/software_freedom_conservancy_quits_github/
        - Let's see how the Django project reacts to it
        - Andrew to follow the public discussion to keep us updated 
    - (Andrew) Also review v4 task list in point 5 below?: https://github.com/django-cms/django-cms/projects/2
    - Update Iacopo:  
        - Identify important with issues their project 
            - Andrew to send wish-list to Nicolai 
            - Make sure that django-cms blog is up to date 
5. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
6. News & updates for / from dCA Board and MarCom
    - Applications for Fellowship Program 
        - around 4 applications so far 
        - start soon with interview process 
            - https://www.django-cms.org/en/fellowship-program/
    - Create new Slack channel for marcomm input
        - Everytime an update is pushed to pypi a notification is send to slack or email 
        - Jacob to build a docker image
7. Review approve and post the meeting notes

## 03.06.2022

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - (Name) 
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
    - Mark's Birthday
    - Andrew: Happy birthday Mark. Wheels Distribution at release time. Wheels has been removed from v3 and due to porting now v4 too. Are we / should we be providing wheels binaries for releases?
6. Review Tasks
    - (https://github.com/django-cms/django-cms-mgmt/projects/1)
    - 
7. News & updates for / from dCA Board and MarCom
9. Review approve and post the meeting notes

## 20.05.2022 (Today)

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - (Name) 
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
    - Andrew / Mark: Where should we host our (coding) style guide? ideally protected and versioned.
        - Andrew has a draft as a starting point
        - Add link in [documenation](https://docs.django-cms.org/en/latest/contributing/code.html)
        - Suggestion by Jacob: to use "we" instead of "you" in the documentation 
    - Andrew: Discussion further to last weeks point, Nephila packages appear to be no longer maintained? Both last changed dec 2020:
        - djangocms-blog
            - Fabian has PR's outstanding
        - djangocms-page-sitemap
            - Andrew has PR's outstanding
        - Nicolai to reach out to Nephila and ask if we can move both repos under the dCA umbrella  
    - Andrew: django-cms V4 on Pypi .... Needs blocking mechanism for v3 projects first of course!
      - Update on the progress in the next weeks
      - https://github.com/django-cms/django-cms/pull/7249
    - Jacob: AFAIK Paolo changed the plugin-tree to use recursive CTE instead of django-treebeard. However, the code doesn't say so. Problem of treebeard is, that it is susceptible to race-conditions. They are almost impossible to reproduce, but they happen.
        - Maybe get feedback from the community in [discussion board](https://github.com/django-cms/django-cms/discussions)?
    - Mario: created a compatibility table  
 
5. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
6. News & updates for / from dCA Board and MarCom
     - General Assembly -> Minutes will be sent out soon 
     -
     - News planned:
         - General Assembly summary
         - Launch of Fellowship Program 
         - Anything else? 
    - Simon  
8. Review approve and post the meeting notes


## 06.05.2022 

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - (Name) 
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
    - MCO: [the compatibility table needs updating](https://docs.django-cms.org/en/develop/#software-version-requirements-and-release-notes), Ticket: https://github.com/django-cms/django-cms/issues/7312, can we briefly discuss my [PR](https://github.com/django-cms/django-cms/pull/7313)
    - Andrew: Release numbers for django-cms 4.x proposal https://github.com/django-cms/django-cms/discussions/7149#discussioncomment-2694746
    - Andrew: Nephila packages appear to be no longer maintained? Both last changed dec 2020, I have a patch waiting to be accepted:
        - djangocms-blog
            - Fabian has PR's outstanding
        - djangocms-page-sitemap
            - Andrew has PR's outstanding
 
6. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
7. News & updates for / from dCA Board and MarCom
8. Review approve and post the meeting notes


## 22.04.2022 (CANCELLED)

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


## 08.04.2022

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - (Name) 
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
    - Andrew django-cms develop-4 django 3.2 workstream needs to be protected away from django 4+ changes, maybe release/4.0.1 vs 4.0.x? 4.1 would say 4 was released?
        - Next steps: agree on a branch to capture a stable dj3.2 workstream.  
    - Jacob: In model `cms.Page` the fields `created_by` and `changed_by` are strings containing the username. This is a violation of Codd's 2nd normalization rule and should be fixed by using a foreign key pointing on model `auth.User`. 
    - Mark: Treebeard `NodeAlreadySaved` error coming from 4.5.1 (thought this was only a 4.5 issue). This PR is attempting to allow newer treebeard installations; https://github.com/django-cms/djangocms-attributes-field/pull/52
    - Mark: Possible new bot to analyse PRs; https://lgtm.com/
    - Mark: Stale issue bot PR; https://github.com/django-cms/django-cms/pull/7298
    - Mark: Potential DjangoCon Europe talk on cms v3 & v4?
6. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
7. News & updates for / from dCA Board and MarCom
    - Invitations for GA will go out next week 
    - New workgroup: #workgroup-js-frontend-application 
9. Review approve and post the meeting notes

## 25.03.2022

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
    - Fabian: Build pipeline for frontend js probably requires overhaul by expert.
        - Mark: Time to replace phantomjs? Can Playwright enable this? https://playwright.dev/
        - Decision: Create workgroup "JS Frontend Application" and post proposals there.
    - Jens-Erik: How to deal with PRs where the [fix](https://github.com/MacLake/djangocms-picture/commit/c76cabaafc9d759fb332fec6a0841c90e3179274) is trivial, but a test is demanded that is way more complex? See [issue](https://github.com/django-cms/djangocms-picture/issues/108).
    - End of meeting: Andrew Filer checks demo discussion
5. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
6. News & updates for / from dCA Board and MarCom
    - Preparation for the next General Assembly are underway
    - DjangoCon 2022 in Portugal? https://2022.djangocon.eu/ 
    - Call-to-action regarding new workgroup "JS Frontend Application"
    - New Gold member: famewurk
8. Review approve and post the meeting notes

## 11.03.2022

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - (Name) 
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
    -  Andrew: django-filer checks framework: https://github.com/django-cms/django-filer/pull/1285/files
        -  Opinion of feature?
        -  Decision on modal / popup?
5. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
6. News & updates for / from dCA Board and MarCom
7. Review approve and post the meeting notes

## 25.02.2022

#### Agenda Points
<small>TBD in in the first 5 min of the meeting</small>

1. Add new entry for next meeting from template
2. Guest(s) intro
    - (Name) 
3. Review agenda and add missing points 
4. Varia: further points raised by Tech Committee members:
    - Simon: djangoCMS Documentation is now available for [Dash](https://kapeli.com/dash)
    - Mike: New time for the v4 call next week
        - Wednesday 5.30pm CEST (bi-weekly)
    - Mark: New django setting to acknowledge that someone is using cms v4. Something that can prevent migrations running unless we've got acknowledgement. [Related conversation](https://github.com/django-cms/djangocms-versioning/pull/257#event-6126521892)
    - Jacob: Video tutorials for our users are available.
6. Review Tasks
    - https://github.com/django-cms/django-cms-mgmt/projects/1
7. News & updates for / from dCA Board and MarCom
    - [New article by Mark](https://www.django-cms.org/en/blog/2022/02/22/security-enhancements-for-django-cms/) - check it out 
9. Review approve and post the meeting notes

## 11.02.2022

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


