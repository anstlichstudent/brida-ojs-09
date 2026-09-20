---
title: "Learning OJS 3.3: A Visual Guide to Open Journal Systems"
version: "3.3"
language: en
source: "https://docs.pkp.sfu.ca/learning-ojs/3.3/en/"
license: "CC BY 4.0"
---

# Learning OJS 3.3: A Visual Guide to Open Journal Systems

> **Source:** [PKP Docs — Learning OJS 3.3](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/)  
> **Language:** English  
> **Version:** OJS 3.3 (released February 2021)  
> **Note:** This file combines the chapters from the original guide. Images and videos remain linked to PKP Docs and YouTube.

## Table of Contents

- [Preface](#preface)
- [About Open Journal Systems (OJS)](#about-ojs)
- [Site Administration](#site-administration)
- [Journal Settings](#journal-settings)
- [Website Settings](#website-settings)
- [Workflow Settings](#workflow-settings)
- [Distribution Settings](#distribution-settings)
- [Users and Roles](#users-and-roles)
- [Statistics](#statistics)
- [Tools](#tools)
- [Subscriptions](#subscriptions)
- [User Account Management](#user-account-management)
- [Authoring](#authoring)
- [Reviewing](#reviewing)
- [Editorial Workflow](#editorial-workflow)
- [Production and Publication](#production-and-publication)
- [Attribution and License](#attribution-and-license)

## Preface

Open Journal Systems (OJS) is an open source solution to managing and publishing scholarly journals online. OJS is a highly flexible editor-operated journal management and publishing system that can be downloaded for free and installed on a local Web server.

This guide is a comprehensive manual covering the various functions and configuration options of OJS version 3.3, released in February 2021. It contains information on everything users need to use the software to publish and manage content as a site administrator, journal manager, editor, peer reviewer, and/or author. It provides detailed instructions with screenshots for applying journal and website settings, using and configuring the editorial workflow including making submissions and peer review, managing users, using statistics, and configuring subscriptions. By following this guide, users will be able to successfully submit, edit, publish, and display academic articles on OJS.

---

## About Open Journal Systems (OJS) {#about-ojs}

Open Journal Systems \(OJS\) is an open source solution to managing and publishing scholarly journals online. OJS is a highly flexible editor-operated journal management and publishing system that can be downloaded for free and installed on a local Web server.

It has been designed to reduce the time and energy devoted to the clerical and managerial tasks associated with editing a journal, while improving the record-keeping and efficiency of editorial processes. It seeks to improve the scholarly and public quality of journal publishing through a number of innovations, including enhancing the reader experience, making journal policies more transparent, and improving indexing.

This guide covers OJS version 3.3, released in February 2021, and features significant enhancements over the previous versions of the software. We hope you find it helpful for your publishing projects.

### Background {#background}

This PKP School video explains the background on PKP and OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of background on PKP and OJS](https://www.youtube.com/watch?v=SQfFGwIK2wI)

*OJS is a journal/web site management/publishing system*. OJS covers all aspects of online journal publishing, from establishing a journal website to operational tasks such as the author's submission process, peer review, editing, publication, archiving, and indexing of the journal. OJS also helps to manage the people aspects of organizing a journal, including keeping track of the work of editors, reviewers, and authors, notifying readers, and assisting with the correspondence.

*OJS is flexible and scalable*. A single installation of OJS can support the operation of one or many journals. Each journal has its own unique URL as well as its own look and feel. OJS can enable a single editor to manage all aspects of a journal and the journal's website, or OJS will support an international team of editors with diverse responsibilities for a journal's multiple sections.

*OJS supports the principle of extending access*. This system is intended not only to assist with journal publishing, but to demonstrate how the costs of journal publishing can be reduced to the point where providing readers with "open access" to the contents of the journal becomes a viable option. The case for open access is spelled out over a wide series of articles stemming from this project which are freely available under Research > Publications on the [Public Knowledge Project](https://pkp.sfu.ca/) website.

*The origins of OJS*. The system was first released in 2001 as a research and development initiative at the University of British Columbia, with the support of the Social Sciences and Humanities Research Council of Canada, the Max Bell Foundation, the Pacific Press Endowment, and the MacArthur Foundation. Its continuing development is currently overseen by the Simon Fraser University Library. For more information, see the [Public Knowledge Project website](https://pkp.sfu.ca).

<hr />

### OJS Features {#ojs-features}

Visit our website to learn more about [Open Journal Systems](https://pkp.sfu.ca/software/ojs) and what it has to offer the whole researcher-to-reader workflow, from submission and peer review through to production and distribution.

### Install and Upgrade {#install-and-upgrade}

OJS is easy to install and configure. However, running a web service requires a systems administrator who knows how to deploy web applications. Our Administrator's Guide provides full instructions on how to [download, install and configure OJS](https://docs.pkp.sfu.ca/admin-guide/en).

> If you do not have the expertise, staff or desire to install and manage OJS on your own, [PKP Publishing Services](https://pkp.sfu.ca/hosting-services) provides complete hosting solutions for every budget.

### What's New in OJS 3.3 {#whats-new}

OJS 3.3 has a simplified dashboard navigation menu and new features related to submission management, communicating with users, and accessibility. This section will outline the main changes so you know what to expect when you upgrade to OJS 3.3. You can also watch [a video that demonstrates new features in OJS 3.3](https://youtu.be/3D_hS4Bd-Y8), created by [PKP Publishing Services](https://pkpservices.sfu.ca).

Many of these changes are applicable also to Open Monograph Press (OMP) and Open Preprint Systems (OPS).

If you are upgrading from OJS 2 and want to see an overview of changes in OJS 3.X, see [What’s New In OJS 3 in a previous version of this guide](https://docs.pkp.sfu.ca/learning-ojs/3.1/en/introduction#whats-new-in-ojs-3) and PKP’s guide to [Upgrading from OJS 2 to OJS 3](https://docs.pkp.sfu.ca/upgrading-ojs-2-to-3/). Please note that you will need to first upgrade from OJS 2 to OJS 3.2, and from there upgrade to OJS 3.3.

For a summary of changes in OJS 3.3 that are relevant to developers and development, please see the [Release Notebook for OJS OJS/OMP/OPS v3.3](https://docs.pkp.sfu.ca/dev/release-notebooks/en/3.3-release-notebook)

#### Dashboard Interface and Navigation Menus

There are some changes to the dashboard interface and navigation menus for logged in users in OJS 3.3.

Journal Managers, Editors, Reviewers, Authors, and others who log in may notice a change in the main navigation menu on the left side. In 3.3, only users in roles who have access to the Settings menus (Journal Managers and Editors) will see the left-hand navigation menu. There are also additional menu links for Issues, Announcements, and Payments, and some of the menu links have moved.

![The dashboard that Journal Managers see when logged in](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.3-navigation-menu-dashboard-jm.png)

Users in other roles will not see the menu because they can only access the Submissions part of the menu.

![The dashboard that Authors see when logged in](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.3-navigation-menu-dashboard-author.png)

A user can now access their user profile and select a language on multilingual journals by clicking the person icon on the top right corner.

![The menu where users can edit their profile and select a language](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.3-navigation-menu-dashboard-user-menu.png)

The link from the dashboard to the public journal site home page has moved. A Journal Manager or Editor can now view the public journal site by clicking the name of the journal that appears on the top left corner of the page. For multi-journal installations, you can click the site map symbol on the top left corner of the page and then a list of journals in the installation will appear below and you can select the site you want to view.

![The link to view the public journal site](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.3-navigation-menu-dashboard-view-journal.png)

#### Editorial Workflow

##### Uploading submission files

During submission, Authors can upload multiple files at once as well as drag-and-drop files. They are no longer asked to enter metadata such as a description, license, etc. This information can be entered during the workflow, where the old file upload wizard is still in use. You can find further instructions in the [Authoring chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/authoring#step-2).

[Video: A short video that demonstrates how files can be uploaded in OJS 3.3.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-upload-submission-files.mp4)

##### Submission filters

All Active and Archived submissions can now be filtered by assigned issue and assigned Editor. Only Journal Managers can filter by assigned Editor. You can find further instructions in the [Editorial Workflow chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/editorial-workflow#submission-dashboard).

##### Reverse a declined decision

A new editorial action allows Editors to reverse a declined decision in the submission and review stages. After a declined decision is reverted, the submission is restored to its previous stage and review round if active. You can find further instructions in the [Editorial Workflow chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/editorial-workflow#assigning-the-submission).

##### Delete only declined submissions

Only declined submissions can be deleted from the submissions list. You can find further instructions in the [Editorial Workflow chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/editorial-workflow#archives).

##### Review type terminology

In previous versions of OJS, the review types were “Double Blind,” “Blind,” and “Open.” In OJS 3.3 these have been changed to “Anonymous Reviewer/Anonymous Author,” “Anonymous Reviewer/Disclosed Author,” and “Open.”

##### Category displayed on article page

An article’s assigned categories now appear on the article landing page. You can find further instructions in the [Journal Settings chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/journal-setup#categories).

##### Disable submissions

Journal Managers and Editors can configure the Workflow Settings to disable all submissions for a journal. This can be used by journals that are no longer accepting new content. You can find further instructions in the [Journal Settings chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/journal-setup#sections).

#### User Management and Communication

##### Export users

There is now an export tool available under Tools > Import/Export that can be used to export users to a CSV file. This can be used to import users into third-party mailing services. You can find further instructions in the [Users and Roles chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/users-and-roles#email-users).

##### Notify users

OJS 3.3 has a much-requested feature to notify, or send a message, to all users in a role. See the [Users and Roles chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/users-and-roles#email-users) for more details.

##### Filter email templates by workflow stage

When managing and editing email templates under Workflow Settings > Email, Journal Managers and Editors can filter the email templates by workflow stage. You can find further instructions in the [Workflow Settings chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-workflow#filters).

#### Accessibility

In 2019 OJS was audited for accessibility to people with disabilities and use assistive technology. All of the changes that were recommended by the audit have been implemented in OJS 3.3, including an accessible Default Theme and custom blocks now requiring a title. More information about custom blocks is in the [Website Settings chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-website#custom-block-plugin).

#### For Multilingual Journals

OJS 3.3 has a number of new features that improve usage for journals working and/or publishing in multiple languages.

##### Date and time formats

Date and time formats can now be specified for each journal and locale/language. Further instructions are in the [Website Settings chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-website#date-and-time).

##### Right-to-left languages

There is better support for languages that read right-to-left, such as Arabic, Farsi, and Hebrew, in the rich text editor that appears in many form fields in OJS.

##### Remote URLs
Navigation menu items with remote URLs can now have different remote URLs for each language.

### Community Contributions {#community-contributions}

The OJS team encourages contributions from the developer community. If you are interested in getting involved in making OJS even better, we welcome your participation.

Excellent examples of community contributions include the vast array of languages that OJS is available in; and third-party plugins posted to the [community forum](https://forum.pkp.sfu.ca/) and the archived forum page.

We also welcome software testing and bug reporting contributions.

### Support {#support}

PKP offers the following free support resources for OJS:

* [PKP Docs Hub](https://docs.pkp.sfu.ca/): User guides, developer documentation and publishing tips for all of our software. Also includes links to community developed videos.
* [PKP Community Forum](https://forum.pkp.sfu.ca/): An online discussion board where you can ask questions, answer questions, and share ideas.
* [PKP School](https://pkpschool.sfu.ca/): A collection of online, open, and self-paced courses designed by PKP experts in English and Spanish. Includes video tutorials on Setting up Your Journal; the Editorial Workflow in OJS 3; and Becoming an Editor.

There is also a “Help” link on the top right corner of every page in OJS, OMP, and OPS where you can find information about the current page and its functions.

For questions about a particular journal site, such as submission requirements, contact that journal directly, using the contact information listed on the journal's **About** page.

> **Original chapter:** [About Open Journal Systems (OJS)](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/about-ojs)

---

## Site Administration

As part of installing OJS, you will have created a Site Administrator user account. When you log into OJS with that account you will have access to Site Administrator settings from the Dashboard.

You will be able to create new hosted journal instances, manage language support across your system, and perform other administrative functions.

More technical information about administering an OJS site, including upgrades, email, statistics, and importing and exporting, is available in the [Administrator's Guide](https://docs.pkp.sfu.ca/admin-guide/en/).

### Site Management {#site-management}

To get to Site Management, login as the Site Administrator, and choose Administration from the left menu.

![OJS site admin main menu with 2 options: site management and administrative functions.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-sa-site-admin.png)

#### Hosted Journals

From here, choose Hosted Journals. On the resulting page, you will see all of the journals in this OJS installation. In the example, below, there is only one.

![OJS hosted journals menu with 1 existing journal.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-sa-hosted-journals.png)

To edit the existing journal, click on the blue arrow to the left of the journal name. You will see options to edit, remove, or update the settings.

![Existing journal editing options: edit, remove, settings wizard, users.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-sa-hosted-journals-edit.png)

**Edit** will let you change the title, description, or path.

![Existing journal editing screen with title, description and path fields available to edit.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ch4-hosted-journals-edit-modal.png)

**Remove** will let you delete the journal from the installation. You will be asked to confirm that you really do want to do this, as it is irreversible.

![Confirmation screen for journal deletion.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ch4-hosted-journals-remove.png)

**Settings Wizard** will take you to the various settings options for that journal.

Restrict Bulk Emails allows the journal administrator to disable the ability to send bulk emails to certain roles. The bulk email feature can be enabled under [Site Settings > Bulk Emails](#bulk-emails). A journal manager will be unable to send bulk emails to any roles that you select under the “Disable Roles” setting. Use this setting to limit abuse of the email notification feature. For example, it may be safer to disable bulk emails to readers, authors, or other large user groups that have not consented to receive such emails.

![Settings wizard screen with the restrict bulk emails tab selected.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-admin-restrict-bulk-emails.png)

We'll go over the remaining settings in detail in the Settings chapters.

![Settings wizard screen with the masthead tab selected.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ch4-hosted-journals-settings-wiz.png)

**Users** will allow you to add and manage users associated with this journal.

![Users tab with a list of current users.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-sa-hosted-journals-users.png)

Back on the Hosted Journals page, you can use the Create Journal link to add a new journal to this OJS installation. From the resulting form, fill in the fields with the new information.

![Create journal screen with title, description and path fields available to fill out.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ch4-hosted-journals-create.png)

> Note: If you do not want the new journal to be visible yet, uncheck the _Enable this journal to appear publicly on the site_ box.

#### Site Settings

This section will appear if you have two or more journals, and allow you to add information regarding your overall OJS installation, not individual journals.

##### Site Setup

This includes the name of your site, a site logo, an introductory statement about your site, a site footer, a redirect option (if you only plan to have one journal on this installation), contact information, a minimum password length for registered users, style sheet and theme options, and sidebar management.

You will have the opportunity to provide details about your individual journal(s) at a later stage.

![OJS admin menu with site setup tab selected.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-sa-site-settings.png)

##### Languages

OJS is designed to be a multilingual system, allowing journals supporting a wide variety of languages to be hosted under a single site. When you install OJS, you can select one or more languages for your site.

The Site Administrator can set the default language of the site and install additional locales to make other languages available for use by journals. Journal Managers can then manage their own language settings under Website Settings > Languages. See the [Website Settings chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-website) for details.

Under Administration > Site Settings > Languages you can see a list of languages that are installed on your site, enable languages, and set any language as the Default Locale, which means it is the language that users will first see when first visiting the site.

![OJS admin menu with languages tab selected.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-sa-languages.png)

To add another language:

1. Click Install Locale
2. Check off the locales you would like to install
3. Click Save

After installing the new locale, you will have to enable it on the Site Settings > Languages page.  Further configuration of the language’s availability on the site can be done under Website Settings > Languages by a Journal Manager. See the [Website Settings chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-website) for details.

OJS 3 doesn't yet have as many translations as OJS 2, but we expect to have more contributed over time. Contributions are always welcome.

##### Plugins

From here, you can choose to enable or disable various plugins, making them available (or not) to all of the journals on this OJS installation.

![OJS admin menu with plugins tab selected.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-sa-plugins.png)

##### Navigation Menus

Use this section to modify your site-wide menus. You can learn more about configuring menus in the Website Settings chapter.

![OJS admin menu with navigation menus tab selected.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-sa-menus.png)

##### Bulk Emails

OJS 3.3 has the option to allow bulk emails to be sent to several user groups in a journal at one time. See [Users and Roles > Email Users](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/users-and-roles#email-users). As the site administrator, you can use the site settings to select the hosted journals that will be allowed to send bulk emails.

Note that misuse of this figure to send unsolicited email may violate anti-spam laws in some jurisdictions and may result in your server’s emails being blocked as spam. Seek technical advice before enabling this feature and consider consulting with journal managers to ensure it is used appropriately.

![OJS admin site settings with bulk emails tab selected.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-site-settings-bulk-emails.png)

It is possible to disable sending bulk emails to certain roles for individual journals under [Hosted Journals](#hosted-journals) > Settings Wizard.

#### Next Steps

Once you've created a journal and configured the site settings, you may want to create a user account for the Journal Manager or Editor -- see the [Users and Roles chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/users-and-roles) for details.

<hr />

### Administrative Functions {#administrative-functions}

This section provides detailed information about the server on which your OJS installation is running.

![OJS site admin main menu with 2 options: site management and administrative functions.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-sa-admin-functions.png)

#### System Information

Use this section to find out details about the server running your installation.

![System information screen displaying current version, version history and server information.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-sa-sysinfo.png)

OJS Version information shows which version is currently installed, and your version history including any upgrades. You can click the Check for updates link to see if you are using the most recent version of OJS.

The Server Information provides details about the server environment hosting your OJS installation.

The OJS Configuration section displays all of the configuration options and their values as they are in _config.inc.php_.

You can find more information about _config.inc.php_ configuration parameters in the file itself.

The final section on this page displays additional server information: your operating system, PHP version, server and database information. You can also view extended PHP information by clicking the Extended PHP information link (this displays the output of `phpinfo()`)

All of this information can be useful when trying to troubleshoot a problem.

#### Expire User Sessions

Clicking _Expire User Sessions_ immediately clears all active user sessions in the system, requiring any user that is currently logged in to sign in to the system again. This can be useful before an upgrade, to ensure all users are logged out.

#### Clear Data Caches

Clicking _Clear Data Caches_ clears all cached data, including locale information, help cache, and search cache. This function may be useful to force data to be reloaded after customizations have been made.

#### Clear Template Cache

Clicking _Clear Template Cache_ clears all cached versions of HTML templates. This function may be useful to force templates to be reloaded after customizations have been made.

#### Clear Scheduled Task Execution Logs

If scheduled tasks have been enabled for your journal, clicking _Clear Scheduled Task Execution Logs_ will delete the task execution log files from your server. The execution log files include dates that correspond to previously completed scheduled tasks (e.g. sending automatic email review reminders).

> **Original chapter:** [Site Administration](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/site-administration)

---

## Journal Settings

The Settings section allows you to configure your OJS installation to best meet your publishing needs.

You can find the Settings in the left menu panel when you are logged in as a user with Journal Manager permissions.

![OJS dashboard View for Journal Managers with links to Settings menu and its submenus in left-hand sidebar.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-journal.png)

It consists of Journal Settings, Website Settings, Workflow Settings, and Distribution Settings, which will be covered in the next 4 chapters.

The Journal Settings page includes details about the journal.

Use the tabs to navigate to the different sections of Journal Settings: Masthead, Contact, Sections.

![OJS dashboard view of Journal Settings with navigation tabs for the Settings submenus across top portion of page content.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-settings-journal-page.png)

### Masthead {#masthead}

This PKP School video explains how to configure the Masthead in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure the Masthead in OJS](https://www.youtube.com/watch?v=DMi6izQ7Pyw)

**Journal title** is the name of your journal. E.g., Journal of Software Documentation

**Journal initials** are the initials of the journal. E.g., JSD.

**Journal Abbreviation** is the abbreviation of your journal name. E.g., JSoftDoc.

**Publisher** is the name of the organization publishing the journal.

Note that the publisher name entered here is used for metadata but will not be displayed on your site. To show the publisher name on your site you can enter it under Journal Settings > Contact > Mailing Address. You can also add it under "About the Journal" below.

**ISSN** (International Standard Serial Number) is an eight-digit number which identifies journals. It is managed by a world wide network of National Centres coordinated by an International Centre based in Paris, backed by Unesco and the French Government. A number can be obtained from the [ISSN web site](https://www.issn.org/). This can be done at any point in operating the journal.

OJS journals will typically have an online ISSN, but some may also publish a print version, which requires a different print ISSN.

Please note that the ISSN entered here is used for metadata but will not be displayed on your site. It's recommended that you also add the ISSN to the footer of your site. You can do this under Website Settings > Appearance > Footer.

**Journal Summary** is a brief description of your journal. If you are on an OJS installation with multiple journals, this text will appear with your journal listing. You can also choose to add the journal summary to the journal homepage in the Website Settings.

**Editorial Team** allows you to add the names of your editorial team or anyone else you wish to mention. This will appear on the public website under About &gt; Editorial Team.

**About the Journal** is a space to add any information about your journal which may be of interest to readers, authors, or reviewers.

This could include your open access policy, the focus and scope of the journal, copyright notice, sponsorship disclosure, history of the journal, a privacy statement, and inclusion in any LOCKSS or CLOCKSS archival system.

Hit the **Save** button to save your changes.

### Contact {#contact}

This PKP School video explains how to add journal contacts in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to add journal contacts in OJS](https://www.youtube.com/watch?v=HTDZRG7XEqw)

Use this section to add journal contacts.

![OJS dashboard view of Journal Settings submenu Contact where information can be added in text fields.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-settings-journal-contact.png)

**Principal Contact**: Add contact information for the journal's main contact person, including name, email, phone, affiliation, and mailing address for the journal. This will appear on the journal's Contact page.

**Technical Support Contact**: Add contact information for the journal's technical support person. This information will appear on the journal's Contact page and also in different points in the workflow to offer assistance to users.

Hit the **Save** button to save your changes.

### Sections {#sections}

This PKP School video explains how to configure Sections in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure sections in OJS](https://www.youtube.com/watch?v=IMotkKrDZyc)

Use this page to configure the different sections of your journal. E.g., Articles, Editorials, Reviews, Commentary, etc. OJS requires at least one section, and creates an "Articles" section by default. You can create new sections, edit existing sections, or delete sections. The sections will appear for an author to select when they make a submission and they will be used to organize the articles in your published issues. You can also assign editors to specific sections. This part of the guide explains how you can configure sections.

![OJS dashboard view of Journal Settings submenu Sections with links for Order and Create Section and editable list of current sections.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-settings-journal-sections.png)

Submissions can also be disabled for individual sections. This can be done in instances where a section is no longer being used, in order to prevent articles from being submitted to a particular section.

A section can be marked as “Inactive” in the section settings:

![View of Journal Sections in the OJS dashboard. Red box surrounding checkbox next to the section Articles indicates where to mark it inactive.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-section-setting-inactive.png)

You can modify sections by clicking on the blue arrow to the left of the section name. This will reveal options to edit or delete the section.

#### Edit a Section

Selecting the edit link will open a new window with different configuration options.

![New window displaying a section's current settings that is editable.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-settings-website-settings-sections-edit-1.png)

From here, you can change the name or abbreviation of the section.

**Section Policy**: Use this field to add important details such as submission requirements, peer review, etc.

**Word Count**: Use this to limit the number of words for abstracts in this section.

**Section Options**: Each section can have different settings, including whether it is indexed, peer-reviewed, accepts unsolicited submission, or listed in the table of contents.

For example, an Editorial section will not typically be peer-reviewed.

Submissions can also be disabled for individual sections. This can be done in instances where a section is no longer being used, in order to prevent articles from being submitted to a particular section.

You can check off "Will not be included in the indexing of the journal" for sections that contain front matter, back matter, and anything else that might clutter the search index unnecessarily.

![A window for entering Word Count, Review Form, and Section Options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-section-options.png)

**Identify items published in this section as a\(n\)**: This is used by some systems. Note that it is not a required field.

**Section Editors**: If you have editors enrolled in your journal, you will see them listed here and can assign one of them to the section. This means any submissions made to the section are automatically assigned to the editor, saving you from manually assigning an editor.

Hit the **Save** button to save your changes and return to the Sections page.

#### Create Section

From the sections page, select the Create Section link to open a blank window, exactly the same as the window used for editing a section described above.

![A new window for entering section information in text fields and selecting section options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-settings-website-settings-sections-create.png)

Fill in the details and hit Save to record your work.

#### Restrict Section Submitters

Each section allows to restrict submissions by checking the "Items can only be submitted by Editors and Section Editors" checkbox.

![The list of options for restricting a section. Items can be selected from list by checking the box to the left of the item.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-settings-journal-sections-restrict.png)

If this checkbox is checked for all sections, authors will not be able to submit to the journals. Authors who select New Submission from their dashboards will now see the message "This journal is not accepting submissions at this time."

![Screenshot example of message displayed on a journal New Submission page.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-journal-not-accepting-submissions.png)

#### Order Sections

When you have more than one section created, you will see an Order link. Use that to reorder how those sections display on your journal website.

![A list of available sections from top to bottom of page in OJS dashboard.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-settings-journal-sections-order.png)

Hit the **Done** button when you are finished.

#### Delete Sections

You can only delete a section if there are no articles assigned to it. If you want to delete a section that has articles assigned to it, you will need to move the articles to a different section first. Then click the blue arrow below the section name to reveal the **Delete** link, then click the link. OJS will ask if you want to permanently delete the section and you can click **Yes**.

### Categories {#categories}

This PKP School video explains how to create categories in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to create categories in OJS](https://www.youtube.com/watch?v=Y97U1icfEPw)

In OJS 3 you can create Categories to organize your articles into thematic collections and provide another way for readers to access your content. Categories can be displayed as a browse block on your journal site and readers can select a category to view all articles in that category. You can place an article in a category by editing its metadata, which is explained in the [Production and Publication chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/production-publication). This section explains how to create and edit categories.

![OJS dashboard view of Journal Settings submenu Categories with links for Order and Add a Category and editable list of current categories.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-categories-menu.png)

To create a new category:

* Click Add Category
* Enter a name for your category that will be displayed to readers
* Enter a path for the category’s URL on your site
* Enter a description which will appear above the list of articles in the category
* You can optionally change the order of the articles by date or title
* Optionally add an image which will appear at the top of the category’s page
* Click Save

![A new window for entering category information in text fields and selecting category options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-create-category.png)

To edit a category:

* Click the name of the category you want to edit
* Make the changes
* Click OK

To remove a category:

* Click the blue arrow next to the category you want to remove
* Click the Remove button that appears below
* Confirm that you want to remove the category

To display categories on your website you can go to Website Settings > Sidebar Management and place the Browse block on your sidebar.

> **Original chapter:** [Journal Settings](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/journal-setup)

---

## Website Settings

The Website Settings allow you to configure how your journal's website looks and operates. It consists of 3 main tabs for Appearance, Setup, and Plugins.

![OJS dashboard view of website settings menu.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-web-appearance.png)

### Appearance {#appearance}

This PKP School video explains how to configure your journal's appearance in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure your journal's appearance in OJS](https://www.youtube.com/watch?v=4i5uRgzFHfg)

#### Theme

The theme determines the overall design or layout of your site. Several different theme options are available and you can try them out without affecting your site's content or configuration.

First you can ensure that all available themes have been enabled on your site.

1. Go to the Plugins tab under Website Settings.
2. Scroll to the bottom and find Theme Plugins.
3. Check the box next to each plugin to enable it.

You can also look for additional themes in the Plugin Gallery and install and enable those.

Now that you have all available themes, return to the Appearance tab to try out different themes.

1. Under Theme you will see a drop-down list of themes. Select one.
2. Scroll to the bottom of the page and click Save.
3. The theme may have additional sub-themes or configuration options available. To make these appear, refresh the page in your browser.
4. If you select a different sub-theme or change the colour scheme or other design features, click Save at the bottom of the page again.
5. Open your site's home page in a new tab or window of your browser to see how the site looks with the new theme or sub-theme and with different configuration options.
6. If you do not see the changes appear on your site, you may need to clear the cache under the Administration menu.

As of OJS/OMP/OPS 3.3, the **Default Theme** has been externally audited for accessibility and adheres to best practices like colour contrast, keyboard navigation, and form/link focus. [PKP Accessibility Statement](https://docs.pkp.sfu.ca/accessibility-statement/) contains further details.

If you would like to make minor changes to your site's design and layout, you can upload a **Journal Stylesheet** in Website Settings > Appearance > Advanced.

- **Typography**: Quickly choose the fonts for your journal. This option may or may not be available depending on the selected theme.

- **Colour**: Quickly change the colour of your journal's header. This option may or may not be available depending on the selected theme.

- **Journal Summary**: Check this off to show the journal summary on the homepage. You can add your journal summary under Journal Settings > Masthead. This option may or may not be available depending on the selected theme.

- **Header Background Image**: Check this off if you if you want the uploaded homepage image to be shown as the header background.

For further theme customization options, consult the [Designing Your Journal](https://docs.pkp.sfu.ca/designing-your-journal/en/) guide. Note that changes made to the themes may impact journal accessibility.

#### Setup {#setup-1}

Where you can upload images (logo, thumbnail, homepage) to your sites main page, enter footer information, and configure your sidebar menu.

- **Journal thumbnail**: Upload a small logo or image representative of the journal that will be used in lists of journals on this OJS installation. This will only be used on OJS installations with multiple journals.

- **Homepage Image**: Uploading an image here will will place it on your journal's home page.

- **Page Footer**: Enter any images, text or HTML code that you'd like to appear at the bottom of your website.

- **Sidebar**: This allows you to move different blocks in or out of the sidebar in the reader interface. You can also create a custom block using the [Custom Block plugin](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-website#custom-block-plugin)

#### Advanced

Where you can upload your journal stylesheet, Favicon, and Additional Content.

- **Journal Style Sheet**: Use this to upload a unique style sheet for your journal. Instructions on modifying the CSS are available in the [Designing Your Journal: Creating a Stylesheet](https://docs.pkp.sfu.ca/designing-your-journal/en/creating-stylesheet) guide.

If you would like to make more significant changes to the design or give your site an entirely unique look, you can develop your own theme or child theme. Instructions are available in the [PKP Theming Guide](https://docs.pkp.sfu.ca/pkp-theming-guide/en/).

- **Journal Favicon**: Add a [favicon](https://en.wikipedia.org/wiki/Favicon) to display in the reader's browser address bar.

- **Additional Content**: Any text entered here will appear on your homepage.

Hit **Save** to record your changes.

### Setup

#### Information

This PKP School video explains how to configure the Information settings in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure Information settings in OJS](https://www.youtube.com/watch?v=48qU18uqqkg)

Use these fields to modify the text in the For Readers, For Authors, For Librarians pages on the journal website.

![OJS dashboard view of Information menu with boiler plate text in the fields for readers and for authors.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-web-info.png)

Remember to hit **Save** to record any changes.

To remove these fields and their contents from displaying publicly on the website's user interface, deselect the Information Block in Website Settings > Appearance > Sidebar Management.

#### Languages

This PKP School video explains how to configure the Language settings in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure the language settings in OJS](https://www.youtube.com/watch?v=VU5kAPOqNPc)

OJS is multilingual, which means that the interface, emails, and published content can be available in multiple languages and authors can make submissions in one or more languages on a single site or journal. When you install OJS, you can select one or more languages for your site.

Under Website Settings > Languages you can see a list of languages or locales installed on your site and configure how the languages are used in your journal. Consider carefully how you want to configure and use languages in your journal because significant problems can occur if you change the settings later.

![OJS dashboard view of Languages menu with English and French options, English option selected as primary locale.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-web-lang.png)

- **Primary Locale**: One language must be set as the primary locale, which means the language the journal appears in by default.

- **UI**: If you want the journal’s front end and back end interface to be available in other languages, select them here. Enabling a language for the UI will allow users to select the language of the application interface. For example, buttons, page titles, and on-screen messages will be in the user's selected language.

- **Forms**: This will enable all selected languages to be available when filling in online forms. Enabling a language for forms will allow text boxes to support multilingual data entry, including the Publication tab for submissions. For example, configuration settings and metadata can be entered in multiple languages.

- **Submission**: If you want authors to be able to make submissions in other languages, select them here. This will allow authors to select a language when they make a submission and add metadata in selected languages when uploading their submission.

Additional languages can be installed on your site by an Administrator – see [the Site Administration chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/site-administration) for details.

If enabling multiple languages to appear in the UI, make sure that in Website Settings > Appearance > Sidebar Management the Language Toggle Block is selected to make that feature available to users.

#### Navigation

This PKP School video explains how to configure the Navigation settings in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure navigation settings in OJS](https://www.youtube.com/watch?v=OJL-XEgzhYU)

This section allows you to configure your navigation menus, such as including new links.

![OJS dashboard view of Navigation Menu with user and primary menus and an option to add or edit navigation menu items.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-web-navmenu.png)

- **Navigation Menus**: Configure the User Menu and/or the Primary Menu.

Some menu item types will only be displayed under certain conditions. For example, the Login menu item type will link to your login page, but it will only appear in the menu when your website visitor is logged out. Similarly, the Logout menu item type will only appear when a website visitor is logged in.

When you assign a Menu Item with display conditions to a Menu, you will see an icon of an eye with a slash through it. You can click that icon to learn more about when it will be displayed or hidden.

- **Navigation Menu Items**: These are pre-programmed links you can add to the menu above, which point to pre-programmed parts of the website. You can rename any of these pages by clicking on _Edit_. For example, you can rename "Archives" as "Back Issues."

- **Navigation Menu Items: Add Item**: You can add new items to the menu. Click on _Add Item_ and choose from the drop-down menu. In addition to the pre-programmed links, you can also add an unlimited number of custom links. There are two types of custom links:

Custom Page: If you wish to add a new webpage to OJS to the Primary Menu (e.g., "Journal History"), select _Custom Page_ to create a static webpage. Title your new page, and choose a URL path, being careful to ensure that the path is unique. Custom pages can be used for additional content not otherwise available on your website. They must be updated manually, using the correponsponding _Edit_ button within the Navigation Menu Items list.

Remote URL: If you wish to add a link to an external website outside of OJS (e.g., "Our Society"), select _Remote URL_ and insert the full URL. It is good practice to periodically check the remote URL to ensure that it remains functional.

![Add item screen with item title and remote URL filled out.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-web-navmenu-add.png)

Once created, custom links will now appear in the list of Navigation Menu Items. Next, go to the desired Navigation Menu (e.g., Primary), use the blue arrow to reveal the options, and choose Edit. You can now drag and drop it from Unassigned Menu Items to Assigned Menu Items and into the appropriate location on the menu.

![Primary navigation area with a list of assigned and unassigned menu items.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-web-navmenu-add-nav.png)

Hit Save to record the change.

#### Announcements

This PKP School video explains how to configure the Announcements settings in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure announcements settings in OJS](https://www.youtube.com/watch?v=OmiDQGX4SGs)

This section allows you to create and display news announcements on the journal's website.

![OJS dashboard view of Announcements menu with an option to enable and display announcements.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-web-announce.png)

- **Announcements**: Check this off if you want to have announcements in your website
  - **Introduction**: Enter any general information you would like to appear on your announcements page.
  - **Display on Homepage**: Enter the number of announcements to be displayed on the homepage. If this is left blank, no announcements will be displayed.

Once the Announcements setting is enabled, click "Save." An "Announcements" menu item now appears in the main navigation on the left hand side. Click on this menu item and select "Add Announcement." Here you can include the title of the announcement, a short description and / or full text of the announcement, and an (optional) expiry date. 

If you wish to send an email notification to all users (who have not opted out of email notifications), select "Send notification email to all registered users." Note that this option only works when sending a new announcement. You can edit an announcement you made before, but no email will be sent at this stage if you select the "Send notification" option.

![OJS 3.3 Create the text for a new announcement.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-settings-website-new-announcement.png)

The announcement should now appear on an "Announcements" tab on the public-facing journal site.

![OJS 3.3 Announcements menu enabled in the sidebar with an option to add and edit announcements.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-settings-website-announcements.png)

This PKP School video explains how to configure the Website settings in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure website settings in OJS](https://www.youtube.com/watch?v=3vAR6lu-4DE)

#### Lists

Limit the number of items (for example, submissions, users, or editing assignments) to show in a list before showing subsequent items on another page. Also, limit the number of links to display to subsequent pages of the list.

#### Privacy Statement

Enter the privacy statement you want to appear on your site.

#### Date and Time

This option allows for the configuration of different format for dates and times for each journal and locale, which could previously only be set up in the 'config.inc.php' file. Note that the `config.inc.php` file can still be used to set the time and format across multiple journals, and the settings for the primary locale will be the default for other locales, unless otherwise configured.  A custom format can be entered using the [special format characters](https://www.php.net/manual/en/function.strftime.php#refsect1-function.strftime-parameters).

![OJS 3.3 Date and Time menu with an option to select long and short date formats.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-date-and-time-setup.png)

### Plugins {#plugins}

This PKP School video explains how to configure Plugins in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure plugins in OJS](https://www.youtube.com/watch?v=PMAsXY_tLMU)

Use this page to see all of the installed plugins and find new plugins.

To learn more about available plugins, see [the Plugin Inventory](https://docs.pkp.sfu.ca/plugin-inventory/en/).

#### Installed Plugins

All of the plugins listed here are available in your OJS installation. Check the Enable link to use them.

![OJS dashboard view of Plugins menu with the tab for installed plugins selected.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-web-plugins.png)

You will notice that some plugins are required for the system and cannot be disabled.

Click the blue arrow next to the plugin name to reveal links to Delete, Upgrade, or Configure settings for the plugin.

#### Plugin Gallery

The Plugin Gallery provides access to externally-created plugins, that may not be included in your OJS installation, but are available for download and activation. Only an Administrator user can install a new plugin.

![OJS dashboard view of Plugins menu with the tab for plugin gallery selected.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-web-plugins-gallery.png)

Selecting the plugin title will provide additional details, including the author, status, description, and compatibility.

![Hypothes.is plugin selected in the plugin gallery shows that it is installed and up-to-date.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-web-plugins-gallery-hypo.png)

#### External Plugins

Sometimes new plugins or plugins that are developed by folks outside of PKP will not appear in the Plugin Gallery and you need to install them separately.

1. Download the tar.gz file of the plugin from its repository under the Releases tab.
2. Go to Installed Plugins tab.
3. At top right, click Upload a New Plugin.
4. Upload the plugin file.
5. When it has finished uploading, click Save. Give it some time to install.

If upload fails you may get an error message that says, “The uploaded plugin archive does not contain a folder that corresponds to the plugin name.” Usually this means you have to change the name of the plugin folder inside the zipped folder to a more simple name. For example, change “translator-ojs-3_0_0-0” to “translator.”

Remember to hit Save to record the change.

#### Content Enhancement and Discovery Plugins

OJS 3 has a number of plugins that you can enable to help enhance the user experience and discoverability of your content and journal. This section will outline the different plugins available in OJS and how to configure and use them.

As some of the plugins below are 3rd party plugins, it may require that you download the zip file from GitHub and upload it to your journal. For general information on plugins and how to install and enable plugins, please see [Learning OJS 3 - Plugins](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-website#plugins).

Please note that as PKP does not maintain 3rd party plugins, we cannot guarantee that it will work with your version of OJS.

##### Browse Plugin

This plugin implements a block plugin that allows the user to navigate content by categories. The browse block appears on the journal's sidebar.

This plugin can be enabled from the Plugin Gallery.

![Browse plugin with categories for Summer, Fall, Spring, Winter.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-settings-plugin-browse.png)

##### Citation Style Language Plugin

The Citation Style Language plugin adds a “How to Cite” block to the article page that contains a citation for the article in the format of your choice, with an option below to generate the citation in another format.

![Example of a citation on an article page under How to Cite added by the Citation Style Language Plugin.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-settings-plugin-citation.png)

This is an Installed Plugin and will need to be enabled under Website Settings > Plugins > Installed Plugins.

To configure the plugin:

* Click the blue arrow next to the plugin name
* Click the **Settings** link that appears below.

![Citation Style Language Plugin settings button.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-settings-plugin-citation-2.png)

* Select the Primary citation format you would like to use from the first list, followed by the other citation formats you * would like to be available from the second list
* Next, you can optionally select a downloadable format to make available to readers to export to bibliography management software
* You can also add the location of your publication/publisher for citations that require it
* Click **OK** when you have finished configuring

Now the How to Cite block will appear on every article page in your journal.

*Please note: The citation style formats are generated by an external library. If you notice an error in a citation format you can file an issue in [the Citation Style Language styles repository on GitHub](https://github.com/citation-style-language/styles).*

*You can also add a custom citation style with custom coding.*

##### Custom Block Plugin

To configure and add custom blocks:

* Click Manage Custom Blocks below the plugin name
* From this screen, click Add Block to create a new block or click Edit or Delete under the block name to manage existing blocks.
* When adding a new block, enter a name for your block (required). In recent versions you can include spaces in the name and select whether or not the name  will appear above the block content.
* The display and order of blocks can be edited from the Sidebar Management section of Dashboard > Settings > Website > Appearance > Setup.

##### Custom Header Plugin

The Custom Header plugin can be used to add custom JavaScript to a header or block. JavaScript is often required to link your site with outside services but cannot be added directly to a field for security reasons.

The plugin can be installed from the Plugin Gallery.

##### Disqus plugin

The [Disqus plugin](https://github.com/ajnyga/disqus) integrates with [Disqus](https://disqus.com) and allows users to add comments to the article pages.

The Disqus plugin is a third-party plugin and must be installed from its Github repository.

After you install and enable the plugin, you must register for a Disqus account on the [Disqus website](https://disqus.com). When you register, choose the option to use Disqus on your website. Disqus offers free and paid plans and you must choose a plan when you register.

When asked to register your **Website Name**, create a name based on your journal name. This will show up in Disqus feeds, email notifications, and your Community tab. For example, "pkpworkshopsjournal."

Skip the **Install Disqus** step and go to **Configure Disqus**. Enter your journal url in the **Website URL** field. Enter your comments policy as applicable.

![Configure Disqus menu on the Disqus website.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-settings-plugin-disqus-configure-disqus.png)

Now you can configure the Disqus plugin on your journal site:

1. Go to Website Settings > Plugins
2. Find the Disqus plugin
3. Click the blue arrow next to the plugin name and **Settings** that will appear below
4. Enter the Website Name from your Disqus account in the **Disqus forum's shortname** field
5. Click **OK**

![OJS Disqus plugin settings menu with an option to enter a forum's shortname.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-settings-plugin-disqus-configure-plugin.png)

After configuring the plugin, if you open one of your article pages, you should see Disqus comments at the bottom. Your users will have to register with Disqus to use the feature.

![Example of an article page with Disqus comment field at the bottom.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-settings-plugin-disqus-comment-on-article.png)

##### Hypothes.is plugin

This plugin adds Hypothes.is integration to the public article view of OJS, permitting annotation and commenting. It currently supports commenting on HTML galleys.

This plugin can be enabled from the Plugin Gallery.

Once enabled, readers will see the hypothes.is tools on the right side of the HTML galley.

![Hypothesis view next to an HTML galley with sample text.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-settings-plugin-hypothesis.png)

You will need a free hypothes.is account in order to participate in public commenting. Specific/Private commenting groups can also be set up. [See hypothes.is](https://web.hypothes.is/help/how-to-create-a-private-group/) for instructions.

Public annotations and highlights will be visible (if any) once you are signed in.

![Hypothesis view next to an HTML galley with portions of the sample text highlighted.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-settings-plugin-hypothesis-2.png)

##### Keyword Cloud plugin

This plugin displays a tag cloud of keywords that can be enabled on the sidebar of your journal or press.

![Keyword cloud displayed in a journal sidebar.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-settings-plugin-keyword.png)

This is a 3rd party plugin that will need to be [downloaded from GitHub](https://github.com/lepidus/keywordCloud).

Once you’ve downloaded the file from GitHub, upload it to your journal and enable it. This will make the keyword cloud available as a block that you can add to the sidebar of your journal.

To add the keyword cloud display to your sidebar:

1. Go to Settings > Website > Appearance > Sidebar Management
2. Drag the Keyword Cloud block from the **Unselected** column to the **Sidebar column**
3. Rearrange the order of the blocks as needed
4. Click **Save**

The cloud will should now appear on the sidebar of your journal site.

##### Most Read Plugin

This plugin creates a “most read articles” section in the journal’s sidebar with the 5 most viewed articles (with links) in the last week, along with the number of views per article.

![Most read of the week list with article titles and links displayed in a journal sidebar.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-settings-plugin-most-read.png)

This is a 3rd party plugin and the file will need to be [downloaded from GitHub](https://github.com/ajnyga/mostRead).

Once you’ve downloaded the file from GitHub, upload it to your Journal and enable it. This will create a “Most Read” block that you can add to the sidebar of your journal.

To add the Most Read block to your sidebar:

1. Go to Settings > Website > Appearance > Sidebar Management
2. Drag the Most Read block from the **Unselected** column to the **Sidebar** column
3. Rearrange the order of the blocks as needed
4. Click **Save**

The block will now appear on the sidebar of your journal site.

##### Recommend Articles by Author Plugin

This plugin inserts a list of articles by the same author (with appropriate links) on an article’s abstract page.

![Most read articles by the same author(s) with a sample article and link.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-settings-plugin-author-rec.png)

This plugin can be enabled in the Plugin Gallery.

Once it has been enabled, there is no additional configuration required.

##### Recommend Similar Articles Plugin

This plugin inserts a list of similar articles to the article abstract page.

This plugin can be enabled in the Plugin Gallery.

Once it has been enabled, there is no additional configuration required.

##### Usage Statistics Plugin

This plugin displays the number of downloads of an article on the article page.

![Bar graph of article downloads displayed on an artilce page by the Usage Statistics plugin.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-settings-plugin-usage-stats.png)

To configure the Usage Statistics Plugin, you must be an **Administrator**:

1. Go to Settings > Website > Plugins.
2. Under Generic Plugins, find the Usage Statistics Plugin.
3. Click the blue arrow to the left of the plugin name to make links appear below the plugin.
4. Click Settings.
5. Scroll to the bottom of the pop-up box that opens to the section Statistics Display Options.
6. Check the box beside the Display submission statistics chart for the reader.
7. Below that you can select whether you would like to display the statistics as a bar or line graph and the maximum number of months to display usage for.
8. Click Save.

![Usage Statistics plugin settings with statistics display options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-settings-plugin-usage-stats-2.png)

Please note that:

* Usage statistics can only be displayed for the current year. The plugin is reset at the beginning of each year.
* The statistics being displayed indicate the number of times an article was downloaded.

> **Original chapter:** [Website Settings](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-website)

---

## Workflow Settings

The Workflow Settings allow you to configure various parts of the journal's editorial workflow. The workflow setting has 5 main tabs.

### Submission {#submission}

This PKP School video explains how to configure the submission process in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure the submission process in OJS](https://www.youtube.com/watch?v=_I2-IpEWu9E)

Use this section to configure the submission process.

#### Disable Submissions

A journal manager will be able to disable submissions for the entire section or disable submissions to a specific section or for the journal as a whole.

Once the setting is enabled, a notification is displayed indicating that submissions have been disabled. When this setting is enabled, users will no longer be able to make submissions in the journal.

![OJS 3.3 disable submission menu.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-workflow-disable-submissions.png)

![OJS 3.3 notice about the journal not accepting submissions.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-workflow-disable-submissions-notification.png)

#### Metadata

This section determines what types of metadata will be collected during the submission process, such as keywords and references.

#### Components

This PKP School video explains how to manage Components in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to manage components in OJS](https://www.youtube.com/watch?v=UkmvhHjP5V0)

Components are the file types authors may upload to the site. Typically, one file will be the article text, and others can include interview transcripts, data, images, etc. The components available for the author to choose from when making their submission are listed here.

![OJS 3.3 article components menu.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-settings-workflow-comp.png)

Using the links provided, you can change the **Order** of the components \(how they will be listed to the submitting author\), **Add a Component** \(if something you need is not included by default -- e.g., Video\), or **Restore the Defaults** \(if someone has made too many modifications and you just want to reset everything\).

##### Edit Component

You can also edit each component by selecting the blue arrow to the left of the component name. This will reveal an Edit link and a Delete link.

![OJS 3.3 component editing menu.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-settings-workflow-comp-edit.png)

- **Name**: This is the name of the component, as presented to the author.

- **File Type**: Choose how the files associated with this component will be treated and displayed. Anything that is marked as a Dependent file will not be published.

- **File Metadata**: Select the type of metadata that these files may receive. Document should be selected for the main publication files, such as the downloadable PDF, so that these files inherit their metadata from the publication. Otherwise, choose Supplementary Content for most file types. Artwork is appropriate for files which require distinct credit, caption and licensing metadata.

- **Key**: Optional short symbol for the component.

#### Checklist

In the Submission Preparation Checklist, Authors must check off that they agree with each item on this list. Use the _Order_ link to change the order of the items, use the _Add Item_ link to create a new item, and use the blue arrow to the left of the item name to _Edit_ an existing item.

![OJS 3.3 submission checklist editing menu.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-settings-workflow-settings-components-edit-item-edit.png)

#### Author Guidelines

Use this field to add information for your authors that will be useful during the submission process. This information will be displayed on the journal website.

- Author Guidelines: Recommended guidelines include required file types for the submission document, the preferred citation format, or any elements that should be present in the submission.
- Copyright Notice: This is the author copyright agreement between the author and the journal, and the author agrees to these terms at the time of submission.

### Review {#review}

This PKP School video demonstrates how to configure the Review process in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure the Review process in OJS](https://www.youtube.com/watch?v=1adbIbQM6E0)

This tab allows you to configure your journal's review process.

![OJS 3.3 review configuration editing menu.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-workflow-review.png)

#### Setup

**Default Review Mode**: Select whether your journal will follow an anonymous reviewer/anonymous author, anonymous reviewer/disclosed author, or open review process.

**Restrict File Access**:Check this off if you want the reviewer to respond to the request before accessing the submission files.

**One-click Reviewer Access**: Enable (default) the first option to provide reviewers with one-click access to the review, bypassing the need to go to the website, login, and find the submission. For security reasons with this option, editors are not able to modify email addresses or add CCs or BCCs prior to sending invitations to reviewers.

**Default Review Deadlines**: Indicate how long reviewers have to decide to accept or decline a review request from the editor, and how long they have to make a recommendation. These dates are calculated from the date the review is sent. 

**Automated Email Reminders**: Reviewers will automatically be notified when they are assigned to a review; however, you may wish to enable or disable reminder emails for reviewers. Use the drop down menu to select either the number of days or “Never Remind” under “Send a reminder if a reviewer has not responded to a review request within the following time (days) after response due date” to set the number of days that can pass after the due date before reviewers will be reminded to accept or reject a review request.

Use the drop down menu to select either the number of days or “Never Remind” under “Send a reminder if a reviewer has not responded to a review request within the following time (days) after response due date” to set the number of days that can pass after the due date before reviewers will be reminded to make a recommendation for a submission.

Hit the **Save** button to record your changes.

![OJS 3.3 notification of author submission screen.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-review-reminders.png)

Note that some system settings must be configured by the Site Administrator to send email. See the [Administrator's Guide](https://docs.pkp.sfu.ca/admin-guide/en/email) for more information.

#### Review Guidance

**Review Guidelines**: Provide your reviewers with criteria for judging a submission's suitability for publication in the press, which may include instructions for preparing an effective and helpful review.

**Competing Interests**: Add your competing interest disclosure policy statement here.

#### Review Forms

Review forms provide reviewers with a set of questions to respond to. This can help focus their feedback in ways that is more useful to you.

**Create Review Form**: Use the Create Review Form link to make a new form.

![OJS 3.3 new review form creation menu.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-settings-workflow-settings-review-create.png)

The Description and Instructions provide information about the form and when to use it for Journal Managers and Editors. This content is not included on the form that reviewers see. You can add instructions and guidelines for reviewers under Review Guidelines \(below\).

Back at the Review Forms page, select the blue arrow to the left of the form name to reveal the Edit link.

![OJS 3.3 review forms with edit menu expanded.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-settings-workflow-settings-review-edit1.png)

Select the Edit link and complete the form.

![OJS 3.3 review form edit menu and response options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-settings-workflow-settings-review-create-items.png)

**Form Items** are form questions.

You can choose whether to make the question mandatory for reviewers and visible to the author.

You can then choose the type of response, including:

* a single word text box
* a single line text box
* an extended text box \(for longer answers\)
* checkboxes \(where the reviewer can select multiple possible responses\)
* radio buttons \(where the reviewer can only select one possible answer\)
* dropdown menu \(also where reviewers can only select one possible answer\)

**Response Options** are the selections you make available for the checkboxes, radio buttons, or dropdown menus. A good example of a checkbox response is a [Likert scale](https://en.wikipedia.org/wiki/Likert_scale), where the reviewer must choose only one option: E.g., Good, Neutral, Bad.

Remember to hit the **Save** button to record your changes.

Use the **Preview** tab to test out the form.

![OJS 3.3 review form preview and response options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-settings-workflow-settings-review-preview.png)

Once you send the form to a reviewer you will no longer be able to edit it because that would change the record for existing reviews using that form. If you want to make changes to the review form at that point you can copy the existing form and create a new updated version.

**Anonymous Reviewer/Disclosed Author**: Check this box to display a link for instructions on ensuring all submission files are anonymized.

![OJS 3.3 checkbox to display submission anonymization instructions.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-settings-workflow-settings-review2.png)

### Publisher Library {#publisher-library}

This PKP School video explains how to use the Publisher Library in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of the Publisher Library in OJS](https://www.youtube.com/watch?v=QhOJjxW0_Rw)

The Journal Manager and Editors may upload documents that they would like to share with the other users in the Publisher Library. Any document added in this area will be visible within a user’s Document Library in their manuscript’s Submission Library.

You can also upload a file here that you would like to be publicly accessible via a URL, which you can link to from other parts of your site, including the author guidelines, submission checklist, or a static page.

Suggested forms that can be uploaded in this area can include the galley approval form, supplemental material cover page, and other forms related to your journals workflow.

![OJS 3.3 publisher library menu.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-workflow-publib1.png)

To add a file here, click ‘Add a file’ on the top right corner of the Publisher Library box.

![OJS 3.3 add a file to the publisher library.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-workflow-publib2.png)

**Name**: Title of Document you want to appear to the user

**Type**: Select Marketing, Permission, Reports, Other

**Public Access**: Enabling this will allow users to download this file using the hyperlink provided if it is hyperlinked in other parts of your journal site.

### Emails {#emails}

This PKP School video explains how to configure emails in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure emails in OJS](https://www.youtube.com/watch?v=ZK-Nb7wfHew)

#### Email Setup

The section allows you to configure the emails that are sent out from the system.

![OJS 3.3 emails menu.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-workflow-emails.png)

**Signature**: The information in this field will be added to the bottom of every email sent out by the system.

**Bounce Address**: A notice will be sent to this email address of any system-sent emails that fail to deliver, such as when the targeted email address is no longer valid.

#### Email Templates

OJS facilitates work flow communication through the use of prepared email messages. Please note, some configuration is required to send email. See the [Administrator's Guide](https://docs.pkp.sfu.ca/admin-guide/en/email) for more information.

You can view and modify the prepared email templates here. You will see a list of email templates under the Emails tab. The title and summary of each email template is displayed in the list.

![OJS 3.3 emails templates.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-settings-workflow-email-templates.png)

If you click the arrow beside each email template you can view the message subject and contents and who is the default sender and recipient of the message.

![OJS 3.3 editorial assignment template editing screen.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-settings-workflow-email-template-view.png)

You can search for an email template by keyword by typing something in to the **Search** box.

You can click **Filters** to reveal options to filter the templates by status, sent from, sent to, and which workflow stage it is used during. These filters can help you find templates you want to edit.

![OJS 3.3 email template filtering options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-settings-workflow-email-template-filters.png)

See [Template Descriptions](#template-descriptions) at the end of this chapter for a table of all email templates and their sender, recipient, and workflow stage.

##### Edit email templates

When you edit an email template, you change what it will say every time it is used.  For emails that are sent voluntarily, such as a message sent to a reviewer asking them to review a submission, you can also change the contents of the message at the time of sending it. This changes the contents for that message only.

To edit a template:

1. Go to Workflow Settings > Emails > Prepared Email Templates
2. Click the blue arrow next to the template name to reveal links below it
3. Click Edit
4. Make changes to the subject and the body text. Be careful to not delete any tags such as “{$authorName}:,” which automatically insert content from a submission.
5. When you’re finished editing, click Save.

##### Disable email templates

All of the templates are enabled by default when you install OJS, but you can disable some templates by clicking the Disable button. Most of the templates that can be disabled are messages that are sent automatically by OJS. Disabling the template will mean that the automatic notification will not be sent.

To disable a template:

1. Go to Workflow Settings > Emails > Prepared Email Templates
2. Click the blue arrow next to the template name to reveal links below it
3. Click Disable (if the button does not appear, then this template can't be disabled)

##### Reload default email templates

If you have edited email templates but want to reverse the edits and restore them to their default contents, you can reset them:

1. Go to Workflow Settings > Emails > Prepared Email Templates
2. Click Reset All Templates
3. When the confirmation message appears, click OK.

##### Add email template

Click the button **Add Email Template** to create a custom email template that you can use when notifying a user or adding a participant to a submission. Note that in versions earlier than OJS 3.1.2, you can create a custom email templates but it will not be available to use at any stage in the workflow.

##### Filters

Click here to filter email templates based on the following: Enabled, Disabled, Custom Template. You can also filter email templates based on who it was sent from and who it is sent to.

##### Add email attachment

There is no direct email attachment option in OJS 3, but you can upload and share public files via the Publisher Library:

1. In Settings > Workflow > Publisher Library > Add a file, upload your document and tick the “Public Access” checkbox
2. Click "OK" for the URL to be generated
3. Insert the URL in your email

You can also choose to modify an existing email template with this URL, or share it publicly on the website.

##### Template descriptions

OJS 3.2 now provides a description for every template outlining the sender and recipient, stage of workflow.

The table below provides an overview of the prepared email templates found in OJS 3.2. Note that "Editor" refers to any type of editor (e.g. journal editor, production editor, etc.). The following columns appear in the table:

- **Template**: The name of the email template.
- **Description**: A description of the template.
- **Sender**: The name or signature that will appear at the end of the message. In some cases, the system sends the message automatically but the sender appears as a particular user.
- **Recipient**: Who the email can be sent to.
- **Workflow** stage: The workflow stage that this template is used in.

| Template                           | Description                                                                                                                                                                                                                                                                                                                                                                                                                          | Sender                             | Recipient             | Workflow                 |
|------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------|-----------------------|--------------------------|
| Announcement - ANNOUNCEMENT       | This email is used to notify users of a new announcement posted by the journal.                                                                                                                                                                                                                                                                                                                                       | System                         | Registered Users                |               |
| Citation Editing - CITATION_EDITOR_AUTHOR_QUERY       | This email allows copyeditors to request additional information about references from authors.                                                                                                                                                                                                                                                                                                                                       | Copyeditor                         | Author                | Copyediting              |
| Copyediting Request - COPYEDIT_REQUEST                   | This email is sent by a Section Editor to a submission's Copyeditor to request that they begin the copyediting process. It provides information about the submission and how to access it.                                                                                                                                                                                                                                           | Section Editor                     | Copyeditor            | Copyediting              |
| Editorial Assignment - EDITOR_ASSIGN                      | This email notifies a Section Editor that the Editor has assigned them the task of overseeing a submission through the editing process. It provides information about the submission and how to access the journal site.                                                                                                                                                                                                             | Editor                             | Section Editor        | Submission               |
| Editor Decision - EDITOR_DECISION_ACCEPT             | This email from the Editor or Section Editor to an Author notifies them of a final "accept submission" decision regarding their submission.                                                                                                                                                                                                                                                                                          | Editor/Section Editor              | Author                | Review                   |
| Editor Decision - EDITOR_DECISION_DECLINE            | This email from the Editor or Section Editor to an Author notifies them of a final "decline" decision regarding their submission.                                                                                                                                                                                                                                                                                                    | Editor/Section Editor              | Author                | Review                   |
| Editor Decision - EDITOR_DECISION_INITIAL_DECLINE    | This email is send to the author if the editor declines his submission initially, before the review stage                                                                                                                                                                                                                                                                                                                            | Editor/Section Editor              | Author                | Submission               |
| Editor Decision - EDITOR_DECISION_RESUBMIT           | This email from the Editor or Section Editor to an Author notifies them of a final "resubmit" decision regarding their submission.                                                                                                                                                                                                                                                                                                   | Editor/Section Editor              | Author                | Review                   |
| Editor Decision - EDITOR_DECISION_REVISIONS          | This email from the Editor or Section Editor to an Author notifies them of a final "revisions required" decision regarding their submission.                                                                                                                                                                                                                                                                                         | Editor/Section Editor              | Author                | Review                   |
| Editor Decision - EDITOR_DECISION_SEND_TO_EXTERNAL   | This email from the Editor or Section Editor to an Author notifies them that their submission is being sent to an external review.                                                                                                                                                                                                                                                                                                   | Editor/Section Editor              | Author                | Review                   |
| Editor Decision - EDITOR_DECISION_SEND_TO_PRODUCTION | This email from the Editor or Section Editor to an Author notifies them that their submission is being sent to production.                                                                                                                                                                                                                                                                                                           | Editor/Section Editor              | Author                | Production               |
| Editor Recommendation - EDITOR_RECOMMENDATION              | This email from the recommending Editor or Section Editor to the decision making Editors or Section Editors notifies them of a final recommendation regarding the submission.                                                                                                                                                                                                                                                        | Recommending Editor/Section Editor | Editor/Section Editor | Review                   |
| Article of Possible Interest - EMAIL_LINK                         | This email template provides a registered reader with the opportunity to send information about an article to somebody who may be interested. It is available via the Reading Tools and must be enabled by the Journal Manager in the Reading Tools Administration page.                                                                                                                                                             | Journal Manager                    | Reader                |                          |
| Galleys Complete - LAYOUT_COMPLETE                    | This email from the Layout Editor to the Section Editor notifies them that the layout process has been completed.                                                                                                                                                                                                                                                                                                                    | Layout Editor                      | Editor                | Production               |
| Request Galleys - LAYOUT_REQUEST                     | This email from the Section Editor to the Layout Editor notifies them that they have been assigned the task of performing layout editing on a submission. It provides information about the submission and how to access it.                                                                                                                                                                                                         | Editor                             | Layout Editor         | Production               |
| Archiving Request for {$contextName} - LOCKSS_EXISTING_ARCHIVE            | This email requests the keeper of a LOCKSS archive to consider including this journal in their archive. It provides the URL to the journal's LOCKSS Publisher Manifest.                                                                                                                                                                                                                                                              | LOCKSS                             | Journal Manager       | Post-Production/Indexing |
| Archiving Request for {$contextName} - LOCKSS_NEW_ARCHIVE                 | This email encourages the recipient to participate in the LOCKSS initiative and include this journal in the archive. It provides information about the LOCKSS initiative and ways to become involved.                                                                                                                                                                                                                                | LOCKSS                             | Journal Manager       | Post-Production/Indexing |
| Article Indexing Error - LUCENE_ARTICLE_INDEXING_ERROR_NOTIFICATION                 | This email template is used to notify the technical contact of a journal that an error occurred during article indexing.                                                                                                                                                                                                                                | Lucene search plugin                             | Journal Manager       | Post-Production/Indexing |
| Journal Indexing Error - LUCENE_JOURNAL_INDEXING_ERROR_NOTIFICATION                 | This email template is used to notify the technical contact of a journal that an error occurred during journal indexing.                                                                                                                                                                                                                                | Lucene search plugin                             | Journal Manager       | Post-Production/Indexing |
| Journal Search Service Error - LUCENE_SEARCH_SERVICE_ERROR_NOTIFICATION                 | This email template is used to notify the technical contact of a journal that an error occurred while trying to access the Solr search                                                                                                                                                                                                                                | Lucene search plugin                             | Journal Manager       | Post-Production/Indexing |
| Manual Payment Notification - MANUAL_PAYMENT_NOTIFICATION        | This email template is used to notify a journal manager contact that a manual payment was requested.                                                                                                                                                                                                                                                                                                                                 | Author                             | Journals Manager      |                          |
| New notification from {$siteTitle} - NOTIFICATION                       | The email is sent to registered users that have selected to have this type of notification emailed to them. This includes notifications of announcements and new issues published.                                                                                                                                                                                                                                                                                                                         | System                             | Registered User       |                          |
| A message regarding {$contextName} - NOTIFICATION_CENTER_DEFAULT        | The default (blank) message used in the Notification Center Message Listbuilder.                                                                                                                                                                                                                                                                                                                                                     |                                    |                       |                          |
| Welcome to the the {$siteTitle} mailing list! - NOTIFICATION_MAILLIST_WELCOME                       | This email is sent to an unregistered user who just registered with the notification mailing list.                                                                                                                                                                                                                                                                                                                          | System                             | Registered User       |                         
| Issue Now Open Access - OPEN_ACCESS_NOTIFY                 | This email is sent to registered readers who have requested to receive a notification email when an issue becomes open access.                                                                                                                                                                                                                                                                                                       | Registered Reviewer                | System                | Publish                  |
| Submission ORCID - ORCID_COLLECT_AUTHOR_ID            | This email template is used to collect the ORCID id's from authors.                                                                                                                                                                                                                                                                                                                                                                  | Journals Manager/System            | Author                | Submission               |
| Requesting ORCID record access - ORCID_REQUEST_AUTHOR_AUTHORIZATION | This email template is used to request ORCID record access from authors.                                                                                                                                                                                                                                                                                                                                                             | Journals Manager/System            | Author                | Submission               |
| Password Reset - PASSWORD_RESET                     | This email is sent to a registered user when they have successfully reset their password following the process described in the PASSWORD_RESET_CONFIRM email.                                                                                                                                                                                                                                                                        | System                             | Registered User       |                          |
| Password Reset Confirmation - PASSWORD_RESET_CONFIRM             | This email is sent to a registered user when they indicate that they have forgotten their password or are unable to login. It provides a URL they can follow to reset their password.                                                                                                                                                                                                                                                | System                             | Registered User       |                          |
| New Issue Published - PUBLISH_NOTIFY                | This email is not yet used in OJS 3.                                                                                                                                                                                                                                          | System                             | Registered Users      | Publish                  |
| Registration as Reviewer with {$contextName} - REVIEWER_REGISTER                  | This email is sent to a newly registered reviewer to welcome them to the system and provide them with a record of their username and password.                                                                                                                                                                                                                                                                                       | System                             | Reviewer              |                          |
| Article Review Acknowledgement - REVIEW_ACK                         | This email is sent by a Section Editor to confirm receipt of a completed review and thank the reviewer for their contributions.                                                                                                                                                                                                                                                                                                      | Section Editor/Editor              | Reviewer              | Review                   |
| Request for Review Cancelled - REVIEW_CANCEL                      | This email is sent by the Section Editor to a Reviewer who has a submission review in progress to notify them that the review has been cancelled.                                                                                                                                                                                                                                                                                    | Reviewer                           | Editor/Section Editor | Review                   |
| Able to Review - REVIEW_CONFIRM                     | This email is sent by a Reviewer to the Section Editor in response to a review request to notify the Section Editor that the review request has been accepted and will be completed by the specified date.                                                                                                                                                                                                                           | Reviewer                           | Editor/Section Editor | Review                   |
| Unable to Review - REVIEW_DECLINE                     | This email is sent by a Reviewer to the Section Editor in response to a review request to notify the Section Editor that the review request has been declined.                                                                                                                                                                                                                                                                       | Reviewer                           | Editor/Section Editor | Review                   |
| REVIEW_REINSTATE                   | This email is sent by the Section Editor to a Reviewer who has a submission review in progress to notify them that a cancelled review has been reinstated.                                                                                                                                                                                                                                                                           | Editor/Section Editor              | Reviewer              | Review                   |
| Submission Review Reminder - REVIEW_REMIND                      | This email is sent by a Section Editor to remind a reviewer that their review is due.                                                                                                                                                                                                                                                                                                                                                | Editor/Section Editor              | Reviewer              | Review                   |
| Automated Submission Review Reminder - REVIEW_REMIND_AUTO                 | This email is automatically sent when a reviewer's due date elapses (see Review Options under Settings > Workflow > Review) and one-click reviewer access is disabled. Scheduled tasks must be enabled and configured (see the site configuration file).                                                                                                                                                                             | System                             | Reviewer              | Review                   |
| Automated Submission Review Reminder - REVIEW_REMIND_AUTO_ONECLICK        | This email is automatically sent when a reviewer's due date elapses (see Review Options under Settings > Workflow > Review) and one-click reviewer access is enabled. Scheduled tasks must be enabled and configured (see the site configuration file).                                                                                                                                                                              | System                             | Reviewer              | Review                   |
| Submission Review Reminder - REVIEW_REMIND_ONECLICK             | This email is sent by a Section Editor to remind a reviewer that their review is due.                                                                                                                                                                                                                                                                                                                                                | Editor/Section Editor              | Reviewer              | Review                   |
| Article Review Request - REVIEW_REQUEST                     | This email from the Section Editor to a Reviewer requests that the reviewer accept or decline the task of reviewing a submission. It provides information about the submission such as the title and abstract, a review due date, and how to access the submission itself. This message is used when the Standard Review Process is selected in Management > Settings > Workflow > Review. (Otherwise see REVIEW_REQUEST_ATTACHED.)  | Editor/Section Editor              | Reviewer              | Review                   |
| Article Review Request - REVIEW_REQUEST_ATTACHED            | This email is sent by the Section Editor to a Reviewer to request that they accept or decline the task of reviewing a submission. It includes the submission as an attachment. This message is used when the Email-Attachment Review Process is selected in Management > Settings > Workflow > Review. (Otherwise see REVIEW_REQUEST.)                                                                                               | Editor/Section Editor              | Reviewer              | Review                   |
| Article Review Request - REVIEW_REQUEST_ATTACHED_SUBSEQUENT | This email is sent by the Section Editor to a Reviewer to request that they accept or decline the task of reviewing a submission for a second or greater round of review. It includes the submission as an attachment. This message is used when the Email-Attachment Review Process is selected in Management > Settings > Workflow > Review. (Otherwise see REVIEW_REQUEST_SUBSEQUENT.)                                            | Editor/Section Editor              | Reviewer              | Review                   |
| Article Review Request - REVIEW_REQUEST_ONECLICK            | This email from the Section Editor to a Reviewer requests that the reviewer accept or decline the task of reviewing a submission. It provides information about the submission such as the title and abstract, a review due date, and how to access the submission itself. This message is used when the Standard Review Process is selected in Management > Settings > Workflow > Review, and one-click reviewer access is enabled. | Editor/Section Editor              | Reviewer              |                          |
| Article Review Request - REVIEW_REQUEST_ONECLICK_SUBSEQUENT | This email from the Section Editor to a Reviewer requests that the reviewer accept or decline the task of reviewing a submission for a second or greater round of review. It provides information about the submission such as the title and abstract, a review due date, and how to access the submission itself. This message is used when the Standard Review Process is selected in Management > Settings > Workflow > Review, and one-click reviewer access is enabled.                                                                                                                                                                                                                                                                                                                                                                                                                                 | Editor/Section Editor                                    | Reviewer                      | Review                         |
| Article Review Request - REVIEW_REQUEST_REMIND_AUTO                                    | This email is automatically sent when a reviewer's confirmation due date elapses (see Review Options under Settings > Workflow > Review) and one-click reviewer access is disabled. Scheduled tasks must be enabled and configured (see the site configuration file).                                                                                                                                                                                                                                                                                                                                                                                                                                 | System                                   |  Reviewer                        | Review                           |
| Article Review Request - REVIEW_REQUEST_REMIND_AUTO_ONECLICK                                   | This email is automatically sent when a reviewer's confirmation due date elapses (see Review Options under Settings > Workflow > Review) and one-click reviewer access is enabled. Scheduled tasks must be enabled and configured (see the site configuration file).                                                                                                                                                                                                                                                                                                                                                                                                                                    | System                                   |  Reviewer                     | Review                         |
| Article Review Request - REVIEW_REQUEST_SUBSEQUENT                                   | This email from the Section Editor to a Reviewer requests that the reviewer accept or decline the task of reviewing a submission for a second or greater round of review. It provides information about the submission such as the title and abstract, a review due date, and how to access the submission itself. This message is used when the Standard Review Process is selected in Management > Settings > Workflow > Review. (Otherwise see REVIEW_REQUEST_ATTACHED_SUBSEQUENT.)                                                                                                                                                                                                                                                                                                                                                                                                                                     |  Editor/Section Editor                                  | Reviewer                       | Review                         |
| Revised Version Uploaded - REVISED_VERSION_NOTIFY                                   | This email is automatically sent to the assigned editor when author uploads a revised version of an article.                                                                                                                                                                                                                                                                                                                                                                                                                                     | System                                   | Editor/Section Editor                      | Review                         |
| STATISTICS_REPORT_NOTIFICATION                                   | This email is automatically sent monthly to editors and journal managers to provide them a system health overview.                                                                                                                                                                                                                                                                                                                                                                                                                                     | System                                   | Editor/Journals Manager                      |                          |
| Submission Acknowledgement - SUBMISSION_ACK                                   | This email, when enabled, is automatically sent to an author when he or she completes the process of submitting a manuscript to the journal. It provides information about tracking the submission through the process and thanks the author for the submission.                                                                                                                                                                                                                                                                                                                                                                                                                                     | System                                   | Author                      | Submission                         | 		 
| Submission Acknowledgement - SUBMISSION_ACK_NOT_USER                                   | This email, when enabled, is automatically sent to the other authors who are not users within OJS specified during the submission process.                                                                                                                                                                                                                                                                                                                                                                                                                                     | System                                  | Author (not registered in OJS)                      | Submission          |   
| Submission Unsuitable - SUBMISSION_UNSUITABLE                                   | This email sends a message to an author who makes an unsuitable submission to the journal and recommends they submit elsewhere.                                                                                                                                                                                                                                                                                                                                                                                                                                     | Editor                                  | Author                      | Submission          |   
| Subscription Expired - SUBSCRIPTION_AFTER_EXPIRY |  This email notifies a subscriber that their subscription has expired. It provides the journal's URL along with instructions for access.       | System         | Subscriber |  |                                                                                                                                                                                                                                                                                                                                                                                         
| Subscription Expired - Final Reminder - SUBSCRIPTION_AFTER_EXPIRY_LAST | This email notifies a subscriber that their subscription has expired. It provides the journal's URL along with instructions for access.                                   | System | Subscriber |				 |                                                                                                                                                                                                                                                                                                                                                                                                                                       
| Notice of Subscription Expiry - SUBSCRIPTION_BEFORE_EXPIRY                          | This email notifies a subscriber that their subscription will soon expire. It provides the journal's URL along with instructions for access.                              | System      | Subscriber |    |                                                                                                                                                                                                                                                                                                                                                                                                                                   
| Subscription Notification - SUBSCRIPTION_NOTIFY                         | This email notifies a registered reader that the Manager has created a subscription for them. It provides the journal's URL along with instructions for access.   | System                                  | Subscriber                      |                          |
| Subscription Purchase: Individual - SUBSCRIPTION_PURCHASE_INDL                                   | This email notifies the Subscription Manager that an individual subscription has been purchased online. It provides summary information about the subscription and a quick access link to the purchased subscription.                                                                                                                                                                                                                                                                                                                                                                                                                                      | System                                 | Subscription Manager                      |                          |
| Subscription Purchase: Institutional - SUBSCRIPTION_PURCHASE_INSTL                                   | This email notifies the Subscription Manager that an institutional subscription has been purchased online. It provides summary information about the subscription and a quick access link to the purchased subscription.                                                                                                                                                                                                                                                                                                                                                                                                                                     | System                                   | Subscription Manager                       |                          |
|Subscription Renewal: Individual - SUBSCRIPTION_RENEW_INDL| This email notifies the Subscription Manager that an individual subscription has been renewed online. It provides summary information about the subscription and a quick access link to the renewed subscription.|System| Subscription Manager |   |
| Subscription Renewal: Institutional - SUBSCRIPTION_RENEW_INSTL                                   | This email notifies the Subscription Manager that an institutional subscription has been renewed online. It provides summary information about the subscription and a quick access link to the renewed subscription.                                                                                                                                                                                                                                                                                                                                                                                                                                     | System                                   | Subscription Manager                      |                          |
| Journal Registration - USER_REGISTER                                   | This email is sent to a newly registered user to welcome them to the system and provide them with a record of their username and password.                                                                                                                                                                                                                                                                                                                                                                                                                                     | System                                   | User                      |                          |
| Validate Your Account - USER_VALIDATE                                   | This email is sent to a newly registered user to validate their email account.                                                                                                                                                                                                                                                                                                                                                                                                                                     | System                                   | User                      |                          |

> **Original chapter:** [Workflow Settings](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-workflow)

---

## Distribution Settings

The Distribution Settings focus on access to and visibility of your journal. The tabs consist of License, Search Indexing, Payments, Access, and Archiving.

Please note that if your journal is multilingual and you have Forms enabled for multiple languages in the language settings, you will have to configure some of this information for each language. You can switch to another languages by selecting the language under the Help link on the top right.

### License {#license}

This PKP School video explains how to configure copyright and licensing terms in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure copyright and licensing terms in OJS](https://www.youtube.com/watch?v=qfzvbN4a-bM)

In this section you can configure copyright and licensing terms for your journal's content.

![Distribution settings license tab showing copyright holder, license and copyright year options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-settings-dist-permissions.png)

**Copyright Holder**: Select who holds copyright to the articles published by your journal. The trend in open access publishing is to allow authors to retain copyright of their work.

**License**: Select the license for your journal. CC Attribution 4.0 is a widely used license for open access journals, allowing for maximum sharing and reuse. For definitions of different Creative Commons licenses, see the [Creative Commons website](https://creativecommons.org/).

The license you select will be automatically added to each article's metadata and displayed on the article page of each published article.

**Copyright Year**: Select whether you want the copyright year to come by default from the article's publication date or the issue's publication date.

If you use a continuous publishing model, select the article's publication date. If you use a traditional, issue-based publishing model, select the issue's publication date.

This default can be overridden on a case-by-case basis.

**License Terms**: Enter any additional license terms you would like to display alongside the license selected above on the published article page.

### Search Indexing {#search-indexing}

This PKP School video explains how to enhance search indexing in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to enhance search indexing in OJS](https://www.youtube.com/watch?v=qf_5sTlDXM0)

This section helps you enhance your search engine optimization and make your content more discoverable.

![Distribution settings search indexing tab showing description and custom tags options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-settings-dist-index.png)

Use **Description** to provide a brief description of your journal for search engines.

Use **Custom Tags** to add custom HTML header tags to the header of every page of your journal, which can help your site get indexed by search engines. Tags need to be added as HTML elements. If you simply enter words they will appear at the top of every page of your site instead of in the site's metadata. Here is an example of text that could be entered in this field:

```html
<meta name="description" content="The Journal of Public Knowledge. Publication of the Public Knowledge Project - PKP and Simon Fraser University - SFU" />
<meta name="keywords" content="open access, scholarly publishing, open source software, non-profit organizations, scholarly journals, free software" />
<meta name="author" content="metatags generator">
<meta name="robots" content="index, follow">
<meta name="revisit-after" content="3 month">
```

### Payments {#payments}

This PKP School video explains how to configure the Payments settings in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure payments in OJS](https://www.youtube.com/watch?v=9r0mRqtNVuU)

OJS provides the ability to collect online payments and manage subscriptions and author fee payments.

Using the PayPal plugin, you can accept payments through PayPal, or you can accept manual payments (such as cheque, email transfer, etc.), but they must be made outside of OJS and are not automatically recorded in OJS.  If you would like to use a different payment service you will have to create your own plugin.

#### Enable Payments

To use payments and subscriptions features, you first have to enable payments under this tab. After you check off **Enable**, additional configuration settings will appear below.

![Distribution settings payments tab showing enable payments, currency and payment plugins options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-settings-dist-pay.png)

Select the currency you will use.

Select the fee payment method you will use under **Payment Plugins**.

If you select **PayPal Fee Payment**, additional fields will appear.

To accept PayPal payments, you will need to go to Website Settings > Plugins and enable the PayPal Plugin, then do additional setup and configuration explained in the [PayPal Plugin Guide](https://docs.pkp.sfu.ca/using-paypal-for-ojs-and-ocs/en/). Through this process you will get the values for the **Account Name**, **Client ID**, and **Secret** fields.

![Paypal fee payment screen showing test mode enable option, account name, client ID and secret fields.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-settings-dist-paypalsettings.png)

If you select **Manual Fee Payment** under **Payment Plugins**, a field will appear where you can enter instructions that will appear to users who are making a manual payment.  For example, “Send a cheque payable to the Public Knowledge Project” to ______.”

![Manual fee payment screen showing manual payment instructions field.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-settings-manual-payments.png)

You will also need to enable the Manual Payment Plugin under Website Settings > Plugins to accept manual payments.

Click **Save**.

A new menu item will appear on the main dashboard menu called **Payments**.

Go to the [Subscriptions Chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/subscriptions) for further instructions on managing subscriptions and payments.

If you plan to make your journal or articles available by subscription, go to Distribution Settings > Access and check off “The journal will require subscriptions to access some or all of its contents.”

![Distribution settings access tab showing publishing mode options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-settings-dist-access.png)

#### Donations

In OJS 3.x there is not an option to set up a payment type for donations, to manage donations with the Payments module, or to use the PayPal plugin to accept donations. You can add the Donations block to your sidebar, but it will have to link to an external site where donation payments can be made.

### Access {#access}

This PKP School video explains how to configure the Access settings in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure access settings in OJS](https://www.youtube.com/watch?v=RlKVwF3h_PM)

Under the Access tab you can configure whether you want your journal contents to be open access, available by subscription, or a combination. By default, the open access option is selected. However, if you wish to use OJS for a subscription journal, choose the second option (see above section on Payments for further information). Selecting the second option will allow you to further delay open access by different periods of time.

![Distribution settings access tab showing publishing mode and delayed open access options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-settings-dist-access-delayed.png)

If you are only using OJS to manage your submission workflow and not publish your content, you can select "OJS will not be used to publish the journal's contents online."

OJS allows you to configure how and when content can be accessed at an article and issue level. When you create an issue, there is a tab called **Access** under which you can set the **Access Status** as **Subscription** or **Open Access**.

![Issue settings access tab showing subscription and open access options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-issue-access.png)

If you set it as **Subscription**, underneath that a box will appear where you can optionally enter an **Open Access Date**, at which the content will become open access.

Once you set it as **Subscription**, on the **Table of Contents** tab, a checkbox will appear beside each article under **Open Access**, where you can optionally set individual articles as open access, even if the rest of the issue remains available by subscription.

![Issue table of contents showing open access checkboxes.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-OJS3.2-article-access.png)

**Enable OAI** will be enabled by default, as this is an important protocol used by indexing services and other applications to harvest your journal's metadata. However, if you are not using OJS to publish your journal's content you may want to disable OAI.

![Enable OAI screen with enable and disable options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-settings-dist-oai.png)

### Archiving {#archiving}

This PKP School video explains how to enable archiving in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to enable archiving in OJS](https://www.youtube.com/watch?v=ohHaj-MSLNA)

If you are a member of a LOCKSS or CLOCKSS network, use this tab to activate your journal. The PKP PN Plugin, which deposits your content in the PKP Preservation Network (PN), is available for OJS 3.1.2 or newer.

For instructions on enabling the PKP PN, see the [PKP Preservation Network Guide](https://docs.pkp.sfu.ca/pkp-pn/en/).

If you use another network, enabling it here will make your content available to the network, but you will also need to contact the network to make it aware of your journal.

![Distribution settings acrhiving tab showing LOCKSS and CLOCKSS options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-settings-web-archive.png)

> **Original chapter:** [Distribution Settings](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-distribution)

---

## Users and Roles

This section provides information on accessing all of user accounts associated with your journal, as well as managing roles and permissions.

### Managing Users {#managing-users}

This PKP School video explains how to manage users in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to manage users in OJS](https://www.youtube.com/watch?v=_AAtxnFEodQ)

In addition to managing the journal web site, the Journal Manager is also responsible for all of the user accounts in the system.

To view the user accounts, select Users & Roles from the left menu.

![Users and Roles screen with list of journal users](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-users.png)

If you want to export a list of all registered users, you can find the option to export it as an XML file under the **Tools** menu. If you prefer your user data in a spreadsheet format, you can download it as a CSV file from **Statistics > Users**.

#### Users

Users are displayed in last name order.

You can edit a user account by selecting the blue arrow to the left of an entry.

![Blue arrow selected by a user's name with options to edit their account](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-users-edit.png)

This opens the options to Email, Edit User, Disable, Remove, Login As, Merge User.

##### Email Users

If you want to email a user about a particular submission, you can use the Discussion feature in the submission. This keeps all communication about a submission in one place.

To send an email to a user that is unrelated to a submission:

1. In the Journal Manager or Editor’s dashboard, go to Users & Roles > Users
2. Find the user you want to email
3. Click the blue arrow next to the user’s name to reveal links below it
4. Click Email. A pop-up box will appear where you can type in your message and send it

![Email pop-up box for emailing a user](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-users-email.png)

###### Bulk Email Notifications by Role

In OJS 3.3 you can email multiple users at the same time using the Notify tab. This feature will need to be enabled for each journal by the journal administrator under Site Settings > Bulk Emails. The site administrator can also disable certain roles in the journal from receiving bulk emails under Hosted Journals > Settings Wizard.

If enabled for the journal by the site administrator, emails can be sent to all users in one or more role, such as all journal managers and / or all section editors, etc. See [Site Administration > Site Settings](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/site-administration#site-settings) for instructions on enabling this feature.

In the Notify tab, select the user roles that you would like to email. Type your subject and email message. You have the option to send a copy of the email to your own email address. You will receive a status notification indicating that the message was sent successfully.

![OJS 3.3 selecting multiple users to notify with an email message](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-users-roles-notify.png)

This email feature can be used to send practical, core service emails to users who are actively working on the journal. For example, you might send an email to all copy editors reminding them of the “house style” for a particular word use or spelling. Avoid using this feature to notify large numbers of readers; the Announcement feature is preferable for large broadcast emails. See [Website Settings > Setup > Announcements](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-website#announcements) for details about this feature.

If several recipients flag your message as spam, it could result in all emails from the journal being sent to the spam folder. Care must be taken not to abuse this feature by sending excessive, unwanted emails. Become familiar with anti-spam and email privacy laws in your region, such as CASL in Canada and GDPR in the EU and UK. Note that there is no “unsubscribe” option available for users who receive these emails.

It is not possible to add cc or bcc addresses other than your own, or to add attachments to messages. To send attachments you can instead use the Discussion feature or the Submission Library.

**Edit User** allows you to make changes to that user's account.

![Edit information about a user](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-users-edit-user.png)

**Disable** keeps the account in place, but blocks the user from accessing it.

**Remove** un-enrolls the user from all roles in the journal, but the user account remains in the system. The only way to actually remove a user account from your system is to **Merge Users** (see below).

**Login As** allows you to temporarily log in as that user, for example, to complete an outstanding task.

##### Merge User

The Merge User feature lets you fold this user account, including any submissions or assignments, into another user account on your system.

> **Note**: This is the only way to completely delete an account from the system.

You may want to create a dummy user account (e.g., Deleted Users), and use that to merge unwanted accounts into.

To merge users:

1. At Users & Roles > Users, find the user account you want to remove
2. Click the blue arrow next to the username
3. Click **Merge User** from the menu that appears below
4. Find the user account that you want to merge this user account into (the user you want to maintain)
5. Click the blue arrow next to username
6. Click **Merge into this user**
7. Press **OK** to confirm

##### Search Users

When you have a large number of users, you will want to take advantage of the search feature.

![Search for a journal user by name, email, and role](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-users-search.png)

This can help you quickly find a user by first name, last name, or email address, or to see all users in a particular role.

**Note**: If you leave the Search field blank, select a Role, and hit Search, you will get a list of all users in that role (e.g., all copyeditors).

![Search for all users with a given role](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-users-search-roles.png)

##### Add User

To add a new user to your journal, select the Add User link. This will open a new window with a set of fields to fill in.

![Add a user and enter their information](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-users-add-new.png)

Once these fields are completed and you hit _Save_, you will then be asked to assign roles to the new account. Use the _Add Role_ link to open the role selector.

![Assign a role to a new user's account](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-users-add-new-roles1.png)

Once you have added all of the roles, hit the **Save** button.

##### Register a User from Another Journal

On multi-journal installations, an Administrator can register a user from Journal A as a user on Journal B.

1. Log in to Journal B as an Administrator
2. Go to Users & Roles > Users
3. Search for the user from Journal A that you want to register on Journal B, checking off **Include users with no roles in this journal**
4. When the user appears, click the blue arrow next to their name
5. Click **Edit User**
6. Scroll down to **User Roles** on the Edit User box that appears.
7. Check off the role that you want the user to have on Journal B
8. Click **Save** at the end of the form

##### If a User Can't Log In

If a user can't log in to your journal site, tell them to select **Forgot your password** on the Login page. They will then receive a reset password link by email and will be able to reset their password.

If the user has further issues, a Journal Manager or Editor can do the following:

1. Go to Users & Roles > Users
2. Find the user who can't log in and click the blue arrow next to their name
3. Click the **Edit User** button that appears below
4. Enter a new password in the **Password** field, making note of what the password is
5. Check off **User must change password on next log in**
6. Click **Save** at the end of the form
7. Send the new password to the user and instruct them to log in with it

If the user still cannot log in, their account may have been disabled. To re-enable it:

1. Go to Users & Roles > Users
2. Find the user who can't log in and click the blue arrow next to their name
3. Look below their name for **Enable** or **Disable.**  If Disable appears, the account is already enabled. If Enable appears, click it to re-enable the account.

<hr />

### Permissions and Roles {#permissions-and-roles}

This PKP School video explains how to manage roles in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to manage roles in OJS](https://www.youtube.com/watch?v=3sqD41OKuFs)

The OJS workflow revolves around different roles with different permissions and responsibilities for each user, allowing them access to different parts of the workflow. Users in the system must have at least one role. Users can also have more than one role, for example, being a Journal Manager, Editor, and Author in the same journal.

Each role is first assigned a permission level, which will broadly define what level of access a user has to a particular journal. Roles are then further customized by providing a position name, and granting or restricting access to various stages of the Editorial Workflow.

There are a number of predefined roles that you can use and edit in OJS. Read in-depth about these predefined roles organized by their permissions level. Italicized roles are new in OJS 3.
 
* The **Site Administrator** is a single user responsible for administration of the entire OJS installation. This permissions level will not appear in user lists or in role settings.
* **Journal Managers** have access to the entire Editorial Workflow, as well as all other journal settings.
Available predefined Journal Manager roles: Journal Manager, Journal Editor (formerly “Editor” in OJS 2), Production Manager
* **Section Editors** have access to the entire Editorial Workflow, but cannot make any changes to journal settings.
Available predefined Section Editor roles: Section Editor, *Guest Editor*
* **Assistants** can access only the parts of the Editorial Workflow assigned to their role.
Available predefined Assistant roles and their assigned editorial workflow stages:
    * Submission & Review stages: *Funding coordinator*
    * Copyediting stage: Copyeditor, *Marketing and sales coordinator*
    * Production Stage: *Designer*, *Indexer*, Layout Editor, Proofreader
* **Reviewers** are users who appear when you're assigning reviews in the Editorial Workflow and have access to that stage when they're assigned.
* **Authors** can make new submissions.
* **Readers** can access the reader-facing website. This is the minimum permissions level granted to all users.
* **Subscription Managers** can edit site access settings as well as settings related to subscriptions. This is a new permissions level in OJS 3, with one predefined role, *Subscription Manager*.

Predefined and custom roles can be checked from the Roles tab.

![Roles tab showing all current roles in the journal](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-users-roles.png)

From this page, you can see each role, and the editorial stage each role can access. A good example of this is the Copyeditor role, which can only access the copyediting stage. Copyeditors cannot jump to the Review stage to see what happened during the peer review process. See the Editorial Workflow chapter for more information about the different editorial stages.

In addition to assigning and editing the predefined roles, Site Administrators and Journal Managers can also create new roles or rename existing ones. 

#### Editing Roles

Unchecking a box removes access to that stage for users with that role.

Selecting the blue arrow to the left of the role name reveals the edit link. Clicking this opens the editing window.

![Edit details of a role](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-users-roles-edit.png)

**Permission Level**: This indicates how much a user with this role can do in any stage.

The Journal Assistant level can communicate with other users and upload and revise files. In Journals where only one user has been assigned with an Assistant role, they will be automatically assigned to a new submission. Once a second person has been assigned this role, this action will stop.

**Role Name**: You can use this field to easily rename any role.

**Abbreviation**: Each role must have a unique abbreviation.

**Stage Assignment**: This allows you to determine which stage users with this role can access.

**Role Options**: Use these checkboxes to show anyone with this role in the contributor list \(e.g., the author list\). As of OJS 3.2, roles can be assigned permission to edit submission metadata by enabling the checkbox.

Use the second option to determine whether users can self-register in this role. Authors and Reviewers are good candidates for self-registration. You would definitely NOT want to allow users to self-register as Journal Managers or Editors!

The third option is useful for guest editors or possibly section editors, depending upon your preferred workflow and authority chain.

#### Create New Roles

Use the _Create New Roles_ link to open a window where you can create a new role for your journal, including setting which stages it can access and how much permission it should have.

<hr />

### Site Access Options {#site-access-options}

This PKP School video explains how to configure site options in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to configure site access options in OJS](https://www.youtube.com/watch?v=lqf4GmA01PA)

This page allows you to determine how readers can access your journal.

![Site access options tab under Users and Roles](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-users-siteoptions.png)

**Additional Site and Article Access Restrictions**: Choose from these options to limit access.

> Keep in mind that while requiring registration to read open access content can be convenient for your tracking, it can dissuade some people from reading your content. Use with care.

**User Registration**: This option allows you to determine whether users can create their own accounts or must be enrolled by a Journal Manager.

> Allowing users to register themselves, but only into Author, Reviewer, or Reader roles, is a good choice.

> **Original chapter:** [Users and Roles](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/users-and-roles)

---

## Statistics

The statistics features of OJS allow you to view different numbers pertaining to the activity, access, and downloads of various aspects of your site, including article and abstract views, subscription activity, editorial and review activity, and user counts separate by role. There is also a Report Generator section for producing various reports from some of the available data.

This section will describe the statistics report/visualization tools available in OJS and how to use them. If you are interested in how to manage statistics as a systems administrator, including configuring the statistics framework, managing legacy statistics and statistics in OJS 2, and troubleshooting statistics, please view [the PKP Administrator’s Guide’s documentation on statistics](https://docs.pkp.sfu.ca/admin-guide/en/statistics).

For a video walkthrough of Statistics in OJS, see our [Setting up a journal in OJS 3.3. Module 13: Statistics
](https://www.youtube.com/watch?v=fU1orCK7GSM&list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY) video below.

[![Setting up a journal in OJS 3.3. Module 13: Statistics](https://img.youtube.com/vi/fU1orCK7GSM/0.jpg)](https://www.youtube.com/watch?v=fU1orCK7GSM&list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY)

### Definitions {#definitions}

The following definitions may be helpful to you for understanding the variety of statistics tracked by OJS.

* **Abstract page:** the landing page for an article, containing the title, author information, abstract, DOI, and links to any article full-text galleys.  Also known as the “article page” or “landing page.” This page is normally used as the point of record for the article for DOIs or other hyperlinks: Crossref DOIs resolve to article abstract pages, as opposed to galley files, for example, as would most other indexing services.
* **Article view:** within the statistics framework, any reference to an “article view” means a single unique view of the article abstract page by a visitor. This is not an aggregate count of all article and galley views - it refers to abstract views only.
* **Galley view:** within the statistics framework, any reference to a “galley view” means a single unique view or download of the a specific galley file by a visitor. Also known as a “galley download.” This is not an aggregate count of all galley views - if there are multiple galleys for an article \(e.g., an HTML file, a PDF file, etc.\), each will have its own unique galley view count. OJS does not distinguish between galley downloads and views in the metrics table; downloads are counted as galley views.
* **Multi-clicks:** the process \(accidental or nefarious\) of increasing usage counts by clicking on an abstract page or galley file multiple times in quick succession. OJS identifies and removes these attempts from its usage metrics, as per the Project COUNTER Code of Practice.
* **Project COUNTER Code of Practice:** a set of practices developed by COUNTER to establish a means to report on usage metrics for electronic resources in a consistent way. The Code provides rules on what should be counted as a view, including specific rules for robot usage and multi-click abuse. OJS filters metrics through these rules. It should also be noted that PKP is part of the COUNTER Bots and Crawlers Working Group.
* **Robots, crawlers, bots:** nonhuman site visitors who may still view and download article data. These are usually identified as such to the server, and OJS does not count them in its usage metrics, as per the Project COUNTER Code of Practice.

### Articles {#articles}

OJS offers Editors and Journal Managers the option of viewing graph and table representations of article usage, including abstract views and full-text downloads.

The visual statistics can be found under Statistics on the left menu panel, by clicking Articles.

![OJS interface with the Articles option highlighted under Statistics in the left menu.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/ojs-statsmenu.png)

The Articles statistics show the articles’ abstract views in both graph and table format. The visual graphic can be changed to Monthly or Daily view. The table format will allow you to filter the Total in ascending or descending order.

![Sample of a graph of abstract views produced by the Articles statistics tool.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/abstract-views.png)

![Sample article details table produced by the Articles statistics tool.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/article-details.png)

The calendar icon on the top right corner of your dashboard gives you the option of changing the article view to the Last 30 days, Last 90 days, Last 12 months, All dates, or a Custom Date Range.

![The calendar used for selecting date ranges in the Articles statistics tool.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/calendar-range-articles.png)

The filter icon on the top right corner of your dashboard gives you the option of filtering the articles by Sections.

![The calendar used for selecting date ranges in the Articles statistics tool.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/article-filters.png)

You also have the option of searching the statistics of a specific article by title, author, or manuscript ID by using the search function under Article Details.

![The search bar for locating specific article statistics.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/article-details-search.png)

### Editorial Activity {#editorial-activity}

This section provides statistics about the editorial workflow, such as number of submissions received, days to first editorial decision, and acceptance and rejection rates. You can filter these statistics using a custom date range to, e.g., find the number of articles accepted during a 12-month period.

![Sample of editorial statistics.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/editorial-activity.png)

There are some important things to note when considering the data in these reports:

* Published submissions within a date range only count the initial publication date and not subsequent versions.
* Days to decision uses an 80% threshold, so the data listed represent that 80% of submissions with a decision have received one within X number of days.
* The acceptance and decline rates only count submissions that have received an accept/decline decision, so they exclude submissions still in the queue.
* If a date range is applied, it only counts submissions that were submitted AND accepted/declined within that date range. So, e.g., a submission that was submitted before the date range but received an accept/reject decision within the date range will not be counted. For this reason, it's best to use long date ranges and older date ranges to get accurate acceptance/rejection rates.

An Editorial Activity Report will be generated monthly and can be sent by email to editors and section editors. All managers and section editors are automatically opted out of the monthly report; however, you can opt in by going to User Profile > Notifications and unchecking the box that disables the automated email.

### Users {#users}

This section provides information about new user/role registrations within a specified time period. The Total column is not a total number of accounts created; it identifies how many users have that role in the system right now. When an existing user receives a new role, such as a registered author becoming a reviewer, that addition to the total number of reviewers in the system will be reflected in the data by an increase in the number of reviewers but no change in the total number of users.

![Sample users statistics data.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/users.png)

### Report Generator {#report-generator}

The Report Generator page provides access to a variety of reports from your journal.

![The list of reports on the Report Generator page in OJS, detailed below.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/report-generator.png)

The system generates reports that track the details associated with site usage and submissions over a given period of time. These reports can be broadly grouped into “usage” reports that contain usage metrics indicative of visitor readership and “content” reports that provide data on the respective item (eg. review information). Reports are generated in CSV format which requires a spreadsheet application to view. 

* PKP Usage Statistics Report: Provides granular daily usage metrics for all article, article file, issue and homepage views/downloads. Will include visitor country data, if that is being logged. See Usage Statistics Report below for more information and examples. (Usage)
* Subscriptions Report: Provides information on any individual and institutional subscriptions. This report option is only available if subscriptions are enabled on the journal. (Content)
* Articles Report: Provides a spreadsheet of all published articles. (Content)
* COUNTER Reports: Provides COUNTER reports for all journals on the OJS application. Provides monthly and year to date aggregate counts for abstract and galley views. (Usage)
* Review Report: Provides review information on all articles in the system, including reviewer names, reviews, and recommendations. (Content)
* View Report: Provides a report on galley and abstract views by readers (i.e., how many times a PDF for an article has been viewed). (Usage)
* Custom Report Generation: Customizable version of the Usage Statistics report, where various facets can be selected and specific date spans can be set. See Generate Custom Report for more information and examples. (Usage)

#### Usage Statistics Report

This report provides granular data on monthly views for the journal homepage, issue TOCs, article abstract/landing pages, and file views in CSV format. It provides country information (if configured). Each row provides a total monthly view count for a particular object (journal home page, article abstract page, article galley, or issue table of contents). It further facets this by country if country support has been enabled and properly configured.

**Use for:** generating a multifaceted overview content usage from month to month. It lists monthly view counts for all articles, article file downloads, issue TOC views, and journal homepage views for the specified timespan. Additional manual manipulation of the resulting report must be done to achieve aggregate results.

**Do Not Use for:** attempting to get a quick usage snapshot, legacy usage, or journals that have a very large metrics dataset \(due to long history, high readership, or depth of metrics granularity\). Use the Custom Report Generator instead.

**Special Notes:**

* This report attempts to capture the entire usage history for: the journal home page, all article abstracts, all article galleys, and all issue table of contents.
* **OJS version 3.1.1 or older installs**: To reduce the potential for exceeding time limits for downloads, this report only provides 5,000 records. If you have a lot of reportable data, this report will most likely not report it all. If this is the case, the Custom Report Generator plugin should be used instead, using smaller date ranges. (This restriction was removed in OJS 3.1.2.)

**Example Data \(slightly edited for clarity\):**

| **ID** | **Type** | **Title** | **Issue** | **Journal** | **Country** | **Month** | **Count** |
| --- | --- | --- | --- |
| 1 | Journal | Canadian Journal of Communication | CJC | CA | 201502 | 1678 |  |
| 112 | Article | Toronto Star Fires Reporter Claire Hoy, Sues Him and TV Stations on Libel Charge | Vol 1, No 3 \(1974\) | CJC | CA | 201502 | 3 |
| 112 | Article | Toronto Star Fires Reporter Claire Hoy, Sues Him and TV Stations on Libel Charge | Vol 1, No 3 \(1974\) | CJC | US | 201502 | 1 |

From the above example, we can see that in February 2015 the main CJC journal homepage was viewed 1,678 times, which the article “Toronto Star Fires Reporter …” was viewed 3 times from Canada and once from the United States.

#### View Report

This report provides per-article abstract views and galley views/downloads. These usage metrics are not filtered for multi-clicks or bot/crawler activity and thus may seem inflated in comparison to more recent statistics.

Example Data (slightly edited for clarity):

In the sample below we can see that article 95, “The Making of the Canadian Media,” has had 443 abstract views and 1476 total galley views. The PDF and Total Galley views are the same because there were no HTML views. With article 1125, “Digital Networks,” the abstract was viewed 1821 times and total galley views are 8478, which is the sum of the HTML and PDF views.

****

| **ID** | **Article Title** | **Issue** | **Date Published** | **Abstract** | **Total Galleys** | **HTML** | **PDF** |
| --- | --- | --- |
| 95 | The Making of the Canadian Media | Vol 6, No 1 \(1979\) | 1979-01-03 | 443 | 1476 |   | 1476 |
| 1125 | Digital Networks | Vol 24, No 4 \(1999\) | 1999-04-01 | 1821 | 8478 | 2093 | 6385 |

#### Generate Custom Report

Use this feature to build your own reports. These reports provide granular data on daily views for the journal using the full metrics dataset. You are able to aggregate results by:

* Country
* Region
* City
* Month
* Day

Metrics are tracked against specific item types (AKA “objects”):

* File downloads
* Abstract views
* Issue Table of Contents views
* Journal Homepage views

![The custom report generator interface in OJS.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator1.png)

You are also able to limit results to specific date spans.

This is the most flexible report option available in OJS and can provide a very detailed amount of data. Below are some examples of statistics questions that may be useful to journals, as well as instructions on how to formulate a report to answer those questions using this feature.

Special Notes on the Report Generator:

* Depending on the amount of data in your system, the facets you choose to retrieve, and the date span you choose, the system may fail to completely generate a report without timing out. If you encounter this, try reducing the requested date span.
* If you generate a custom report, the report will also provide you with a Report URL that you can save to use to repeat the identical report process. Make sure to copy and save the URL somewhere so that you can re-run your search later (it will disappear once the page is reloaded).
* If you create a report that reports on “yesterday” or “current month,” the resulting Report URL will always use “yesterday” or the “current month” relative to the day you run it. So if you originally created a report to report on “yesterday” a year ago and then ran it today, it would report on yesterday. However, if you specify a specific date range, say April 1 - April 15 2018, the resulting Report URL will always report metrics for that specific range.
* Note that the current day’s data will not be available until the next day.
* The generator works like a funnel for data. The trick is to narrow down the bigger elements (such as date range), select what you’re interested in from there (issues, articles, etc.), then tweak the data at the end (i.e., sort by number of downloads).
* The Report Generator is most useful if you use the Advanced Options. All the examples below make use of the advanced options.

##### Example report: How well has a particular (i.e., most recent) issue performed over the last few months?

This particular query will give you a monthly count of how many full text galleys have been downloaded from a particular issue. You’ll have a column for month and total count for month and a separate row for every month.

* Under “Default report templates” select “Article file downloads” from the dropdown list.
* Uncheck all boxes in the “Aggregate stats by.”
* Click on the “Month” radio button and enter date range under “Or select range by.”

![The custom report generator with the above described settings entered in OJS.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator10.png)

* Open “Advanced Options” and select only “Month” under Columns

!["Month" selected under the advanced options in the custom report generator.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator3.png)

* We want only a very light filtering of our data. Select submission files, then select the galley formats you wish to include in your report. This example selects only PDF, but you could select PDF and HTML if your journal also offers full-text HTML article downloads. Use Ctrl+Click or Command+Click to select multiple types. Under Object ID, enter the object ID of the issue that you’re interested in, which will be located in the issue’s URL. For example, an issue with the URL publicknowledgeproject.org/journal/index.php/journal/issue/view/**24** has the object ID 24.

![A sample issue ID entered into the custom report generator.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator4.png)

* Ignore the “By geo location” and “Order by” options, and click “Generate custom report.”
* You’ll end up with a very simple monthly report of the galley downloads for the one issue of interest for your journal.

![Results in .csv format returned from the above custom report.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator5.png)

* Save the URL at the bottom of the page for your records!

##### Example report: What are the most downloaded articles over the last 5 years?

This report will present a list of article titles (and the issues they come from) ordered by descending download counts.

* Select “Article file downloads” from the dropdown box.
* Uncheck all boxes under “Aggregate stats by.”
* Select the “Month” radio button and enter a date range.

![The custom report generator with the above described settings entered in OJS.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator10.png)

* Select only “Article” and “Issue” under Columns. We’ll be narrowing down the type at a later point in the query.

!["Article" and "Issue" selected under the advanced options in the custom report generator.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator6.png)

* Select “Submission Files” under object type and select all galley types you wish to include in the download count. 

![The above described settings entered in OJS.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator7.png)

* Ignore “geo location” (not shown here).
* “Order by” will arrange your articles in descending order by number of downloads. To achieve this, select “Count” in the first drop down box, and the select “Descending.”

![Arrows pointing to the first two drop downs in the Order by section, with "Count" and "Descending" selected.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator8.png)

* The resulting report will appear as follows (truncated):

![Results in .csv format returned from the above custom report.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator9.png)

* Save your URL at the bottom of the page!

##### Example: What’s our most popular issue?

This query displays a count of full text downloads for each journal issue and orders the results from highest to lowest.

* Select “Article file downloads” from the dropdown box.
* Uncheck all boxes under “Aggregate stats by.”
* Select the “Month” radio button and enter a date range.

![The custom report generator with the above described settings entered in OJS.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator10.png)

* Under columns, click on “Issue.”

!["Issue" selected under the advanced options in the custom report generator.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator11.png)

* Under “Filters”, select “Submission Files” under Object Type, and select the galley file type(s) used by your journal (use Ctrl+Click or Command+Click to select multiple types).

![The above described settings entered in OJS.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator7.png)

* Ignore “geo location” (not shown here).
* “Order by” will arrange your articles in descending order by number of downloads. To achieve this, select “Count” in the first drop down box, and the select “Descending.”

![Arrows pointing to the first two drop downs in the Order by section, with "Count" and "Descending" selected.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator8.png)

* Run your report. Here is what you’ll get:

![Results in .csv format returned from the above custom report.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator12.png)

* Don’t forget to save your URL to run at a later date.

##### Example: What countries are downloading our articles (for a specific date interval)?

This query will display aggregate counts for fulltext downloads by country in descending order. Note that one will need to specify a date range.

* Select “Article file downloads” from the dropdown box.
* Uncheck all boxes under “Aggregate stats by.”
* Select the “Month” radio button and enter a date range.

![The custom report generator with the above described settings entered in OJS.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator10.png)

* Select only “Journal” and “Country” under Columns. You can use Ctrl+Click or Command+Click to select multiple items. We’ll be narrowing down the type at a later point in the query.

!["Journal" and "Country" selected under the advanced options in the custom report generator.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator13.png)

* Under “Filters”, select “Submission Files” under Object Type, and select the galley file type(s) used by your journal (use Ctrl+Click or Command+Click to select multiple types).

![The above described settings entered in OJS.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator7.png)

* “Order by” will arrange your articles in descending order by number of downloads. To achieve this, select “Count” in the first drop down box, and the select “Descending.”

![Arrows pointing to the first two drop downs in the Order by section, with "Count" and "Descending" selected.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator8.png)

* Run the report.
* Don’t forget to save your URL to run at a later date.

![Results in .csv format returned from the above custom report.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/custom-report-generator14.png)

#### Display Usage Statistics for Readers

In OJS 3 you can display an article’s usage statistics for the current year as a graph on the article landing page by using the Usage Statistics Plugin, as seen in this image.

![A sample article with a graph of monthly downloads shown under the abstract.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/reader-statistics.png)

To enable the Usage Statistics Plugin:

1. Go to Settings &gt; Website &gt; Plugins.
2. Under Generic Plugins, find the **Usage Statistics Plugin**.
3. Check the box to the right of the plugin description.

To configure the Usage Statistics Plugin:

1. Go to Settings &gt; Website &gt; Plugins.
2. Under Generic Plugins, find the **Usage Statistics Plugin**.
3. Click the blue arrow to the left of the plugin name to make links appear below the plugin.
4. Click **Settings**.
5. Scroll to the bottom of the pop-up box that opens to the section **Statistics Display Options**.
6. Check the box beside **Display submission statistics chart for reader**.
7. Below that you can select whether you would like to display the statistics as a bar or line graph and the maximum number of months to display usage for.
8. Click **Save**.

![The optional statistic checkboxes where users can enable/disable city or regional data collection, and enable the statistics viewable to readers.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/usage-stats-plugin-configuration-basic.png)

Please note the following:

* Usage statistics can only be displayed for the current year. The plugin is reset at the beginning of each year.
* The statistics being displayed indicate the number of times an article was downloaded.

> **Original chapter:** [Statistics](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/statistics)

---

## Tools

The Tools section can be accessed from the left sidebar menu.

![Tools side menu options](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-users-tools.png)

Tools consist of an Import/Export tab, a Report Generator tab (called Statistics in OJS 3.1.1 and earlier), and a Permissions tab.

> **Video:** [Video of setting up a journal in OJS 3.3. Module 14: Tools](https://www.youtube.com/watch?v=v3zjjVFYAyc)

This PKP School video explains how to access and use Import/Export tools. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

### Import/Export {#importexport}

Import/Export allows you to easily get data out of your OJS journal and get data into it.

![List of Import/Export plugins available](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-users-tools-import.png)

Some of the tools allow you to export to third-party systems, such as PubMed or the DOAJ. Others allow you to import or export article data.

If you want to export user data, you can find the option to export it as an XML file here. If you prefer your user data in a spreadsheet format, you can download it as a CSV file from **Statistics > Users**.

For detailed instructions on importing and exporting see the [Administrator's Guide](https://docs.pkp.sfu.ca/admin-guide/en/data-import-and-export).

For more information on the Crossref XML Export Plugin, see the [PKP Crossref Guide](https://docs.pkp.sfu.ca/crossref-ojs-manual/en/).

#### Quick Submit Plugin

> **Video:** [Video of setting up a journal in OJS 3.3. Module 18: Plugins- QuickSubmit](https://www.youtube.com/watch?v=_nm1dGIZS8Y)

This PKP School video explains how to use the Quick Submit Plugin to add complete submissions to an issue. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

The Quick Submit Plugin allows you to quickly add complete submissions to an issue. It provides a one-step submission process for editors needing to bypass the traditional submission, review, and editing process.

The Quick Submit Plugin can be used in the following cases:

* Journals who are using OJS to display and publish their content without using the editorial workflow
* Journals that were published using another platform and are migrating to OJS, when a conversion tool for that platform is not available
* Journals that were originally published in print and have since been digitized

To use this plugin, you will need the following:

* To be enrolled as an Editor or Journal Manager
* A set of ready-to-publish files (e.g., PDFs)
* All of the metadata for the files (e.g., author names, titles, abstracts, etc.)

First, ensure that the Quick Submit Plugin has been installed and enabled for your journal.  You will need to have the Journal Manager role to enable the plugin and the Administrator role to install the plugin.

![Settings side menu options with the option for Website selected.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/find-plugins.png)

1. Go to Settings > Website > Plugins
2. Under Installed Plugins, look for the Quick Submit Plugin.  If you see it listed, skip to step 8.
3. If you do not see the Quick Submit Plugin under Installed Plugins, go to the Plugin Gallery tab.
4. Click on Quick Submit. A popup box will open.
5. Click on Install.  If you do not see the Install button, you will need to ask the Administrator of your site to install the plugin for you.
6. A popup box will open and ask “Are you sure you wish to install this plugin?”  Click OK and wait a few minutes while the installation completes.
7. After the plugin has been installed, go back to the Installed Plugins tab and find the Quick Submit Plugin.
8. Check the box to the right of the plugin name and description to enable the plugin.

![List of Import/Export plugins from the Installed Plugin tab in Website settings.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/enabled-import-plugins.png)

Next, you will need to create the issues (or issue) that will contain the new articles you are importing.

1. Go to Issues > Future issues and select Create Issue.
2. Enter metadata for the issue
3. If the issue is already published you can check off "Published"
4. Click Save.
5. Do this for all of the issues you are uploading articles for.

![Volume 1 Number 1, 2017 issue titled From below created under Future Issue.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/create-issue.png)

Next you can import each article with the Plugin.

![Tools side menu options with Import/Export selected.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/import-plugins.png)

1. Go to Tools > Import/Export and select Quick Submit Plugin.
2. Upload a cover image if you have one.  This field is optional and can be ignored.
3. Choose the section of the journal that the article will appear in from the drop-down list in the Section field.
4. Enter the metadata for the article in the other fields. If you do not see all of the metadata fields you want, go to Workflow Settings > Submission > Submission Metadata to configure what fields should be included in submissions.
5. Under List of Contributors, click Add Contributor to enter the names of authors and other contributors to the article.
6. Under Galleys, click Add Galley to upload a PDF file of the article.  A popup box will open where you can enter the Galley Label and language of the galley.  Once you click Save, another box will open where you can select the Article Component and upload the file.
7. At the end of the Quick Submit Plugin form, you can select whether you want the article you are adding to be published immediately or unpublished if you wish to publish it later. If you select **Published**, you will have to select the issue you would like to publish it in and enter the **Date Published**. You can also optionally enter page numbers and permissions information.
8. When you have finished entering all data for the article, click Save.

![Submission form on QuickSubmit.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/quick-submit-plugin-2.png)

DOIs are not added with the QuickSubmit Plugin. Instead, you have to add them separately.

To add existing DOIs to articles that have already been assigned:

1. Enable and configure the DOI plugin so that you need to "Enter an individual DOI suffix for each published item."
2. After you finish uploading the article with the QuickSubmit plugin, click “Go to Submission” to go to the article’s submission record. Or go to the article's submission record through the Submissions dashboard.
3. Open Metadata on the top right and go to the Identifiers tab
4. Enter the DOI suffix for the article.
5. Click Save and then Save again to assign the DOI
6. If you normally assign DOIs using a default pattern, re-configure the DOI plugin for this after you have finished adding DOIs to articles you uploaded with the QuickSubmit plugin

To assign new DOIs to articles:

1. Ensure that the DOI plugin is enabled and configured
2. After you finish uploading the article with the QuickSubmit plugin, click “Go to Submission” to go to the article’s submission record. Or go to the article's submission record through the Submissions dashboard.
3. Open Metadata on the top right and go to the Identifiers tab. You should see a preview of the DOI that will be assigned and a checked box next to "Assign the DOI to this article."
4. Click Save and the DOI will be assigned.

### Permissions {#permissions}

The Reset Article Permissions tool allows you to reset the copyright statement and license information on all published articles, and will revert it to your journal's current default settings. Take caution when using this tool and consult legal expertise if you are unsure what rights you hold over the articles published in your journal.

![Option to reset artile permission in the Tools Permissions tab.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-jm-users-tools-permissions.png)

> **Original chapter:** [Tools](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/tools)

---

## Subscriptions

OJS allows you to restrict some or all of your content to subscribers. To enable Subscriptions, first go to [Settings > Distribution > Access](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-distribution).

### Subscription Policies {#subscription-policies}

Fill in details about your subscription policies on this page.

![The Subscription policies tab in the Subscriptions menu.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-subscriptions-policies.png)

- **Subscription Manager**: Add personal details for the responsible person.
- **Subscription Information**: Add policy details to display on the journal website.
- **Subscription Expiry**: Determine whether past subscribers should continue to have access to older content.
- **Subscription Expiry Reminder**: Configure automated renewal reminders.
- **Online Payment Notifications**: Keep the Subscription Manager informed of payment activities.
- **Open Access Options for Subscription Journals**: If appropriate select the number of current months for restricting access. Older content will be automatically made open.

### Subscription Types {#subscription-types}

The next step in setting up subscription management is to designate the types of subscriptions the journal offers.

![The Subscription Types tab in the Subscriptions menu](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-subscriptions-types.png)

Journals typically offer individual subscription and institutional subscription rates. Some journals may have special offers for members of an organization or students. OJS will support the management of print and/or online subscriptions. More than one type of subscription can be created to cover longer periods of time (12 months, 36 months).

Select **Create New Subscription Type** to add a new one.

![The Create New Subscription Type window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-subscriptions-types-create.png)

- **Name of Type**: Give this new subscription type a unique name (e.g., Student).
- **Description**: Provide a brief description that will appear on the website.
- **Cost**: Select the currency type and amount.
- **Format**: Choose the appropriate format (e.g., Online).
- **Duration**: Enter the number of months this type of subscription will cover (e.g., 12).
- **Subscriptions**: Indicate whether this type covers individuals or institutions.
- **Options**: Select the appropriate options (if any).

### Payment Types {#payment-types}

> **Video:** [Module 11: Distribution. Unit 3: Payments](https://www.youtube.com/watch?v=9r0mRqtNVuU)

This PKP School video explains how to set up different payment types in your journal. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

If you haven't already done so, go to [Settings > Distribution > Payments](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-distribution) and set the appropriate currency and payment method (e.g., PayPal).

Use this page to set the amounts charged for various types of fees.

![The Payment Types tab in the Subscriptions menu.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-subscriptions-paytypes.png)

#### Author Fees

If you want to charge an article processing charge (APC) to authors, enter the amount here. Enable Author Fees will allow you to request an article processing charge after the review process has been completed. When the article is accepted by the editor following Review, the editor will have the option to require payment. This will result in the author receiving a notification in OJS and an email, which will direct them through the payment process.

Note that the option to notify authors about the Author Fee will appear only when the payment details (PayPal account details or manual PayPal instructions) have been completed in [Settings > Distribution > Payments](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-distribution#payments).

![A sample notification to the author with the "Request publication fee" option enabled.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-subscriptions-authorfees.png)

Authors will be required to login to the journal before being directed to PayPal to process payment.

#### Reader Fees

If you want to charge fees to access individual articles and issues, you can enter the prices for articles and issues here.

You can apply the fees to PDF files only by checking off "Only Restrict Access to PDF version of issues and articles".

Note that in order to sell access to an issue, you will need to upload an issue galley.

#### General Fees

Use this to charge other fees, such as memberships.

### Payments {#payments}

As various payments are received, they will be listed under this tab.

Only payments made through PayPal will be recorded here.

As of 3.3, a Payment tab has been added on the manuscript dashboard for Editors to record the payment status of Author fees. Manuscripts can only be schedule to an issue once the Author fee has been marked as Paid or Waived.

![Author Fee Payment record tab.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-subscription-authorpublicationfee.png)

### Individual Subscriptions {#individual-subscriptions}

All types of individual subscriptions will appear here.

![The Individual Subscriptions tab in the Subscriptions menu.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-subscriptions-indiv.png)

You can create a new individual subscription by using the Create New Subscription link. First, however, you will need to create a new account for that person under Users & Roles (see [the User Accounts chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/user-accounts)). Once that is done, you can search for the account here, and apply the different configurations.

![The Create New Subscription window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-subscriptions-indiv-create.png)

**Subscription Type**: Select the appropriate type for this new subscriber (e.g., Student) and its status (e.g., Active).

> Subscription Types were configured earlier in this chapter.

**Date**: Set the start and end dates for this subscription.

**Membership**: If the subscriber is associated with any relevant memberships, add that information here (optional).

**Reference Number**: If the subscribe is associated with any relevant reference number (such as an invoice number for payment), add that information here (optional).

**Notes**: If you have any relevant notes to add, record that information here (optional).

### Institutional Subscriptions {#institutional-subscriptions}

All types of institutional subscriptions will appear here.

![The Institutional Subscriptions tab in the Subscriptions menu.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-subscriptions-instit.png)

Institutional subscriptions are managed similarly to individual subscriptions, but are used for libraries, research institutes, and other organizes that subscribe to your journal.

You can create a new institutional subscription by using the Create New Subscription link. First, however, you will need to create a new account for the institution's contact person under Users & Roles (see [the User Accounts chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/user-accounts)). Once that is done, you can search for the account here, and apply the different configurations.

![The Create New Subscription window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-subscriptions-instit-create.png)

- **Subscription Type**: Select the appropriate type for this new subscriber (e.g., Library) and its status (e.g., Active). (Subscription Types were configured earlier in this chapter.)
- **Date**: Set the start and end dates for this subscription.
- **Institution**: Add the name of the institution for this subscription (e.g., Simon Fraser University Library).
- **Mailing Address**: Add the address of the institution.
- **Domain**: Readers coming from a computer with this domain will automatically receive access (e.g., sfu.ca). This will apply to on-campus users.
- **IP Ranges**: The institution may provide you with IP ranges. Readers using a computer in this IP range will automatically receive access. Each IP range should be entered as a new line.

![The IP ranges field where IP ranges are entered.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-subscriptions-instit-IP.png)

- **Notes**: If you have any relevant notes to add, record that information here (optional).

### Payment Notifications {#payment-notifications}

#### Manual payment notifications

With a manual payment notification, once this information is filled out the subscription manager is notified via email that a manual payment has been made. Since the sandbox is restricted from sending emails any tests that you would do would not send an email as it normally does.

These manual subscriptions will also be recorded in the Payment > Individual or Institutional tab. The example below shows a test subscription.

From here the subscription manager can update the status as needed based on your workflow.

![A sample individual subscription with the "Awaiting Manual Payment" status.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-subs-manual-notification.png)

#### PayPal payment notifications

When a payment has been processed through PayPal the account administrator for your PayPal account will receive notification of payment. The payment will also be recorded in the Payment tab in Payments > Payment.

### Subscription Block {##subscription-block}

When a user is being provided access to a site or its content via a subscription, the information of the subscriber providing access can be displayed in the sidebar. The Subscription Block feature must be selected for display in Website Settings > Appearance > Sidebar Management.

### Setting Articles as Open Access {#setting-articles-as-open-access}

If you would like to set certain articles as Open Access, this can be done by going to **Issues** on the left menu. If you would like to set it before publishing the issue, click the Future tab followed by the blue arrow beside the Issue.

Under the Table of Contents, check off the articles that will be set as Open Access.

![The Open Access checkbox located beside an article in the Table of Contents.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-jm-subscriptions-single-article.png)

> **Original chapter:** [Subscriptions](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/subscriptions)

---

## User Account Management

This PKP School video explains the user dashboard in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of the user dashboard in OJS](https://www.youtube.com/watch?v=OoXQzB_s0gM)

When a user log into the system, they will be taken to their Dashboard. From here, users can change their profile information or account settings, as well as see all of the functions of the system to which they have access. For example, a Reviewer will only see the submission they have been assigned to review, while an Editor will see all of the submissions in the editorial workflow. More information about roles and permissions levels is available in the [Users and Roles chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/users-and-roles).

### Registering with a Journal {#registering-with-a-journal}

This PKP School video explains how to register and log in to a journal in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to register and log in to a journal in OJS](https://www.youtube.com/watch?v=kQUTzi2JKiQ)

Unregistered visitors to a journal can normally register as a Reader, Author, and/or Reviewer. Journal Managers are able to remove the ability for visitors to self-register, in which case a notice will appear stating that registration is currently closed (see Journal Settings), but Journal Managers can always register users at any time, and for any role.

To register with a journal, click the Register link on the upper right corner.

![The Register link at the upper right corner of the journal site.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-registration.png)

This will open the Registration Form for you to complete with all required information.

![The Registration Form.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-registration-form.png)

All fields with an asterisk (First Name, Last Name, Affiliation, Country, Email, Username, Password, Repeat Password) are mandatory. If the journal is multilingual, you will need to select your preferred language.

You will be automatically registered as a Reader and an Author. You will be given the option to register as a Reviewer as well.

You will not be able to self-register for an Editorial Role (e.g., Editor, Section Editor, Copyeditor, Layout Editor, Proofreader, or Journal Manager). If you need to be enrolled at that level, contact a current Journal Manager or Site Administrator.

<hr />

### Viewing and Changing your Profile {#viewing-and-changing-your-profile}

This PKP School video explains how to manage a user profile in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

> **Video:** [Video of how to manage a user profile in OJS](https://www.youtube.com/watch?v=OoXQzB_s0gM)

To view and edit your profile, log in and click your Username link from the upper right corner. Choose the View Profile link.

![The View Profile menu.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-edit-profile.png)

From here, by choosing the different tabs, you can update your personal details, contact information, change your roles, add a personal image (which some journals may publish along with your article or on a list of editors), determine your notification settings, or update your password.

Under **Notifications**, you can configure what kinds of notifications you receive from the journal when events occur, such as a new journal issue is published or there is activity on a submission you're involved in.

* Check off "Enable these types of notifications" if you want to see a notification of this event on your dashboard when you log in to the site
* Check off "Do not send me an email for these types of notifications" if you do not want to receive an email notification about this event

![The Notifications tab where you can manage notifications.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-user-notifications.png)

The **API tab** on the user profile allows you to use OJS’s REST API to interact with external applications.  However, most users will not use the API and can ignore this tab.

### Resetting your Password {#resetting-your-password}

You can reset your password by:

1. Logging into the journal
2. Selecting your username and View Profile from the upper right corner of the screen
3. Choosing the Password tab
4. Entering your current password and then your new password twice
5. Hitting Save

![The password reset screen.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-change-pw.png)

Your password is now changed.

#### If you forgot your password

Retrieving your password is a three-step process:

First you need to request a new password:

1. Click the **Login** link at the top-right corner of the navigation bar
2. Click the **Forgot your Password** link on the following page
3. Enter your email address
4. Click **Reset Password**

Then you need to check your email account and confirm your request:

1. Open your email account
2. Open the confirmation email message from the journal (you may need to check your Spam folder)
3. Click the link to confirm that you did indeed request your password to be reset. You will be taken back to the journal in question, and the system will email you a new password.

Now you can retrieve you new temporary password and log in:

1. Go back to your email account
2. Open the email message containing your temporary password (you may need to check your Spam folder)
3. Log in to the journal with your temporary password
4. Fill in a new password when prompted by the journal

If you need further assistance, contact the journal's editorial team. A list of contacts should be available on the **About** page.

> **Original chapter:** [User Account Management](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/user-accounts)

---

## Authoring

In this chapter, you will learn about how an author works in OJS from registration through to proofreading the final galley.

> **Video:** [Video of Submitting an Article in OJS](https://www.youtube.com/watch?v=AJwDWdAu8BQ)
This PKP School video explains how an author can register for a journal and submit an article. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDUKJbWtr4bgy133_jwoiqoF).

### Registering with the Journal {#registering-with-the-journal}

To make a submission to an OJS journal, you will first need to register a user account with a journal and log in \(see [Registering with a Journal](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/user-accounts#registering-with-a-journal)\). After that, when you login, you will be taken to your Dashboard.

![Submissions queue in author dashboard](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-au-dashboard-empty.png)

It is currently empty as you have made no submissions.

<hr />

### Submitting an Article {#submitting-an-article}

Start a new submission by clicking the **New Submission** button on the right side of the screen. You will be taken to Step 1 of a 5-Step process to upload and describe your submission.

![Author submission queue with new submission button](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-au-dashboard-empty.png)

#### Step 1

In **Step 1** you will provide preliminary information about your submission.

![Article submission start screen](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-au-dashboard-new-1.png)

If the journal allows submissions in multiple languages, you can select the language of your submission from the drop-down menu. Languages can be enabled in Website Settings -> Setup -> Language.

If the journal has Categories enabled and setup, you can select the categories your submission from the list. Categories can be setup in Journal > Categories.

Select the appropriate section for your submission \(e.g., article, review, etc.\). If you aren’t sure which section is appropriate, make your best guess.

Read and agree to the statements in the submission checklist by checking each box. Include any comments for the editor, read the journal’s privacy statement, and then click the **Save and Continue** button to move to **Step 2**.

#### Step 2

On **Step 2**, a window will open allowing you to upload your submission file.

![File upload screen](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.3-author-submission-step2.png)

In OJS 3.3 authors can upload multiple files at once, as well as drag-and-drop files.

[Video: OJS 3.3 drag and drop multiple files.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/submission3.3-files.mp4)

Once you've uploaded all your files you can indicate the file type for each from a single menu panel, and metadata such as a description or license can be entered during the workflow.

Once you have finished uploading and labelling all of your files, click the **Save and Continue** button to move to **Step 3**.

#### Step 3

On **Step 3**, you will be asked to add more information about the submission, including the title of the submission (broken down into prefix, title, and subtitle), and the abstract. If the journal allows submissions in multiple languages, clicking on each metadata field will reveal the option to enter the metadata in the other languages that are enabled, allowing you to enter the title, subtitle and abstract in the other language(s). Scrolling down...

![Enter title metadata in another language](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-au-dashboard-new-3.png)

...you are able to add any additional contributors.

![List of contributors](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-au-dashboard-new-3-contrib.png)

You can add more contributors (e.g., co-authors), by clicking the **Add Contributors** link. This will open a new window with fields to enter their information.

![Add contributors](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-author-submission-step3-2.png)

Hit **Save**, and the new contributor will appear on the screen.

![List with new contributors added](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-au-dashboard-new-3-contrib-new.png)

If the categories are enabled in the journal you are submitting to, you will be able to select a category for the manuscript submission, if it applies.

![Select a category](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-authoring-category.png)

You may also see additional fields to complete, such as keywords. If additional languages are enabled for the journal, you can enter the metadata in these languages. Clicking on the metadata field will reveal the fields for other languages enabled in the journal.

![Enter keywords](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-author-submission-step3-4.png)

To enter keyword, simply type the word or phrase and hit your Enter key. The word or phrase will be formatted as a keyword.

Click **Save and Continue** to move forward.

#### Step 4

On Step 4, you will be asked to confirm that you are happy with your submission.

Click **Finish Submission**.

![Finish submission screen](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-au-dashboard-new-4.png)

A box will pop up asking you to confirm you are finished. Click **OK**.

![Confirm submission screen](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-author-submission-step4-1.png)

#### Step 5

![Next steps submission screen](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-au-dashboard-new-5.png)

Your submission is now complete! The editor has been notified of your submission. At this point, you can follow the links to:

* Review this submission
* Create a new submission
* Return to your dashboard

Once you complete a submission, you cannot make changes to it.  If you want to replace the file you submitted or make other changes to the submission, you will need to contact the editor through the Pre-Review Discussions tool.

#### Dashboard

And here is your submission in your Dashboard. You can see that it is currently in the _Submission_ stage.

![Submission in author dashboard](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-au-dashboard-new-sub.png)

Over the coming days, it will move into the Review stage, and if accepted, into the Copyediting and Production stages before being published.

<hr />

### Editing Metadata {#editing-metadata}

In OJS 3, you may edit your own metadata at different stages of the editorial workflow. This will be dependent on settings granted by the Journal. You may either have global permission to make edits or have to send a request to the Editor to do so.

Changes might include updated abstracts, correcting spelling errors, or adding additional contributors.

To make edits to your submitted manuscript, click on the publication tab of your submission.

![Submission publication tab](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-auth-dashboard-publication.png)

You will be able to make changes to any of the sub-menus on the left by clicking to those tabs. If multiple languages are enabled for the journal, you will be able to edit metadata in those languages by clicking on the language tab in the top right. Click ‘Save’ once you’re done making your changes.

![Publication menu items](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-auth-dashboard-publication2-language.png)

When granted permission, you will be able to make changes to the following sections on the Publication tab: Title & Abstract, Contributors, and Metadata. While Galleys is listed as an option on the side menu, you will not be able to upload or make changes in this section.

If you notice that the ‘Save’ button is grey and inactive, this means you will have to request permission from the Editor to make changes to your submission or ask them to make the changes for you.

To learn more about creating metadata, see [the Better Practices in Journal Metadata guide](https://docs.pkp.sfu.ca/metadata-practices/en/).

<hr />

### Responding to a Review {#responding-to-a-review}

> **Video:** [Video of Responding to Reviews in OJS](https://www.youtube.com/watch?v=LR_1BmmSTek)
This PKP School video explains how an editor responds to a review and how an author can upload revisions. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDUKJbWtr4bgy133_jwoiqoF).

Once the review process has completed, you will be notified via email by the editor of their decision.

After receiving the email with the decision, login to your dashboard. Select the manuscript you have been notified about.

![Submission dashboard with items in review](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-auth-responding-revisions.png)

Within the Review tab of the manuscript, you will also see a copy of the Editorial Decision under Notifications. Depending on the type of peer review the journal uses, you may see less information on the Review tab of the journal. The example below shows an open peer review which allows authors to see who the reviewer was.

![Review tab of manuscript](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-auth-responding-revisions2.png)

To view the Editorial decision, click the link under notifications.

![Editor decision notification](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-auth-responding-revisions3.png)

Based on the information in the editor's message, you must now prepare your revisions.

#### Uploading the Revised File

Once you’re ready to upload the revised file, scroll down the page and find the panel for **Revisions**.

![Revisions panel](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-auth-responding-revisions4.png)

Use the *Upload a File* link to upload your revised manuscript.

![Upload review file](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-auth-responding-upload.png)

Use the dropdown menu to choose that you are uploading a revision of an existing file.

Then upload the revised file and hit **Continue**.

![Review file details and continue](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-auth-responding-upload2.png)

Check the file details and hit **Continue** again.

![Add another file or complete upload](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-auth-responding-upload3.png)

If you have any additional files to upload, do so now. Otherwise, hit **Complete**.

Your revised file is now visible in the Revisions panel.

![Revised file now in revisions panel](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-auth-responding-upload4.png)

#### Inform the Editor

The editor will receive a notification about the new file(s) being uploaded. Additionally you can inform the editor via the Review Discussion panel as explained below.

![Review discussions panel](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-auth-responding-discussion.png)

From there, select the *Add Discussion* link.

Select the users you want to notify under Participants.

![Add discussion and select participants](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-auth-responding-discussion-add.png)

Add a subject line and a message.

Hit **OK** to send the message.

An email has now been sent to the editor and you (and the editor) can see the message in the Review Discussions panel.

![Message in review discussions panel](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-auth-responding-discussion-panel.png)

At this point, the author needs to wait to hear back from the editor as to whether the revisions are acceptable.

#### Revisions Accepted

You will receive an email that your revisions have been accepted.

In addition, notifications will appear on your dashboard.

![Notifications in dashboard](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-au-notifications.png)

The notifications show up in order of date, meaning the most recent one will be on the bottom. Click on it to open the message (which is the same as the email you would have also received).

![Notification message](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-notifications2.png)

Use the **X** in the upper right corner to close the window.

Further down your dashboard, you will also see a discussion reply from the editor.

![Discussion reply in review discussion panel](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-rev-discussions.png)

Clicking the discussion title will open it up.

![Review discussion message](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-rev-discussions2.png)

Congratulations! You've been accepted and your submission file is moving on to the Copyedit stage.

<hr />

### Resubmitting for Review {#resubmitting-for-review}

If the editor’s decision is to resubmit for review, you will need to log in and select the article in your submissions page. The resubmission is done in the review stage, there is no need to start a new submission.

At the review stage you will need to do two things to resubmit once you have revised your document:

Upload the new file in the revisions section. To upload a new file click on ‘Upload file.’ A new window will open allowing you to upload your file(s). Select the appropriate option from the dropdown menu to indicate you are submitting a revision of an existing file.

Add a discussion to notify the editor that you have re-submitted.

The peer review process will be repeated, and you will likely receive additional revisions to make. Once these are completed and accepted, you will then be moved to the next stage.

<hr />

### Responding to a Copyediting Request {#responding-to-a-copyediting-request}

> **Video:** [Video of Copyediting in OJS](https://www.youtube.com/watch?v=uc272bhGfeU) 
This PKP School video explains the copyediting process, including how an editor can respond to a copyediting or proofreading request. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDUKJbWtr4bgy133_jwoiqoF).

The next step in the workflow is to inspect your submission files that have been copyedited.

You will receive an email indicating that files are available. To see them, login to the journal and go to your dashboard.

![Author submission dashboard](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-copyedits.png)

You can see your entry in the My Authored panel. Select the Copyediting link to go to the full submission record, including the notification in the Copyediting Discussions panel.

![Copyediting section of author dashboard](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-copyedits-notice.png)

Click on the linked discussion to open it, read the message, and open the attached file.

![Copyediting check discussion message](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-copyedits-message.png)

Once you have read the attached file, you can respond to the copyeditor indicating any required changes or your approval.

![Respond to copyediting check message](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-copyedits-reply.png)

If needed, you could attach a revision, but for this example we will simply approve the changes and hit **OK**.

On your dashboard, you can see that you were the last person to reply to the message.

![Dashboard showing copyediting discussions](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-copyedits-final-dash.png)

Your role in the copyediting process is now complete and you can wait for the request to proofread the final galleys (e.g., PDFs, HTML, etc.) before publication.

<hr />

### Responding to a Proofreading Request {#responding-to-a-proofreading-request}

The next step in the workflow is to inspect your submission files that have been converted into galleys (e.g., PDF, HTML, etc.).

You will receive an email indicating that files are available. To see them, login to the journal and go to your dashboard.

![Author submission dashboard](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-production-dashboard.png)

You can see your entry in the My Authored panel. Select the Production link to go to the full submission record, including the notification in the Production Discussions panel.

![Production section of author dashboard](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-production-record.png)

Click on the linked discussion to open it, read the message, and open the attached file.

![Galley ready for proofreading message](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-production-message.png)

Once you have read the attached file, you can respond to the Layout Editor indicating any required changes or your approval.

![Respond to Galley ready for proofreading message](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-production-message2.png)

That's it! Your role in the editorial workflow is now completed.

> **Original chapter:** [Authoring](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/authoring)

---

## Reviewing

> **Video:** [Video of the Reviewer's Steps in OJS](https://www.youtube.com/watch?v=CINhUa35Jic)

This PKP School video explains how to review an article in OJS. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDUKJbWtr4bgy133_jwoiqoF).

As a reviewer, you will learn of the review request via email or by checking your dashboard:

![The assigned submissions queue in reviewer dashboard](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-rev-dashboard.png)

From the My Assigned list, find the title and Review link. Notice the lack of any author information in this Anonymous Reviewer/Anonymous Author peer review process.

Selecting the Review link will take you to the first review step in the submission record, which is much more limited than the editor’s view, and contains no author information.

![A review request](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-rev-step1.png)

This first step consists of the following sections:

**Request for Review**: provides some text inviting you to act as a reviewer.

**Article Title**: provides the title of the article.

**Abstract**: provides the abstract text.

Further down the screen, you will find additional information.

![More of the review request screen](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-rev-step1-3.png)

The **View All Submission Details** link will open a window with additional information, including all of the non-author metadata:

![The view all submission details screen](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-rev-step1-2.png)

Note that none of these fields are editable by the reviewer, and are only provided to help you conduct a thorough review.

Close this window and move further down the screen. From here you can see the Review Schedule, including all of the relevant due dates.

From here, you can decline or accept the review. If you decline, you will be dropped from the process. If you accept, you will move to review step 2, where you would be able to read any reviewer guidelines provided by the journal.

![The reviewer guidelines](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-rev-step2.png)

Hit **Continue** to move to step 3. From here you can download a copy of the review files and enter your review comments. The first window is for comments to the editor and the author; the second window is just for the editor.

![The download and review tab](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-rev-step3.png)

Once you have read the paper and added your comments, scroll down the page to optionally upload a marked up copy of the review file (remember to strip any personal identification from the file before uploading it).

![The upload reviewer files and review recommendation drop down](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-rev-step3-1.png)

Next, you must then make your recommendation using the dropdown menu.

Your choices include:

**Accept Submission**: it is ready to go to Copyediting as is.

**Revisions Required**: it requires minor changes that can be reviewed and accepted by the editor.

**Resubmit for Review**: it requires major changes and another round of peer review.

**Resubmit Elsewhere**: it doesn’t seem like a good fit for the focus and scope of this journal.

**Decline Submission**: it has too many weakness to ever be accepted.

**See Comments**: if none of the above recommendations make sense, you can leave a comment for the editor detailing your concerns.

Finally, hit the Submit Review button to complete your task. You’ll be asked to confirm.

![The confirmation screen to submit review](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-rev-step3-2.png)

Hit OK. You will be taken to the final confirmation screen thanking you for your work.

![The review submitted completion screen](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-rev-step4.png)

That's it! The review is now complete.

> **Original chapter:** [Reviewing](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/reviewing)

---

## Editorial Workflow

In this chapter, you will follow a submission throughout the workflow, from first submission to final publication.

> **Video:** [Video of Editorial workflow in OJS 3.3. Module 2: Editorial Workflow Overview](https://www.youtube.com/watch?v=K-qjxN7rOJs)

This PKP School video provides an overview of the editorial workflow in OJS 3.3. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDUKJbWtr4bgy133_jwoiqoF).

The workflow is divided into 4 stages:

**Submission**: This is where new submissions land while being assigned to Section Editors and considered for moving into the Review stage.

Some submissions are clearly inappropriate and never make it beyond this stage.

> **Video:** [Video of Editorial workflow in OJS 3.3. Module 4: Responding to a submission](https://www.youtube.com/watch?v=9rx-AahCU10)

This PKP School video explains the steps the Editor takes to assign a new submission to a Section Editor. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDUKJbWtr4bgy133_jwoiqoF).

**Review**: This is where the peer review happens, as well as any revisions required by the author.

Some submission will not pass review and end here. Those that are accepted move to the next stage.

**Copyediting**: Accepted articles move to this stage, where they are improved by the work of a copyeditor. Authors can be given the opportunity to review the copyedits.

**Production**: Once the copyedits are completed and approved, the submission moves to this stage. In Production, the copyedited files are converted to galleys -- HTML, XML, PDF, etc. Again the author has the opportunity to proofread the galleys. Once everyone is satisfied, the submission is scheduled for publication in a future issue.

> **Video:** [Video of Editorial workflow in OJS 3.3. Module 9: Production.](https://www.youtube.com/watch?v=-VRKdBQPdn4)

This PKP School video explains the Production stage. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDUKJbWtr4bgy133_jwoiqoF).

<hr />

### Tasks {#tasks}

Your Tasks are available from the top left menu of your Dashboard. Note the number "1" in the image below. This indicates that there is currently 1 task in your list.

![The expanded Tasks menu in OJS.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-tasks.png)

Tasks provide a quick look at items that need your attention. Bold entries are unread, and unbold entries have been read.

Use the checkbox to mark tasks for deletion \(the link is available at the bottom of the list\).

<hr />

### Submission Notifications {#submission-notifications}

When an author makes a new submission to your journal, the author and all contributors will receive an email acknowledging their submission and an editor will be automatically emailed a notification of the new submission. In some cases an editor will be automatically assigned to the submission. Which editor(s) receive the notification or are automatically assigned will depend on how you have set up your journal (see [Edit a section](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/journal-setup#edit-a-section)). 

* If there is only one user assigned to an Editor or Journal Manager role, that user will be automatically assigned and notified. 
* If one or more Section Editors are assigned to the [section](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/journal-setup#sections) the submission was made in, they will be automatically assigned to the submission and notified.
* If one or more Section Editors are assigned to a [category](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/journal-setup#categories) the submission was made in, they will be automatically assigned to the submission and notified.

You can also configure OJS so that a copy of the notification email is sent to the journal’s primary contact set in Journal Settings, or to another address.

To enable copies of submission acknowledgment email to be sent to the primary contact or another address:

1. In the Journal Manager’s dashboard, go to Settings > Workflow > Submissions
2. Scroll down to Notification of Author Submissions
3. Check off the box next to “Send a copy to the primary contact, identified in the Journal Settings.” if you wish for a copy to be sent to the primary contact email, and/or
4. Enter the email you would like to have a copy sent to in the text field.

![The Notification of Author Submission settings in OJS.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-configure-submission-notification.png)

If you want to disable submission acknowledgement emails entirely, you can do so by disabling the *Submission Ack* email template from the list of prepared email templates. To learn more about disabling and enabling email templates, refer to *Disable email templates* in the [Workflow Settings chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-workflow).

Users can also change their individual notification settings from their own profile under View Profile > Notifications.

### Submission Dashboard {#submission-dashboard}

When you log into your Dashboard, you can find active submissions either from your Tasks, or from one of the queues (My Queue, Unassigned, All Active, and Archives). The counter gives you an overview of how many total items are in each queue.

![The submission dashboard in OJS.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-dashboard-active.png)

#### My Queue

**My Assigned**: This panel includes submissions added to sections where you are a section editor or to your own submissions if you are also an author with this journal.

The **Search** tool for each queue can sometimes be helpful in tracking down submissions.

The **Filter** tool allows you to limit your browsing to specific conditions for faster searching. Depending on their role, editorial roles will be able to filter by the following:

- __Status:__ select from _incomplete_, _overdue_, and _inactive for 30 days_

- __Stages:__ select from _submission_, _review_, _copyediting_, and _production_

- __Sections:__ this option is only available if more than 5 sections exist. After you begin entering text, the filter will auto-suggest. For example, filter by _articles_ or _reviews_

- __Assigned editor(s):__ only Journal Managers and Journal Editors have this filter option. Like sections, this is a textbox which will auto-suggest a Section Editor, Journal Editor, or Guest Editor's name as you start to type it, then display all articles assigned to the editor.

- __Assigned issue:__ only journal managers can filter by unpublished issues, but editors and assistants will be able to filter by published issues. This field is case-sensitive and require exact match. For best results, search by year or title, rather than volume or number. This filter is mostly used if the assignment of a submission to an issue is done in an early phase of the editorial process. 

Some filters allow multiple selections; users can filter by more than one editor, section or issue. Filters are applied with OR conditions, so when a user selects to filter by Editor A and Editor B, all submissions will be returned that are assigned to editor A OR editor B.

When using multiple filters, the AND condition will be applied between filters. For example, when filtering by Review Stage AND Editor A, only submissions assigned to Editor A in the review stage will be returned.

![A sample filter applied to the list of submissions.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-dashboard-filter.png)

Note that you can use the blue arrows to the right of each submission to reveal more details, including how many reviews are outstanding, new discussions, and more. It also reveals buttons to take you to the submission record, view the activity log and notes, and to delete the submission.

![A sample of expanded submission details in the dashboard.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-dashboard-active-details.png)

#### Unassigned

This panel includes submissions added to sections without section editors.

![The Unassigned tab in the Submissions dashboard.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-dashboard-unassigned.png)

In the above example, there are no unassigned submissions, so the panel is empty.

#### All Active

This section includes a list of all submissions, without being organized into queues.

![The All Active tab in the Submissions dashboard.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-dashboard-all-active.png)

#### Archives

This section includes a list of all submissions either declined or already published by the journal. Declined submissions may be deleted from the list of archived submissions. Deleting a declined submission will completely remove the submission and all submission files from your journal.

![The list of archived submissions with the option to delete submissions.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/ojs-3.3-sub-delete.png)

#### Demonstration Submission

For this demonstration, we are looking at the Cerpa submission, entitled _A Review of Object Oriented Database Concepts and their Implementation_. It can be found at the top of the **My Assigned** queue, as well as in the **All Active** queue.

![The My Assigned queue on the OJS Submissions Dashboard, with the example article by Cerpa at the top of the queue.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-submission-queue.png)

Once you find the submission, you can use the view button to view the submission, or use the blue arrow to reveal options and see if there are any open discussions (there are none in this case), the number of production galleys, and access the activity log & notes.

![A submission with the options menu expanded.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-submission-options.png)

**Activity Log & Notes** will bring up the submission's history.

![A sample activity log for a submission](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-dashboard-log.png)

Use the Notes tab to also view or add any editorial notes.

![The Notes tab of the Activity log.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-submissions-notes.png)

#### Submission Record

To view the submission in more detail, select **View Submission** button. This will take you to the submission record.

![A sample submission record.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-dashboard-record.png)

From here, you can see:

**Submission Files**: This panel lists the files that have been submitted. In this view, there is just one file, but multiple files could have been submitted. Submission files will now retain the original names when downloaded.

For journals using anonymous review, the author and reviewer (if they were to upload any document) are still removed. An example filename structure for files downloaded by Reviewers will be `ojs-review-assignment-1-article-text-8.docx` The numeric number corresponds with the manuscript number of assignment.

**Pre-Review Discussions**: This panel allows the editor to communicate with the author, or with others on the editorial team. For example, to ask the author for some additional information, or to ask a section editor to take responsibility for this submission.

**Action Buttons**: These include Send to Review, Accept and Skip Review, and Decline Submission.

> Note: If you don't see these buttons, you likely have not yet assigned the submission to an editor.

**Submission Status** Once an editor has recorded a decision in one stage of the workflow of OJS 3.2, the recorded decision will appear in place of the decision buttons. Editors will still have the ability to change the recorded decision by clicking, ‘Change Decision’ this will enable the 3 options once again.

![The Change Decision button in the submission status.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2_edflow_decisionstatus2.png)
*The screenshot above shows the decision button for MS# 425 prior to a decision being recorded. The screenshot below shows the notification of the recorded decision.*

![The "Submission accepted" status of a submission.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2_edflow_decisionstatus_accept.png)

**Participants**: This panel is where you will see the list of participants involved in the submission, including the editor, section editors, and author. Other names (copyeditors, layout editors, etc.) will appear here as they are added in subsequent steps.

**Submission Library**: The Submission Library is a general storage area for documents that may include conflict-of-interest forms, galley approval forms, etc. A user can upload the completed form for their manuscript in their Submission Library. The uploaded forms will also be available to other participants (with the exception of Reviewers) assigned throughout the editorial or production workflow to edit or re-upload new versions.

**Document Library**: Users throughout the editorial workflow will be able to access all the files in the Publisher Library (see [Workflow Settings chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-workflow)) made available by the Journal Manager or Editor through opening the Submission Library and clicking "View Document Library".

![The location of the View Document Library button in the Submission Library panel.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-settings-workflow-sublib1.png)

**Preview**:  See how the submission will look when published with its current metadata and Galley files by clicking Preview.

![The preview feature that shows how an article will look when published](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-preview.png)

**Metadata**: Where you can view and revise the submission metadata. In OJS 3.2 and later, users can be granted permission to revise certain submission metadata at any stage of the workflow.

![The Metadata tab of a submission.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-dashboard-record-metadata.png)

#### Granting Author permissions

As of OJS 3.2, editors can grant access to allow authors to make metadata changes.
There are two ways editors can grant this type of access.

**Global permission**- will grant all users with the role ‘author’ permission to make metadata changes.

To enable this, go to Users & Roles > Roles. Click the blue arrow beside the ‘Author’ then click edit.

![The location of the Edit button under the Author role.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-editorial-workflow-author-edit.png)

Under Role Options, enable ‘Permit submission metadata edit.’ then click OK.

![The "Permit submission metadata edit" checkbox in the role editing window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-editorial-workflow-author-editmenu.png)

**Limited Permission** - will grant registered authors (typically a single author) permission to only make changes at certain stages of the editorial workflow.

To allow an author to change the metadata at a specific stage of the workflow, click on the workflow stage (ie., Submission, Review, Copyediting, or Production).

Under the participants list, click the arrow beside the author’s name followed by Edit.

![The location of the Edit button for a participant in the participants list.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-editorial-workflow-edit-participant.png)

Under Permissions, enable ‘Allow this person to edit publication details.’ followed by OK.

![The "Allow this person to edit publication details" checkbox in the Edit Assignment window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-editorial-workflow-edit-grantpermission.png)

Once the author has been granted access to made edits they will be able to make changes to the following sections on the Publication tab: Title & Abstract, Contributors, and Metadata.

![The sections available for authors to edit highlighted in the Publication tab.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-editorial-workflow-edit-publicationmenu.png)

#### Assigning the Submission

Depending on [how you have your sections configured](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/journal-setup#edit-a-section), some new submissions may come in unassigned. If this is the case, the next step is to assign an editor or section editor. To do so, select the _Assign_ link in the **Participants** panel.

![The Add Participants window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-submissions-add-participant.png)

You will have the option to locate a user by role, choose an individual, and send them a message requesting their assistance.

> Note: If you aren't sure of the names of the section editors, simply choose that role from the dropdown menu and then hit the Search button. All Section Editors will be displayed and available for selection.

Hit the **OK** button to make the assignment and send the message.

![The added participants name shown in the participants list.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-dashboard-record-assign.png)

> Note the new Pre-Review Discussion that was automatically created as part of the assignment.

You can now see that the Section Editor is listed under Participants, and the Action buttons are available:

**Send to Review**: Moves the submission on to the next stage.

**Accept and Skip Review**: Skips the Review Stage and moves the submission directly into Copyediting.

**Decline Submission**: Rejects the submission before going through the review process. The submission would then be archived. In OJS 3.3, there is now the option to revert a Decline decision in the Submission and Review stage. This can be done by clicking **Change Decision** followed by **Revert Decline**. After a declined decision is reverted, the submission is restored to its previous stage and review round if active.

Although in this example, the editor assigned a section editor, it would also be possible for the editor to assign themselves to the submission.

Once the editor has selected an action, the submission status will change and the action buttons will be disabled.

![The location of the Change Decision button of a submission.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2_edflow_decisionstatus2.png)

#### Section Editor

Now that the Section Editor has been assigned, they can login and view their dashboard. The submission can be found at the top of the My Assigned queue.

![The My Assigned queue of a Section Editor with assigned submissions.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-se-dashboard.png)

Clicking on the article title opens the full submission record.

![A sample submission record.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-se-record.png)

##### Accepting the Assignment

It is not required, but the Section Editor could reply to the Pre-Review Discussion to inform the editor that they will be proceeding with the assignment.

##### Communicating with the Author

If the Section Editor has any questions for the author, they can use the Pre-Review Discussions.

##### Sending to Review

Once the Section Editor is satisfied that the submission is appropriate for the journal, they can select the **Send to Review** button to move the submission to the next stage.

![The Send to Review confirmation window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-se-record-sendReview.png)

Keep the files that are to be reviewed checked off.

<hr />

### Review {#review}

> **Video:** [Video of Editorial workflow in OJS 3.3. Module 5: Assigning a reviewer.](https://www.youtube.com/watch?v=5Hwkqj4Jvew)

This PKP School video explains the steps the Section Editor takes to assign reviewers to the submission. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDUKJbWtr4bgy133_jwoiqoF).

When the submission enters the Review Stage, a notification indicates that Reviewers need to be assigned.

![The "Waiting for reviewers to be assigned" notification.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-se-record-revstage.png)

> Note: In the screenshot above, we see the Section Editor's view. Notice the limited Action buttons \(only Make Recommendation is available\). If we were logged in as an Editor, we would see more Action buttons \(Request Revision, Accept Submission, Decline Submission\).

From the Reviewers panel, you can select Add Reviewer to assign a new Reviewer.

This opens a new window, where Reviewers are listed and can be selected one at a time.

![The Locate a Reviewer window listing all Reviewers.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.1.2-locate-reviewer.png)

Clicking on the blue arrow reveals more information about their review history, including how many active reviews they are currently assigned, how many reviews they have completed or declined, etc. If the user has added a Biography or Reviewing Interests, this information will be displayed here.

Additionally, a Journal Editor can add an Editorial Note about the reviewer in their profile under Users & Roles > Users. This note will appear in the reviewer details on the Add Reviewer screen, but will not be visible to the reviewer or to the public.

![A sample of expanded reviewer details with review history and notes.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.1.2-add-reviewer.png)

In OJS releases 3.0 to 3.1.0, you cannot assign a user to review a submission if they are also an editor of the submission.  If you do, the editor will no longer be able to access the submission after they submit their review, in order to maintain the principles of anonymous peer review. However, starting with OJS 3.1.1, you can assign a user to review a submission if they are also an editor of the submission.

At the bottom of this form, you will see options to:

**Select Reviewer**: Use this to confirm your selection once you have picked a Reviewer from the list.

**Create New Reviewer**: If none of the Reviewers are suitable, you can use this button to create a new Reviewer. This is a new account in the system.

**Enroll Existing User**: If none of the Reviewers are suitable, you can enroll an existing user as a Reviewer.

For this demonstration, we will pick Adela as our Reviewer and hit the **Select Reviewer** button.

This initiates a new window with a message for the Reviewer.

![The Add Reviewer screen with email notification template.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-se-record-revstage-revreq.png)

You can revise any of the prepared text.

If you are using an Anonymous Review method, ensure that the files you send to the Reviewer are stripped of any identifying information about the Author. Additional instruction for this is provided in the [Understanding Different Types of Review](#understanding-different-types-of-review) and [Removing Identifying Information](#removing-identifying-information) sections.

Further down the form, you will see the additional details that are sent to the Reviewer including title, abstract, important dates, and a link to the files to be reviewed.

![Review details include type and due date settings.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-rev-add-4.png)

By default, Reviewers will be provided with an extended text box to type in their comments. However, the Journal Manager can create Review Forms in [**Workflow Settings &gt; Review**](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-workflow#review) to ask more focused questions. If you would like the Reviewer to fill out a review form, select it under **Review Form**.

Hit the **Add Reviewer** button to send the message and assign the Reviewer.

Back on the Review Stage, we can see the Reviewer is now listed.

![The newly added Reviewer seen in the Review Stage.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-rev-reviewer-added.png)

You can make additional changes using the blue arrow toggle next to the Reviewer's name.

![Expanded reviewer details and options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-rev-reviewer-added-2.png)

**Review Details**: Provides details on the review.

![The Review Details window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-rev-reviewer-review-details.png)

**Email Reviewer**: Allows you to send a message to the Reviewer.

![The Email Reviewer window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-rev-reviewer-email-reviewer.png)

**Edit Review**: Allows you to change the review dates and files.

![The Edit Review window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-rev-reviewer-edit-review.png)

**Unassign Reviewer**: Allows you to unassign the Reviewer.

**Cancel Review Request**: As of OJS 3.2, you can cancel a review request. This may be necessary when a reviewer has not responded to a review request or accepted to do a review but never delivered.

![The Cancel Reviewer option in the expanded Reviewer options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-cancel-reviewer.png)

Cancelling a review request will permit you to send a template email to the reviewer. The request will then show up in the editor's reviewer list as "cancelled".

![A sample review request marked "Request cancelled".](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-reviewer-cancelled.png)

Cancelled review will be recorded in reviewer stats that you can see when selecting a reviewer.

![Cancelled requests as seen in a reviewer's stats.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-cancelled-reviews-tracker.png)

**Review Discussion**: Review Discussion is another way for you to contact a reviewer. In a review discussion, you have the option to attach files.

To start a discussion, click ‘Add Discussion.’

![The location of the Add Discussion button.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-rev-contact2.png)

You will then select the reviewer(s) you would like to start a discussion with.

![The list of reviewers to select for discussion.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-rev-contact3.png)

**History**: Provides a brief history of the review.

![The review History window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-rev-review-history.png)

At this point, we could add additional Reviewers, and then wait for their recommendations to come in.

#### Understanding Different Types of Review

OJS is designed to accommodate different types of reviews and has built-in steps to ensure anonymity.

All information will be visible to the journal managers and editors regardless of the type of review selected.
The review type will be automatically selected based on what has been configured under _Settings_ > _Workflow_ > _Review_. The editors can change the review type when sending the review request. Editors/Section Editors must select the review type when sending the review request from the following options:

* Anonymous Reviewer/Anonymous Author
* Anonymous Reviewer/Disclosed Author
* Open

**Anonymous Reviewer/Anonymous Author**: The identity of both the author and the reviewer is kept hidden.

The author or editor must ensure that metadata from the manuscript file is removed in Anonymous Reviewer/Anonymous Author. See [Removing Identifying Information](#removing-identifying-information) for more information.

*Reviewer*: The reviewer will not be able to see the author(s) in their reviewer’s queue if the editor has selected Anonymous Reviewer/Anonymous Author. All identifying information in the metadata of the submission details is automatically removed by the system, as seen in the example below.

![A sample of the metadata a reviewer will see in a double anonymous review - no identifying information is included.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-rev-anon1.png)

At the end of a review, if a reviewer chooses to upload a review file they should remove all identifying information before uploading it to the system. See [Removing Identifying Information](#removing-identifying-information) for more information.

*Author*: No identifying information regarding the reviewer will be visible to the author within their manuscript view.

![A sample of what the author will see after their submission is reviewed - no identifying information is included.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-rev-anon2.png)

*Editor's Decision*: The decision email sent to the author(s) at the end of a review will have generic titles of the reviewers.

![A sample decision email identifying the reviewer only as "Reviewer A".](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-rev-anon3.png)

**Anonymous Reviewer/Disclosed Author**: Reviewer identity is kept anonymous from the author(s). The reviewers can see the author details.

*Reviewer*: The reviewer is able will see full the metadata entered by the author by clicking _View All Submission Details_ in the request tab of the manuscript. The authors’ name will also appear in the reviewer's queue.

*Author*: No identifying information regarding the reviewer will be available within their manuscript view.

![A sample of what the author will see after their submission is reviewed - no identifying information is included.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-rev-anon2.png)

*Editors Decision*: The decision email sent to the author(s) at the end of a review will have generic titles of the reviewers.

![A sample decision email identifying the reviewer only as "Reviewer A".](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-rev-anon3.png)

**Open Review (Disclosed Reviewer/Disclosed Author)**: The identities of both the author and the reviewer are known to each other. Although it is relatively new and less common in scholarly publishing, there are [several compelling reasons](https://digitalpublishingworkshop.com/journal-publishing/new-perspectives-on-peer-review/#how) for journals to opt for an open review process. We advise journals to make their review policies clear and transparent; some examples of such policies:

- [In the Library with the Lead Pipe: an open access, open peer-reviewed journal](https://www.inthelibrarywiththeleadpipe.org/about/)
- [Intersectional Apocalypse](https://journals.lib.sfu.ca/index.php/ifj/reviewpolicy)

*Reviewer*:  The reviewer will be able to see the author’s name if they click on “View All Submission Details.” They do not need to accept the review request, in order to see this information. The reviewer can make their decision on whether they want to review a manuscript, with knowledge about the author’s identity.

![Open Review Reviewer assignment window for editors.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-ed-rev-open1.png)

*Author*: The author can also see the reviewer’s name, but only after the reviewer has accepted the request. The author cannot see the assigned potential reviewer(s).

![Open Review dashboard shown to authors.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-ed-rev-open2.png)

*Communications*: Since the review is open, authors and reviewers can communicate with each other using the discussion feature. Even if they don’t include the editor as a “participant” to the discussion, editors can always view discussions. 

The author, reviewer, and editor can all see messages between reviewer and author.

![Example of Open Review discussion window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-ed-rev-open3.png)

*Editor*: Like other types of reviews, editors can see all activities.  Additionally, the reviewer has the option of leaving messages exclusively for the editor.  Authors cannot see notes submitted under “For editor only.”

![Example of Open Review’s reviewer comments.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.3-ed-rev-open4.png)

Since identities are not secret, it is not necessary to follow steps under [Removing Identifying Information](#removing-identifying-information).

#### Removing Identifying Information

While OJS has a number of built-in functions for anonymous reviews, additional steps may need to be taken outside of the platform to ensure Anonymous Reviewer/Anonymous Author. A submission file may have information that could identify the authors' identity within the document properties.

![A sample of a document whose author is visible within the document properties.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-rev-anon4.png)

Authors may also include their name within the article, footnotes, or references, in which case the editor will have to remove it prior to sending for review. Alternatively, authors can be asked to redact their names from the submission file, with "Author" and year used in the references and footnotes instead of the authors' name, article title, etc., prior to submission.

##### Microsoft Word for Windows

1. Go to _File_
2. Select _Info_
3. Click on _Check for Issues_
4. Click on _Inspect Document_
5. In the _Document Inspector_ dialog box, select the check boxes to choose the types of hidden content that you want to be inspected
6. Click _Remove All_
7. Click _Close_
8. Save the document

##### Microsoft Word for MacOS

1. Go to _Tools_
2. Click _Protect Document_
3. Select _Remove personal information from this file on save_
4. Click _OK_ and save the file

![The "Remove personal information from this file on save" option in Mac OS.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-rev-anon5.png)

#### Re-uploading the Document

The Journal Managers and Editors are able to re-upload the anonymized document in the Review files by clicking **Upload/Select Files** in the _Review Files_ box.

![The Upload/Select Files button under the Review Files section.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-rev-anon6.png)

Click **Upload Review File**.

![The Upload Review File button.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-rev-anon7.png)

Identify the article component and upload the file.

![The article component identification dropdown.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-rev-anon8.png)

Review Details. It may be helpful to rename the file to the time of re-upload. The file can also be renamed by clicking the arrow on the left side of the file name.

![The Edit button in the expanded menu under the list of review files.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-rev-anon9.png)

Click Complete and select the file you would like to use for the review.

The file(s) will appear under the initial upload.
When sending out the review request, ensure that the original manuscript is unselected from the ‘Files To Be Reviewed’.

![Options to toggle which files are included for review.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-ed-rev-anon10.png)

Select the Review File(s) and click **OK**.

#### Responding to Reviews

> **Video:** [Video of Editorial workflow in OJS 3.3. Module 7: Responding to the reviews](https://www.youtube.com/watch?v=LR_1BmmSTek)

This PKP School video explains the steps the Section Editor and the author take once the reviews are complete. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDUKJbWtr4bgy133_jwoiqoF).

Once the Reviewers have completed their work, the Section Editor can see the results in their dashboard. Here they will see notifications that new reviews have been submitted and whether all reviews are in.

![Sample notification of completed reviews in the Section Editor's dashboard.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-rev-responding.png)

Use the _Read Review_ link in the Reviewers panel to read the comments from the Reviewers, including those for both the Author and Editor as well as for the Editor only.

![A sample review with comments.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-rev-read-reviews.png)

Select the _Confirm_ link at the bottom of the screen.

![The Review Confirmed status applied to a review.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-rev-thank.png)

In the Reviewers panel, you can now see a _Thank Reviewer_ link. Choose that to thank the Reviewer.

![The Thank Reviewer window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-rev-thank2.png)

Hit the **Thank Reviewer** button to send the message.

#### Making the Decision

Based on the Reviewer recommendations, you can use the action buttons to make a decision.

![The various action buttons for making a decision regarding a submission.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-rev-decision.png)

Options include:

**Request Revisions**: This will require the Author to make minor changes, the editor has the option to select whether another round of review will be required.

**Accept Submission**: This means the submission is accepted without revisions and can proceed to the Copyediting stage.

**Decline Submission**: This means that the submission has not passed peer review and is unsuitable for further consideration. The submission would then move to the Archives. Only declined submissions in the Archives can be deleted. In OJS 3.3, there is now the option to revert a Decline decision in the Submission and Review stage. This can be done by clicking **Change Decision** followed by **Revert Decline**. After a declined decision is reverted, the submission is restored to its previous stage and review round if active.

#### Request Revisions

In this demonstration, we are going to request that the Author make some minor revisions before acceptance.

To do so, select the **Request Revisions** button. This results in a new message window.

![The Request Revisions window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-rev-req-revisions.png)

You can modify any of the text before sending the message.

Use the **Add Reviews** button to import the Reviewer's comments from the Editor and Author field. Comments in the Editor only field will not be displayed.

If there are any attachments, such as a marked up file created by a Reviewer, you can attach it here (as long as it has been anonymized).
In OJS 3.1.2 and later, you can also upload a new file and add it as an attachment.

Hit the **Record Editorial Decision** button to send the message.

![A sample request for revisions with imported comments and options to share files.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-rev-req-revisions3.png)

You must now wait for the Author to respond with their revisions.

#### Author Responds

Once the Author has made the revisions, you should receive a message (via email and the Review Discussions panel).

![The author's revision found in the Review Discussions panel.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-discussion-panel.png)

You will also see the revised file in the Revisions panel.

At this point, you can download the revised file, check to make sure it is ready, and communicate with the Author using the Review Discussions panel.

In this case, we're going to inform the Author that we are accepting the revisions. To do so, click on the linked title of the discussion. This will open the discussion box.

![An expanded discussion.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-discussion-window.png)

Use the **Add Message** button to reply, either requesting further revision or informing the author that the submission is ready to move on to the next stage.

![A sample reply to an author's revisions.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-discussion-window-reply.png)

#### Additional Round of Review

If you would like to put the revised article through another round of review, you can start a second (or third or subsequent) review round after the author revisions have been received.

It is best to start a new round of review **after** an author uploads revised files on the previous round. Creating a New Round of review before the author has uploaded their files could create some confusion as their dashboard (and yours) will default to the new round. The author will, however, be able to switch back to Round 1 to upload their files. This will also result in having to download the uploaded file from Round 1 and upload it into Round 2.

A new round should **not** be started if you are experiencing any issues with the current round (i.e., unable to record decision, re-invite a declined or removed reviewer).

To start an additional round of review after revised files have been received, click the **New Review Round** tab in the review tab of the manuscript.

![The New Review Round button in the Review panel](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-new-round-1.png)

This will open another menu for you to select which files (provided by the author) to include for the new round of review.

![File selection options for a newly created review round.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-new-round-2.png)

If there are any additional files you want to make available again from the previous round, this can be done by clicking **Upload/Select Files**. 

![The Upload/Select files button in the Review Files window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-new-round-3.png)

Check the box next to **Show files from all accessible workflow stages**. The files available from Round 1 should appear under Submission. The files that appear under Review will only show files uploaded by the author from the previous round (i.e., revised files from Round 1). If you are on Round 3 (and onwards) and require files from Round 1 or 2, you will need to download these to your local desktop and re-upload them using **Upload/Select Files**.

![The list of files for a submission including previous round after the "Show files from all accessible workflow stages" option is enabled.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-new-round-4.png)

Similarly, if there are any additional files authors provide after they upload the resubmission, you can upload them using **Upload/Select Files**.

A new round will be added to the Review panel in the submission dashboard.

![The Round Two tab in the Review panel.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-new-round-0.png)

Once you’re ready to start the new round of review, assign Reviewers as you did in the previous round. You can assign the same reviewers or different reviewers.

Reviewers from previous rounds will not have access to comments they've made the round before. If a reviewer has requested their comments from the previous round, the editor could copy this from Round 1 - Review Details and start a discussion in Round 2. Alternatively, the journal may choose to encourage the submission of Response to Reviewer as part of the resubmission.

These steps can be repeated until a final decision to accept or decline the manuscript has been reached.

#### Moving to Copyediting

The submission is now ready to be moved to copyediting. To do so, use the blue **Send to Copyediting** button.

![The "Send to Copyediting" button in a submission panel.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-send-to-copyediting.png)

This will open a new window.

![The Send to Copyediting window including information about the notification of acceptance to be sent to the author.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-accept.png)

Note that if the journal has enabled an article processing charge (APC) to be charged to authors, the option will appear at this stage to notify the author that the payment is due. Selecting "Request publication fee" will prompt a payment notification email to be sent to the author with payment instructions. For information about enabling author fees, please see the [Subscriptions chapter > Payment Types](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/subscriptions#payment-types) and [Distribution settings > Enable Payments](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-distribution#enable-payments).

![A sample notification for a journal with APCs enabled.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-subscriptions-authorfees.png)

Hit the **Record Editorial Decision** button at the bottom of the window.

The submission is automatically moved to the Copyediting stage.

Back on the review tab, you will notice that the status now indicates the submission has been accepted.

![The "Submission accepted" status of a submission.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2_edflow_decisionstatus_accept.png)

<hr />

### Copyediting {#copyediting}

> **Video:** [Video of Editorial workflow in OJS 3.3. Module 8: Copyediting.](https://www.youtube.com/watch?v=uc272bhGfeU)

This PKP School video explains the Copyediting stage. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDUKJbWtr4bgy133_jwoiqoF).

When a submission is accepted in the Review Stage, it will automatically move to the Copyediting stage.

![The Copyediting stage of a submission.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-copyediting.png)

#### Adding a Copyeditor

When the submission enters the Copyediting Stage, a notification indicates that a Copyeditor needs to be assigned. Copyeditors can be assigned using the *Add* link on the Participants panel.

This will open a new window.

![The Add Participant window in the Copyediting stage.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-copyediting-add.png)

You can use the role dropdown to choose Copyeditor and hit the **Search** button. This will bring up all Copyeditors.

Select one of the Copyeditors for this submission.

Choose a prepared message.

Make any changes needed to the message.

Hit **Send**.

You can now see the new notification that the submission is awaiting copyedits, the Copyeditor is now included in the Participants list, and the request is visible in the Copyediting Discussions.

![The "Awaiting Copyediting" notification and updated participants list.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ed-copyediting-add-dash.png)

You can now wait for the Copyeditor to do their work.

#### Copyeditor

The Copyeditor will receive an email message from the Section Editor requesting them to take on the submission.

To get started, they must login and find the submission from their dashboard.

![The Copyeditor's submission queue.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-dash.png)

Then, they can click the Copyediting link next to the submission name. This will take them directly to the Copyediting stage for this submission.

![The Copyediting stage as seen by an assigned Copyeditor.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-submission.png)

From here, they can see the Draft Files. These are the files that require copyediting. Clicking on the linked title will download the file to their desktop.

Outside of OJS, they will do the copyediting work.

To check the submission metadata, click from the Workflow tab to the Production tab.

![An article record's Publication tab with metadata fields](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-copyediting-metadata.png)

This would include checking the article title, abstract, contributor names, keywords, etc.

If any changes are made, hit the **Save** button before exiting this window.

You can Preview how the Abstract page would look if published with the current metadata by clicking on the Preview button in the top-right portion of the page.

##### Consult with the Author

Once they have finished copyediting, they will run the changes past the Author by adding a new discussion, using the Copyediting Discussions panel's *Add discussion* link.

From the Add Discussion window, they must choose the Author and add a subject line and message.

![The Add Discussion window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-add-discussion.png)

Further down that same window, they must upload a copy of the copyedited file.

![The file upload area of the Add Discussion window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-add-discussion2.png)

To do so, use the *Upload File* link. This will open a new window where you must choose the *Article Component* (e.g., article text) and upload the file.

![The File Upload screen.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-upload1.png)

Hit **Continue** to proceed.

This will open the next step, where you can edit the filename if needed.

![The Edit option next to the file name.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-upload2.png)

Next, you can upload more files if necessary, or hit **Complete**.

![The Confirmation step of the file upload.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-upload3.png)

Back on the Add window, you can now see the attached file.

![The newly upload file attached to the discussion.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-upload4.png)

Hit **OK** to send the message to the author.

It is now visible in the Copyediting Discussions.

![The discussion added to the Copyediting Discussions section.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-discussion.png)

You can now wait for the author's response.

#### Author Replies

Once you hear back from the author, you can review their feedback by checking the discussion reply.

![The previous Copyediting Discussion now containing a "1" in the reply column.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-se-author-copyedits.png)

From here, you can see no further changes are required.

![A sample reply from an author approving the copyediting.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-se-author-copyedits-reply.png)

#### The Final Copyedited File

Now you can go ahead and upload the final copyedited version to the Copyedited panel, near the bottom of the screen.

![The Upload/Select Files option can be found near the Copyedited section of the panel.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-copyedited.png)

Use the Upload/Select Files link to upload the final copyedited version.

![The Upload/Select Files window.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-copyedited-upload-select.png)

It is important to note here that you have a few choices.

1. You can use the Upload File link to upload a new file (e.g., a file with some recent changes since you showed it to the author).
2. You can select the Author's original version (unlikely).
3. You can select the Copyeditor version, which is the version you sent to the author (if you made no further changes, choose this one).

For this demonstration, we will select the Copyeditor version **by checking the box** to the left of that file.

Hit **OK**.

The file is now visible in the *Copyedited* panel (near the bottom of the screen), indicating to the editor that this is the final version, which is ready for the Production stage.

![The selected file seen in the Copyedited panel.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-copyedited2.png)

#### Inform the Section Editor

The final step is for you to inform the Section Editor that the copyediting is complete.

To do so, start a new Copyediting Discussion by using the *Add Discussion* link.

![The list of Copyediting Discussions ](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-copyedited-final.png)

In the discussion window, add the Section Editor, a subject line, and a message.

![A sample message from the Copy Editor to the Section Editor](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-copyedited-discussion.png)

Hit **OK** to send the message.

Returning to the Copyediting stage, you can see the message is posted.

![The message added to the list of copyediting discussions.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-ce-copyedited-done.png)

Your work as the Copyeditor is now complete!

#### Moving to Production

The Section Editor will receive an email that the copyediting is complete, and see a notification in the discussions.

![The Copyediting Stage in the Section Editor's dashboard](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-se-copyedited-dash.png)

You can download and review the final copyedited version from the Copyedited panel.

![The final copyedited version uploaded to the Copyedited panel. ](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-se-copyedited-files.png)

At this point you could communicate further with the Copyeditor, or, if you are satisfied, move the submission to the Production stage.

To do so, select the blue **Send to Production** button.

This will generate an official notice to the Authors that the submission is moving to the next stage.

![The Send to Production window with notification to the author.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-se-send-to-production.png)

Notice that the appropriate file, from the Copyedited panel, is included and will be automatically transferred to Production.

Hit **Record Editorial Decision** to proceed.

The Copyediting stage is now complete and the submission status will be updated. The next chapter covers the Production and Publication stage.

![The "Sent to production" status.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2_edflow_decisionstatus_copyedit.png)

> **Original chapter:** [Editorial Workflow](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/editorial-workflow)

---

## Production and Publication

With the completion of the Copyediting stage, the submission now moves to Production. From here, the copyedited files will be converted to publishable formats in the form of galley files (e.g., PDF, HTML) and proofread before publishing. A new journal issue will be created and the article will be scheduled for publication in the issue. This chapter explains the steps in that process, as well as how to use the versioning feature (first introduced in OJS 3.2) to publish a new version of an article if significant changes are made.

OJS also offers a straightforward way to bypass the editorial workflow described in the previous chapter and submit content directly into production, where it can be added to an issue and published. You can do this via Quick Submit plugin. See the detailed [Quick Submit plugin instructions under the Data Import & Export chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/tools#importexport).

To start working in Production, the Section Editor or Journal Editor must login to the system and choose the submission from their dashboard.

Clicking on the article will open the submission record.

![Production tab in the editorial workflow of a manuscript.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-se-production.png)

You will see the copyedited files are now available in the **Production Ready Files** panel.

In the **Production** tab, you can assign participants (such as a Layout Editor) to the Production stage of the workflow and communicate with participants in the **Production Discussions** panel.

> **Video:** [Video of Editorial workflow in OJS 3.3. Module 9: Production.](https://www.youtube.com/watch?v=-VRKdBQPdn4)

This PKP School video explains the steps the Section Editor, Production Editor and/or Designer will take in the Production stage and the Publication tab. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDUKJbWtr4bgy133_jwoiqoF).

### Publication Tabs {#publication-tabs}

Everything related to publishing a submission is done under the Publication tab. The Publication tab allows you to edit or add information about the submission, including contributors, metadata, and identifiers. It is also where you will upload the final Galley files for publication in the journal.

![Publication tab that displays metadata information of a manuscript.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-production-publication-tab.png)

Here is an overview of what the different tabs in this section are for. Detailed instructions on some of these are available later in the chapter.

**Title & Abstract**
Use this tab to edit the article title, subtitle, and abstract.

If any changes are made, click Save before exiting this window.

**Contributors**
Use this tab to add, edit, or remove article contributors.

**Metadata**
Use this tab to add or edit article keywords.

If any changes are made, click Save before exiting this window.

**Identifiers**
Use the Identifiers tab to view or add a unique identifier, such as a DOI. More information about assigning and managing DOIs is available in the [DOI Plugin Guide](https://docs.pkp.sfu.ca/doi-plugin/).

**Galleys**
Use the Galleys tab to upload the final file for publication. This is explained below.

**Permissions & Disclosure**
Include details about the copyright holder and link to the article license, if applicable. This will be automatically filled in according to your [Distribution Settings](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-distribution).

**Issues**
Use the Issues tab to assign the article to a journal issue. This is explained below.

#### Multilingual Submissions

The Title & Abstract, Metadata, Permissions & Disclosure, and Issue tabs have options for adding and editing metadata in multiple languages. Languages must first be turned on in Website Settings -> Setup -> Languages.

Select the desired language tab below the “Schedule for Production” button, and complete the metadata fields in the selected language.

![Multilingual button and text fields for French (Canada) in the metadata subtab within Publication.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-prod-metadata-lang.png)

The “Issue” tab allows you to upload multiple cover images in selected languages.

![Multilingual button and upload field for an issue cover image for French (Canada) in the Issue subtab within Publication.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-prod-issue-languages.png)

### Format Article for Publication {#format-article-for-publication}

#### Assign Layout Editor

A notification banner indicates that you must assign someone to create the galley files (e.g., the PDFs, HTML, etc.) from the production ready files.

This can vary from journal to journal – you may have layout editors or production assistants to do this work. Some journals use an external graphic design or typesetting service. If you would like to communicate with your layout editor, production assistant, graphic designer, or typesetter through OJS and manage the production process with them in OJS, ensure they have a user account and add them as a participant to the submission.

To make the assignment, use the **Assign** link in the Participants list. This will open a new window.

![New window to assign participants such as Layout Editor.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-se-production-participants-add.png)

Use the role selector and search button to find appropriate users. Select the user and choose a predefined message, then click **OK** to send.

The user has now been notified via email and in the dashboard.

![Manuscript dashboard after additional participants have been assigned.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-se-production-participants-added.png)

You can now see the Layout Editor in the Participants list, and you can see the request notice in the Production Discussions panel.
You can now wait for the Layout Editor to complete their tasks.

#### Layout Editing

As a Layout Editor, you will have received a message inviting you to create the galleys for the submission.
To get started, login to the system and go to your dashboard.

![Layout Editor Dashboard showing list of assigned manuscripts.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-le-dashboard.png)

From here, find the submission and select the **Production** link. This will take you to the submission record.

![Production tab of on the assigned manuscript with 1 production ready file for the Layout Editor.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-le-submission.png)

From the Production Ready Files panel, download the files to your desktop and work outside of OJS to convert them to galley files. The next section explains galley file formats and preparation.

> Note: PKP is currently working on a project to automate the conversion of Microsoft Word documents into other formats, including XML, HTML, PDF, EPUB, etc. Keep an eye on our blog for updates.

#### Prepare and Add Galley Files

A Galley is the final publication-ready file that has been prepared for readers and will be published on the article page. Galleys should be in a stable non-editable format (e.g., HTML, PDF, ePub, or XML) versions of the full-text article. Galley files can also include supplementary material such as multimedia files and research data. You can publish a galley file for an article and for an entire issue.

##### Galley file component types

When you upload a galley file, you will need to select a **Component Type**. These are the same component types that authors select from when they upload submission files. You can configure component types under Workflow Settings > Submission > Components, according to whether you want the component type to be published and whether you want a link to it to appear on the article landing page or in the table of contents.

The configurations are as follows:

* Dependent: the link will not appear with published content at all
* Supplementary: The link will appear on the article landing page
* Neither supplementary nor dependent: The link will appear on the article landing page and in the table of contents

For example, if you want to embed multimedia files in HTML files and have these appear on the landing page, the issue page, and the submission page, you would configure the settings as follows:

* Go to Settings > Workflow > Submission > **Components** tab
* Click the blue arrow next to **HTML Stylesheet** and **Edit**
* Uncheck “Mark files of this type as dependent files” and “Mark files of this type as supplementary files”. Click **Save**.
* Click the blue arrow next to **Multimedia** and **Edit**
* Uncheck “Mark files of this type as supplementary files”. Leave “Dependent files” checked off. Click **Save**.

##### Galley file formats

Online journals publish their articles in a variety of file types. The most common are PDF and HTML, but increasingly additional formats are being used, such as ePub, MP3, and XML.

Plugins in OJS allow PDF, HTML, and XML files to be viewed in a web browser or downloaded. If the files are being downloaded instead of displayed in the browser, you may need to enable one of these plugins under Website Settings > Plugins:

* PDF.JS PDF Viewer provides rendering support for PDF Article files.
* eLife Lens Article Viewer provides rendering support for JATS XML Article files using eLife Lens.
* HTML Article Galley plugin provides rendering support for HTML Article files.

Other formats may require additional plugins or can be downloaded directly. Alternatively, you may host the full-text content on a different platform and embed a remote URL by choosing the checkbox: “This galley will be available at a separate website.”

##### Using templates

Requiring all submissions to use a document template that is pre-formatted with your journal’s publication styles (e.g., the font face, font size, boldness, placement, etc., of the header, body, footers, etc.) can make your document conversion much easier.
[Microsoft provides a brief overview for creating templates in MS Word](https://support.microsoft.com/en-us/topic/create-a-template-86a1d089-5ae2-4d53-9042-1191bce57deb?ui=en-us&rs=en-us&ad=us).

Once you’ve created a template that matches your journal style, it may be useful for submitting authors, layout editors, or other users.
Here’s an example of an OJS journal that requires authors to download and use a template file: [Paideusis](https://journals.sfu.ca/pie/index.php/pie/about/submissions).

Ideally, your template should be created using styles rather than direct formatting. This not only ensures consistency throughout your documents, but will also aid in any conversions to other formats (e.g., HTML). Here’s an [explanation of the difference between styles and direct formatting in Word](https://support.microsoft.com/en-us/office/customize-or-create-new-styles-d38d6e47-f6fc-48eb-a607-1eb120dec563?redirectSourcePath=%252fen-us%252farticle%252fStyle-basics-in-Word-d382f84d-5c38-4444-98a5-9cbb6ede1ba4&ui=en-US&rs=en-US&ad=US)

##### PDF files

A PDF is the easiest type of file to create from a Word document. Current versions of Microsoft Word (and other word processors) let you “Save As” or “Export As” a PDF. The majority of OJS journals publish their articles as PDFs.

PDFs are also popular with many readers as they most closely recreate the printed page. However, PDFs are often less flexible on mobile devices and do not always handle links or embedded media (such as sound or video files) particularly well. With the widespread usage of mobile devices, ensuring your audience can read your articles on their phones or tablets is increasingly important.

Example (see PDF link at bottom of page): [Irish Journal of Technology Enhanced Learning](http://www.journal.ilta.ie/index.php/telji/article/view/22/51)

##### HTML Files

HTML files have the advantage of flexibility. They handle linking and multimedia very well, and can fit on just about any screen - including phones and tablets. They do, however, look different than a printed page, so some readers prefer a PDF. The ideal situation is to provide both PDF and HTML files to best meet the needs of different users.

Creating an HTML file can require more time and effort than creating PDF files. Word processors do not have effective tools for doing a “Save As” to HTML. Microsoft Word tries to do this, but the results are not useful for uploading to OJS. Instead, try following this workflow:

* Convert the Word document. You can use [this free online tool](https://word2cleanhtml.com/) to do an initial conversion.
* Open the resulting HTML files in a text editor (e.g., NotePad in Windows) or HTML editor (e.g., Adobe Dreamweaver). From here, you will need to make any final clean up or formatting. Understanding the basics of HTML is required. There are many [free tutorials](https://www.w3schools.com/html/), but it does take some time.
* Keep the HTML formatting basic. Just focus on paragraphs, line breaks, headings, and links. Don’t worry about fonts, colours, or other design elements - OJS will take care of all of that automatically as part of the overall journal design.
* Upload to OJS as an HTML galley file
* The HTML viewer renders HTML files within an iframe, which may affect navigation to hyperlinked web pages. You can bypass this feature by opening hyperlinks in a new browser tab, by adding the `target="_blank"` attribute to your href tags.

A few example HTML templates can be found and adapted from these sources:

* [Resource by U of A](https://drive.google.com/file/d/1mCP0tguFJf7jJn_CNceEwvRn5eCJrvxP/view) - License: CC0 1.0 Universal (CC0 1.0)

Examples (see HTML link at bottom of the page):

* [Cultural Anthropology](https://journal.culanth.org/index.php/ca/article/view/4434)
* [Evidence Based Library & Information Practice](https://journals.library.ualberta.ca/eblip/index.php/EBLIP/article/view/29621)

###### Style HTML galley files

It is possible to style the design of your HTML galley files in bulk or on an individual per-article basis. Styling in bulk can only be done if you are using a custom theme.

To style an individual HTML galley file:

* While creating the HTML galley file, ensure that it includes a reference to the stylesheet in the `<head>` section, e.g. `<link rel="stylesheet" href="./article_styles.css" type="text/css" />`
* Upload the HTML galley file (see below for instructions on how to **Add Galley Files**)
* Edit the galley file
* Upload the CSS stylesheets with the appropriate **Component Type - HTML Stylesheet**

To style all HTML galley files:
If you are using a custom theme plugin, you can write a line of code to include a custom style for all HTML galleys. This will only apply to HTML galley files that do not have a style applied individually. More information on custom theming is available in the [PKP Theming Guide](https://docs.pkp.sfu.ca/pkp-theming-guide/en/).

###### Add images and multimedia to an HTML Galley

If you would like to include images or multimedia files in an HTML galley file, you can upload them as Dependent Files to the submission, and link to them within the file to display them.

Before beginning the item upload, you will need an HTML page containing one of the following:

* `<audio controls>` element (for MP3)
* `<video>` element (for MP4), or
* `<img src=”imagename”>` tag for images

The HTML page should also contain the exact name of the file you are connecting to.

You will need to save the audio/video/image file in MP3/MP4/JPEG/GIF format using the name in the HTML page.

Your HTML file will need to contain the following minimum code (for audio files). For the related video or image file code, please see the w3schools instructions on [embedding video in HTML](https://www.w3schools.com/html/html5_video.asp) or instructions on [embedding images in HTML](https://www.w3schools.com/html/html_images.asp).

```html
<html>
<head>
<title>MP3 upload</title>
</head>
<body>
<audio controls>
  <source src="filename.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>
</body>
</html>
```

In OJS you will need to configure the settings for your Component Types before adding multimedia files. See **Galley File Component Types** above for details about adjusting these settings.

Make sure you have “Multimedia” and/or “Image” files configured as “dependent files” in the Component Type settings.

![Form to add Multimedia as a dependent component type.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-prod-multimedia-component-edit.png)

Now go back to the submission to upload an HTML stylesheet to display your multimedia file. See below for instructions on how to **Add  Galley Files**. In addition, when you upload the file:

* Label the galley according to the multimedia file type (e.g., MP3, MP4, Image)
* Select **HTML Stylesheet** from the **Article Component** dropdown
* Upload the HTML file you prepared with at least the minimum code (instructions above)
* Click **Continue**
* In the **Review Details** tab you can upload Dependent Files. This is where you will upload the MP3/MP4/image file.

![Step 2 of uploading production ready files where users will go to upload their dependent files.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-prod-multimed-dep-file.png)

Select **Multimedia** or **Image** from the **Article Component** drop-down menu, and upload the MP3, MP4, or image file.

![Step 1 for uploading dependent files, dropdown bar lists Multimedia and Image as selection for Article components.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-prod-upload-multimedia.png)

When uploading an image file you will be asked to add a Caption, Credit, Copyright Owner, and Permission Terms, as applicable.

![Step 2 for uploading dependent files. Text fields to enter Caption, Credit, Copyright Owner, and Permission Terms.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-prod-image-details.png)

Click **Continue** to complete the upload, review the details, and confirm. Your multimedia file has now been added as a dependent file along with the HTML, and will be embedded in the HTML when the item is published.

##### ePUB Files

Similar to HTML files, ePub files are ideal for mobile devices but require specialized coding to create. Conversion tools are available, such as [Calibre](https://calibre-ebook.com/). More detailed HOW TO instructions for creating ePub files are [available here](https://www.wikihow.com/Convert-a-Word-Document-to-Epub).

Like HTML files, some additional cleanup may be required after conversion and [require some knowledge](http://www.jedisaber.com/eBooks/Introduction.shtml) of the format.

Example (see EPUB link at bottom of the page): [International Review of Research in Open and Distance Learning](http://www.irrodl.org/index.php/irrodl/article/view/2895)

##### XML Files

XML files are structured files in which each part of the article is tagged as a distinct element. This allows the reader to easily navigate through and access figures, images, metadata, references, and parts of the article text. Creating XML files is a very efficient way to publish in multiple formats. When you create an XML file, you can then automatically generate PDFs, HTML, ePub, and other formats.

![XML preview of article with navigation menu options.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-prod-xmlgalley.png)

PKP is developing tools that will allow you to create, convert, and edit XML files within OJS. Currently you need to create and edit the files outside of OJS. If you want to produce XML galley files for your journal, you can use the services of a graphic designer or typesetter, or if you have some XML expertise you can create the files yourself. W3schools has excellent tutorials on XML.

Example [Food and Nutrition Research](https://foodandnutritionresearch.net/index.php/fnr/article/view/3609/10173)

##### Multimedia files

It is becoming increasingly popular for journals to publish multimodal content, including audio and video files, in addition to text-based articles. In addition to providing audio and visual formats for text-based articles, which can help to increase the accessibility of journal content, multimodal content is increasingly [valued as an alternative form of scholarship](https://www.tandfonline.com/doi/full/10.1080/07294360.2017.1389857?casa_token=QlJ8xBTQUEMAAAAA%3AWDkOV6R-qfZxJBimLv_Jv4iB3o2XYeA-Cym7uxHoCww9THLVmZFVfKmRP3dtqq098HvYG6kqTl_v) which represents and reflects different modes of expression and ways of knowing. Journals that choose to create audio versions of text-based articles may choose to do so manually, by having someone read the article into a voice recorder, or automatically using Text to Speech software.

Multimedia files can be embedded into the article page on your journal site, or can be linked to  from an external site, such as YouTube or SoundCloud. If you use an external site, the quality may be better, but statistics will not be collected on galley views or downloads, and preservation of the content is dependent on the external site.

When uploading a multimedia file, you can select “article text” from the component list and upload the file (MP3, MP4, image file, etc) directly. This will allow the user to access the file using the image viewing software or the audio/video playing software installed on their device.

Example (see MP3 link in side menu at bottom of the page): [International Review of Research in Open and Distance Learning](http://www.irrodl.org/index.php/irrodl/article/view/3279)

Alternatively, you can embed the audio, video, or image file in an HTML page so that users can view the file directly in their browser. See **Add images and multimedia to an HTML galley** above for instructions on how to do this.

Example: [Intersectional Apocalypse](https://journals.lib.sfu.ca/index.php/ifj/article/view/673)

###### Upload a multimedia file linked from an external site

Upload the multimedia galley file in the Production stage of the workflow. See below for instructions on how to **Add Galley Files**. In addition, when you upload the file:

* Label the galley according to the multimedia file type (e.g., MP3/MP4)
* Check the box indicating “This galley will be available at a separate website”

![Pop-up window to add Video as an external Galley File.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-prod-upload-video-youtube.png)

To get the URL, locate the video or audio in YouTube, SoundCloud, etc., then click **Share** and copy the URL.

![Share Button on Youtube to generate external link for Galley File.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-prod-share-youtube.png)

Paste the URL into the remote galley field and click **Save**.

The video should now appear in the published submission.

#### Contact the Author

Next, you will want to share the PDF with the author for a final look and sign off. To do so, use the **Add Discussion** link in the Production Discussion panel. This will open a new window.

![Creating a discussion post in OJS to indicate that galley are ready for proofreading.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-le-production-add-participant.png)

Remember to add the author at the top of the window and then add a subject and a message.

Before sending, attach a copy of the PDF file using the **Upload File** link. This will make it available to the author.

![Step 1 of uploading galley file in discussion- uploading file.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-le-production-add-participant-upload.png)

Remember to select the correct Article Component and then upload the PDF.

Click **Continue**.

Next, make any changes to the file name (usually you don’t need to do anything here).

![Step 2 of uploading galley file in discussion- confirming file name.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-le-production-add-participant-upload2.png)

Then, you can upload additional files, if necessary.

![Step 3 of uploading galley file in discussion- option to add additional file or complete.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-le-production-add-participant-upload3.png)

Once you are done, hit **Complete**.

The file is now attached and you can send the message using the **OK** button.

![Discussion box showing the uploaded galley file as attachment.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-le-production-add-participant2.png)

The Author has now been notified and you can await their response.

#### Author Response

Once the author has had a chance to review the galleys and respond, you will receive an email notification and will see a reply in the Production Discussions.

![List of Production related discussion on author account.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-production-message-reply.png)

#### Add Galley Files

Now that the Author has proofread the galleys, you can make any final changes, and then upload them to the submission. To upload galleys, go to the Publication tab, then Galleys.

![Galley subtab within the manuscript's Publication tab to add galley.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-au-production-galleys.png)

Then click **Add galley**, which will open a new window.

![Creating new galley for with the galley label PDF and english as the language.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-production-galleys-upload1.png)

Add an appropriate label (e.g., PDF, HTML, etc.) and click **Save**.

![Step 1 of uploading file. PDF file uploaded displays option to Change File, Continue, or Cancel.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-production-galleys-upload2.png)

From this window, choose the appropriate article component (e.g., article text) and upload the galley file. Click **Continue**.

![Step 2 of uploading file. Displays option to edit file name, Continue, or Cancel.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-production-galleys-upload3.png)

If necessary, change the filename. Click **Continue**.

![Step 3 of uploading file. Confirming file has been added. Displays option to Complete or Cancel.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-production-galleys-upload4.png)

If you have more files, upload them now. Otherwise click **Complete**.

You can now see the galleys in the Galley panel.

![Galley subtab within the manuscript's Publication tab. Displays previously uploaded PDF.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-au-production-galleys-uploaded.png)

You can make changes to the upload by selecting the blue arrow to the left of the galley label, which reveals options to edit, change the file, or delete.

#### Edit Galley Files

If you want to make a change to a galley file or galley file label after it has been uploaded, you can edit it. Please note that if the article has already been published, to make a change to the galley file you will first have to un-publish the article or create a new version (see Versioning of Articles below). But before the article is published, you can edit the galley file easily.

1. Open the submission from the submission dashboard
2. Go to the Publication tab and Galleys
3. Click the blue arrow next to the file you want to edit
4. If you would like to edit the galley label, click the Edit button that appears and change the Galley Label
5. If you would like to change the file, click Change File and upload a new file
6. When you are finished editing, click Save

![Galley subtab within the manuscript's Publication tab. Blue arrow for PDF expanded to reveal additional option to Edit, Change File or Delete.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-au-production-galleys-edit.png)

#### Inform the Section Editor

Finally, you will need to inform the Section Editor that the galleys have been completed. To do so, use the Production Discussion panel and choose the **Add Discussion** link.

![Creating a discussion post in OJS to indicate that galley files have been uoloaded.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-production-galleys-complete.png)

Add the Section Editor to the top of the page, and then include a subject line and message. Click **OK** to send the message.

You can now see the final discussion.

![List of Production related discussion Section Editor account.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-au-production-galleys-discussions.png)

#### Section Editor Informs Editor

At this point, the Section Editor receives the notification from the Layout Editor and reviews the galley files.

They can either ask the Layout Editor to make additional changes \(using the Production Discussions\) or inform the Editor that the galleys are ready for publication.

To inform the Editor, use the Production Discussion panel's **Add Discussion** link.

The next step in publishing the submission is to check and finalize the metadata.

### Finalize Metadata {#finalize-metadata}

Before publishing the submission, you should check that the metadata for the article is complete and accurate in OJS and matches the metadata on the PDF. This is important for ensuring that the content is indexed by Google Scholar, discoverable by other services, and accessible to readers. To learn more, see [the Better Practices in Journal Metadata guide](https://docs.pkp.sfu.ca/metadata-practices/en/).

You can check the metadata for the submission by going to **Submissions**, opening the submission, going to the **Publication** tab, and checking the **Title**, **Contributors**, and **Metadata** tabs.

At this point you can also add the article to a category to display it on a thematic category page on your site and extract and save references (if you have not already).

#### Add the Article to a Category

Categories can be used to organize your articles into thematic collections. If you use categories in your journal, you can optionally add the article to a category or categories. For instructions on how to create categories see the [Journal Settings chapter](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/journal-setup). You can add the article to a category by editing its metadata.

* In the article submission, go to the **Publication** tab
* Click **Issue**
* In the **Categories** box, check the category or categories that you want to add the article to
* Click **Save**

![Issue subtab within Manuscripts Publication tab. Shows options to assign Issue, Section, Categories.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-prod-add-to-category.png)

#### Extract and Save References

If you would like to display the article’s bibliographic references on the article page with linked DOIs, and submit the references to Crossref with the rest of the article’s metadata, you can use the “Extract and save references” feature. This feature can only be used if you’re using the DOI plugin and the Crossref plugin to export your metadata to Crossref. The feature will store each reference in the database as a separate reference and add the DOI to the reference on the article page. It will also make it easier for indexing services, such as Google Scholar, identify and index the article’s citations.

The first thing you must do is enable References as a submission metadata field.

1. Go to Workflow Settings > Submission > Metadata
2. Scroll down to **References** and check off **Enable references metadata**
3. New options will appear below and you can select to either 
  * do not request references from the author during submission - the References field will not be on the submission form and instead references can be added by an editor
  * ask the author to provide references during submission - the References field will be on the submission form and authors can optionally add their references to it, or an editor can add references to the submission later
  * require the author to provide references before accepting their submission - the References field will be on the submission form and authors will be required to add their references to it
4. Click **Save**

![Setting option to Eanble Reference metadata with additional options for authors during the time of submission.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-prod-enable-references.png)

Now if you go to a submission record’s **Publication** tab you will see a **References** tab below. An editor can open the tab and copy and paste the article's references into the field. In addition, if you checked the second or third option above, there will be a **References** field when an author makes a submission and the author will be able to add their references to it.

Each reference should be on a separate line and you should sure the text you paste into the field is unformatted and has no extra line breaks or spaces. Remove any DOIs in the references if you plan to add them later with the Crossref Reference Linking plugin.

When the article is published, the references will appear on the article page and the references will be submitted to CrossRef.

After you have exported the article’s metadata to Crossref, you can insert the DOIs for the article references from Crossref if you use the Crossref Reference Linking plugin. Instructions on how to use the plugin are available in the [Crossref Plugin Guide](https://docs.pkp.sfu.ca/crossref-ojs-manual/en/references).

Once you have the plugin set up and have exported the article's metadata to Crossref, you can insert the DOIs from Crossref back into the references:

1. Open the submission
2. Go to the **Publication** tab and **References**
3. Click **Check Crossref DOIs**
4. Some DOIs will now be added to the references

### Create Issue {#create-issue}

> **Video:** [Video of Setting up a journal in OJS 3.3. Module 7: Issues](https://www.youtube.com/watch?v=opvVBWYnHho)

This PKP School video explains how to create, edit, publish, and manage Issues. To watch other videos in this series, visit [PKP’s YouTube channel](https://www.youtube.com/playlist?list=PLg358gdRUrDVTXpuGXiMgETgnIouWoWaY).

When you are ready to publish the article, you have to create an issue to publish it in first. Then you will schedule articles for publication in the issue. The articles will not be published until you publish the issue as a whole. This section explains how to create and edit issues.

From the left menu, select Issues to manage all of the issues for your journal.

![Future Issues tab in Issues. Displays Vol 1 No 3 (2018).](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-issues.png)

You will see tabs for Future Issues and Back Issues.

**Future Issues** are all of your unpublished issues. You can create as many of these as you wish, and schedule submissions to any of them.

**Back Issues** lists all of your published issues.

![Back Issue tab in Issues. Displays Vol 1 No 2 (2018) and Vol 1 No 1 (2018).](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-issues-back.png)

To create a new issue, use the **Create Issue** link and fill in the form.

![Form to create new issue.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-issues-create.png)

There are spaces to add volume, number, year, and title information (e.g., Special Issue #1), as well as a description, cover image, and custom URL. The cover image and description will appear at the top of the issue page on your site, if you add them. If you have volume, number, and title checked off below, you will be required to fill something into each field.

When you’re finished, click **Save**.

#### Edit Issue

You can also edit an existing future issue by selecting the blue arrow to the left of the issue entry on the Future Issues page.

![Vol 1 No 3 (2018) in Future Issues with blue arrow expanded to show additional options to Edit, Preview, Publish Issue, or Delete.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.1-jm-issues-edit.png)

This will reveal an **Edit** link, which will open a new window of information.

![Table of Contents for Vol 1 No 6 (2016): June 2016.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3-issues-details.png)

**Table of Contents**: For a new issue, this will be empty, but for issues that have had submissions scheduled, they will be listed here.

Use the blue arrow next to each submission to reveal links to go directly to the submission record or remove it.

**Issue Data**: This provides access to the volume, issue, number data you entered when first creating the issue.

**Issue Galleys**: This allows you to upload galley of the complete issue – e.g., one PDF containing all articles. This will be linked from the issue web page.

**Identifiers**: Use this space to add a DOI for the issue, if your journal supports issue-level identifiers.

#### Order Sections and Articles

When you publish an issue, articles will be displayed under your journal’s sections.

If you go to Journal Settings > Sections and edit a section, you can configure how it will appear on your published issue page, including whether the title of the section is displayed.

You can also drag and drop the sections to change the order of how they will appear on your published issue.

If you want to change the order of sections on a per issue basis or the order of articles within a section:

* Go to **Issues** and open the issue you want to edit
* Click **Order**
* Drag and drop the sections and articles where you want them
* Click **Done** when you are finished

#### Preview Issue and Articles

If you want to see what your articles will look like prior to publication, click on the Preview button on the Publication tab of the submission record. Users with the permission to preview will see this button from the Copyediting stage forward.

![Publication tab of Manuscipts shows subtab and option to Preview and Schedule Issue and language toggles to enter metadata in Espanol and English.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.3-ed-production-publish-preview-article.png)

If you want to see what your articles will look like in the context of an issue before publishing it, you can use the Issue Preview feature:

* Click the blue arrow next to the future issue
* Click **Preview**
* The issue preview page will open. To preview an article, click the article title in the table of contents.

![Vol 10 No 10 (2019) in Future Issues with blue arrow expanded to show additional options to Edit, Preview, Publish Issue, or Delete.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-ed-production-publish-issue.png)

#### Publish Issue

Once you are happy with the issue hit the **Publish Issue** link to publish it on your journal website.

#### Notify Readers

You will have the option to send a notification to users about the new issue.

To not send a notification of a new issue published, uncheck the box beside “Send notification email to all registered users” before pressing **OK**.

![Option to notify readers upon issue publication.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-ed-production-reader-notify.png)

The content of the announcement is generated automatically and cannot be edited. You can alternatively use the [Announcements](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-website#announcements) feature to send a publication announcement with customized content.

#### Unpublish Issue

Use the **Unpublish Issue** link to remove the issue and all of its content from public view. The issue will revert to the Future Issues tab.

#### Delete Issue

You can use the **Delete** link to remove the issue entirely. Not only will the issue be unpublished, the organizational structure and any issue metadata will also be removed. Any assigned articles will revert to their unpublished status.

### Add the Article to an Issue {#add-the-article-to-an-issue}

Now that you have created an issue, you can add the article to it. Please note that the article will not be published until the issue is published. In this step you are assigning the article to an issue.

* Go back to **Submissions**
* Find and open the submission you want to publish
* Go to the **Publication** tab > **Issue**
* In the **Issue** field, select the issue you want to publish the article in
* The **Section** will be filled in automatically based on the submission metadata but you can change it if needed
* You can select a **Category** if you haven’t already done so (explained above)
* If you want an image to appear on the article page, upload it under **Cover Image**
* You can add **Page Numbers**, which will be included in the metadata and on the table of contents
* **Date Published** will be set automatically when the issue is published. Do not enter a publication date unless the article was previously published elsewhere and you need to backdate it.
* Click **Save** when you are finished

![Issue subtab in Manuscript Publication tab showing all options and fields related to Issue - Issue, Section, Categories, Cover Image, Page Number and Date Published.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-prod-add-to-issue.png)

### Schedule for Publication {#schedule-for-publication}

The next step is to schedule the article for publication. Although the article will not be published until the issue it is assigned to is published, the Schedule for Publication step is the final step in confirming that the article is ready to be published.

Only a Journal Editor can schedule an article for publication, not a Section Editor or Guest Editor.

The article must have been assigned to an issue and passed the Review stage in order to be able to schedule it for publication.

When you are ready to publish the article:

* Open the submission
* Go to the **Publication** tab
* Click the blue **Schedule for Publication** button.

![Publication tab of Manuscripts shows subtab and option to Preview and Schedule Issue and language toggles to enter metadata in Francais (Canada) and English.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs3.2-ed-prod-schedule-for-pub.png)

A message will pop up that confirms you want to schedule the article for publication. Click **Publish**.

#### Schedule for Individual Publications

In previous versions of OJS, an article would be assigned to an issue and would be published when that issue was published. In OJS 3.2, it is now possible to set a specific publication date for each publication.

To do this, under the **Publication** tab of the manuscript, go to **Issues**.

Under **Date Published** you can enter the publication date if it is different from the issue publication date. If not, leave this blank.

![Issue subtab with an Manuscripts Publication tab highlights the Date Published field.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-ed-production-schedule-individual.png)

In order to schedule an individual publication, it must be assigned to an issue and have passed the review stage.

If the date is set to a future date, the publication should be published when the scheduled task runs for that date.

If the scheduled manuscript is unscheduled from the issue, the previously scheduled date should not change.

### Versioning of Articles

An ability to publish versions of articles is one of the major new features in OJS 3.2. This feature supports preprint publication and publishing new versions of articles when a correction or significant change has been made. With the versioning feature you can manage different versions of an article and clearly indicate which is the most current.

Once an article is published, neither metadata nor galleys can be edited. When a revision of a published article or metadata is necessary, it can be done in one of two ways:

![Publication tab of article highlighting options available after article has been published to Unpublish or Create New Version.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-ed-production-versioning-ways.png)

**Option 1: Unpublish and republish**

Unpublishing an article allows you to make changes without creating a new version. After unpublishing, you can update metadata and/or replace the galley file and schedule the article for publication again. If scheduled into a published issue, it will become available right away. No notification will be sent to readers, since the notification is sent when an issue is published, not for an individual article.

**Option 2: Create new version**

When creating a new version, you will be able to make changes to the metadata and/or galley files. Make sure to click **Save** on the bottom right to record the changes.

You can keep track of version updates under **All Versions**. Each version is marked by a number and date published. The version currently being updated is marked by a number and **Unpublished**.

![Publication tab of manuscript showing a list of all versions available for this article. Article currently has 4 published version and 1 unpublished.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-ed-production-all-versions.png)

Once your changes are completed, you can publish the new version by clicking **Publish** on the top right. If scheduled into a published issue, it will become available right away. No notification will be sent to readers since the notification is sent when an issue is published, not for an individual article.

The list of prior versions and update dates will be listed on the published article page.

![List of dates for all versions for article that displays on the article abstract page on the front end.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-ed-production-published-versions.png)

Readers will be able to access previous versions. They will see a message on the article and galley pages advising them that it is an outdated version and pointing them to the most recent version.

Example of an outdated version message on the article page:

![Warning notification of outdated version on article abstract page and prompt to read the most recent version.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-ed-production-outdated-version.png)

Example of an outdated version message on the PDF galley page:

![Warning notification of outdated version on PDF viewer and prompt to read the most recent version.](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/assets/learning-ojs-3.2-ed-production-outdated-pdf.png)

The article URL will always point to the most recent version, with earlier versions being available at the same URL with the version at the end of the URL (e.g. /version/1234/).

#### DOIs and Indexing of Versions

Where a DOI was assigned to the original version, it will not be changed automatically. Previously deposited CrossRef metadata will not be automatically updated. If article metadata was changed, we recommend updating CrossRef metadata in the CrossRef XML Export Plugin by manually depositing the updated article. For instructions on how to manually deposit an article see the PKP’s [CrossRef Plugin Guide - Manual Deposits](https://docs.pkp.sfu.ca/crossref-ojs-manual/en/config#manual-deposits).

Indexing services and repositories that use OAI to harvest metadata will need to harvest the article metadata again in order to update to the new version.

The new version will be tagged properly to be recognized and updated by Google Scholar's index, but the harvester will need to visit your site again in order to find the new version.

It is best to check with a particular repository or index to learn what their process is and what they require.

### Continuous Publishing & Early View

Continuous publishing – also known as rolling publication schedule – is a way of publishing that prioritizes immediacy. When publishing continuously, articles are released as soon as they are ready. Journals may also choose to provide an early view prior to layout (also known as online first, in-press, post-print, first view, etc.).

Some journals may find that a more frequent publication schedule can also help with [search engine optimization (SEO)](https://docs.pkp.sfu.ca/getting-found-staying-found/en/getting-found-visibility#search-engines) and provide a way to generate more frequent social media output.

The content should be considered final, and have already undergone review and copyediting. As the work may be cited right away, figures and appendices should be in place. To avoid confusion, if page numbers are subject to change, they should be avoided.

OJS is currently designed for a traditional publishing model where articles are published in issues. However, there is a way to adopt a continuous publishing model within OJS.

#### Use Current Issue - for Continuous Publishing

* Create a [new issue](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/production-publication#create-issue). Issues can be given a title in the Issue Data. We recommend using a title that communicates its ongoing nature.
* Publish the new issue: while it is possible to publish an issue with 0 articles, an empty issue may be confusing to readers. We recommend that you publish the new issue after at least 1 article is assigned.
* When the next article is ready, assign it to **Back Issues > Current Issue**. This article will be published immediately on the current issue page. If using DOIs, be sure to **Assign Identifier** before publishing. If your DOI registration is not automated, manually register your newest DOI.
* Please note that default DOI patterns are generated using issue numbers:
	 * If you plan to generate a DOI suffix based on vol/issue numbering, do not change the vol/issue later.
	 * If you intend to change vol/issue numbering, do not generate a suffix using the default patterns. Choose to generate a custom pattern instead. See [DOI Configuration documentation](https://docs.pkp.sfu.ca/doi-plugin/en/) for more details.
* After the Current Issue is completed, you may want to rename it according to the standard naming convention (e.g., Volume 2, Issue 5), by going to [Edit Issue](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/production-publication#edit-issue).
* If you only changed the Issue Title:
	* This field is not exported to CrossRef, DOAJ or PubMed, but it is used for DataCite. If you use DataCite, remember to update that record by resubmitting metadata via the DataCite plugin.
* If you have enabled [the Citation Style Language plugin](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-website#citation-style-language-plugin) in your journal, this plugin should be disabled as you will have incorrect citations in the "How to Cite" block on your articles due to changing issue numbers. 
* Consider using the [article versioning feature](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/production-publication#versioning-of-articles) to publish the initial Early View version of the article. When the final version is ready, create a New Version and publish it.

Since new articles will be published immediately, build verification steps within your workflow by using the article [Preview features](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/production-publication#preview-issue-and-articles) to check for accurate metadata and galleys.

#### Use the Forthcoming Plugin - for Continuous Publishing

The [Forthcoming plugin](https://github.com/ajnyga/forthcoming) allows journals to publish a version of an article using OJS’s versioning feature before an entire issue is published. This is an external third-party plugin available for OJS 3.2.1 and above. As a plugin that is not maintained by PKP, we cannot guarantee its functionality or compatibility with all software versions.

See the [Forthcoming plugin’s README file](https://github.com/ajnyga/forthcoming#readme) for details on how it works and contact your OJS administrator to see if support is available for this plugin.

#### Use Custom Pages - for Continuous Publishing and Early View

Create a Custom Page under [Navigation settings](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-website#navigation) and add articles to it.

This option is fully separate from the regular Submission Workflow, and requires a manual addition and removal of article metadata and/or full text.

On the blank Custom page, journals can provide:

* A list of articles with minimal metadata and no full-text articles   
* A list of articles with full metadata and no full-text articles
* A list of articles with hyperlinks to full-text / early view versions (the files must be hosted elsewhere, such as in the [Publisher Library](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-workflow#publisher-library))

When a new article is ready to be shared, manually add it to the Custom Page. Then when the entire issue with the article or the final version of the same article is ready to be published, manually remove it from the Custom Page.

Content of custom pages will not appear in journal keyword searches, and articles added to custom pages will not show up in article searches or receive DOIs.

#### Journal Settings for Continuous Publishing

You may want to change some journal settings to reflect the change in publishing schedule:

* [Default Copyright Year](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-distribution): for a continuous publishing model, select the article’s publication date. This default can be overridden on a case-by-case basis.
* [Journal Policies](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/journal-setup): clearly communicate the publishing schedule and frequency within “About the Journal”.
* [Customize the “Current Issue” label on the homepage](https://docs.pkp.sfu.ca/translating-guide/en/customize-locale#example-customize-the-current-issue-label-on-homepage): if you would like to change the "current issue" label on homepage to "current publications" or "current articles," you can do it via the Custom Locale Plugin (in OJS 3.2 or newer).  

#### Communications

If you would like to notify your readers when each new article is published, create an individual Announcement, as the automatic notification message for a new publication can only be sent when a new issue is published. See the [Website Settings](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/settings-website.html#announcements) chapter for information about Announcements.

If your journal had previously used a traditional issue-based model and has now switched to a continuous publishing model, you may need to update third-party agencies, including:

* ISSN Centre: to update the ISSN record, contact your [National Centre](https://www.issn.org/services/requesting-an-issn/contact-an-issn-national-centre/)
* Indexes that include publication frequency
* Indexes that include information about the time between submission and publication

> **Original chapter:** [Production and Publication](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/production-publication)

---

## Attribution and License

This documentation is sourced from [Learning OJS 3.3: A Visual Guide to Open Journal Systems](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/), published by the Public Knowledge Project documentation project.

Copyright: Simon Fraser University holds the copyright for work produced by the Public Knowledge Project. The documentation is available under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).
