# Learn on Demand Systems Markdown as IDL Guide 

## Revision History

|**Version**|**Date**|**Edited By**|**Comments**|
|---|---|---|---|
|0.1|Feb. 22, 2017|Kirk Munro|Unreleased; first draft|

## Disclaimer

This document supports a preliminary release of a software product that
may be changed substantially prior to final commercial release. This
document is provided for informational purposes only and Learn on Demand
Systems, LLC, makes no warranties, either express or implied, in this
document. Information in this document, including URL and other Internet
Web site references, is subject to change without notice. The entire
risk of the use or the results from the use of this document remains
with the user. Unless otherwise noted, the companies, organizations,
products, domain names, e-mail addresses, logos, people, places, and
events depicted in examples herein are fictitious. No association with
any real company, organization, product, domain name, e-mail address,
logo, person, place, or event is intended or should be inferred.
Complying with all applicable copyright laws is the responsibility of
the user. Without limiting the rights under copyright, no part of this
document may be reproduced, stored in or introduced into a retrieval
system, or transmitted in any form or by any means (electronic,
mechanical, photocopying, recording, or otherwise), or for any purpose,
without the express written permission of Microsoft Corporation.

Learn on Demand Systems, LLC may have patents, patent applications,
trademarks, copyrights, or other intellectual property rights covering
subject matter in this document. Except as expressly provided in any
written license agreement from Learn on Demand Systems, the furnishing
of this document does not give you any license to these patents,
trademarks, copyrights, or other intellectual property.

Copyright 2017 © Learn on Demand Systems, LLC. All rights reserved.

All other trademarks are property of their respective owners.

* * *

# Markdown Support

Lab on Demand now supports the use of [Markdown](https://en.wikipedia.org/wiki/Markdown "Markdown is a lightweight markup language with plain text formatting syntax that allows for easy conversion into HTML or other formats.")
as an Integrated Digital Lab (IDL) source. This support provides additional
value to lab content authors, allowing them to choose whether they want to
use the traditional IDL Studio editor for content editing for a lab, or to
use markdown documents and a markdown editor for their content editing
experience. This choice is akin to choosing between using a point-and-click UI,
which may offer user experience advantages that some people prefer, and using
text-based tools, which offer authoring efficiencies and an ecosystem of rich
tools that others will prefer.

The addition of markdown support into Lab on Demand provides the following
benefits to lab content authors:

1. **Readability** - A Markdown IDL document reads much like a lab manual would.
1. **Simplicity** - Markdown is structured text without tags. Editing Markdown
files is much easier and more efficient than editing lab content inside of a
user interface.
1. **Offline editing** - There are plenty of free and commercial offline
Markdown editors available for all mainstream platforms/devices being used
today: Windows, macOS, Linux, iOS, and Android.
1. **Revision control** - GitHub has native support for Markdown (Markdown is
the preferred method of documentation on GitHub), and with GitHub comes revision
control, support for multiple authors, pull requests, forks/clones, etc.
1. **Multi-author support** - By using Markdown inside of services like GitHub
(or similar services like Visual Studio Online), you can support multiple
content authors contributing to the content for one lab at the same time.
1. **Broad adoption** - Markdown is being adopted all over the place – from
creation of documentation at Microsoft (MSDN docs, PowerShell Help files, etc.)
to defining blog content/pages (Wordpress, Ghost, others) to Slack channels (you
can use Markdown directly inside of Slack messages), and much, much more.
1. **Tooling** - There are some great libraries out there to convert from
Markdown to HTML such as Markdig. Markdig is very fast and includes extra
goodies like AST generation, which makes for much easier Markdown conversion to
other content by using the Visitor pattern.

There is a small learning curve to overcome (Markdown syntax, as well as the
tools that you use to manage your Markdown files such as GitHub); however, the
benefits you will realize once you have learned how to write your lab content in
Markdown and once you have stored those files in GitHub are well worth the
effort.

## Getting started

How you get started using Markdown depends on whether you are writing the
content for a new lab or converting existing lab content that was created using
IDL Studio into Markdown format. Each of these scenarios is covered below.

### Create a GitHub account

In order to reap benefits such as revision control and multi-author support, you
will need a GitHub account. GitHub provides a lot of desirable features for free
that add a lot of value to lab authoring, and we highly recommend using it when
creating your lab content using Markdown.

If you already have a GitHub account, skip to the next section. If not, here is
what you need to do to create a GitHub account:

TODO: Instruct users to create a GitHub account if they haven't already done so,
since GitHub is used throughout the rest of this guide. If the number of steps
are small, list them here, along with a few helpful screenshots if appropriate.
If there are many steps and screenshots necessary, and if this is already well
documented (or captured in video) elsewhere, then link to that content here so
that we don't repeat what is already done elsewhere.

### Authoring content for a new lab using Markdown

TODO: Fill out these details with documentation describing the steps

* download the content from the LearnOnDemandSystems/idl-md-template repository
* add that content to your local git repository for lab content
* upload your changes to a GitHub repository
* import your changes into Lab on Demand (using steps below)

NOTE: The first several steps change for GitHub enabled labs, and the need to
commit becomes optional if you leave auto-commit on

### Authoring content for an existing lab using Markdown

TODO: Fill out these details with documentation describing the steps

* export the IDL content for your lab (using steps below)
* create a git repository for that content and push it to GitHub (or create
a repository in GitHub, clone it locally, and copy the bits there)
* make your changes
* commit your changes to your GitHub repository
* import your changes into Lab on Demand (using steps below)

NOTE: The first several steps change for GitHub enabled labs, and the need to
commit becomes optional if you leave auto-commit on

### Exporting Markdown content out of Lab on Demand

![Export Markdown - Step 1](media/export/01-export.png "Click on \"Export\" to export your lab content out of Lab on Demand")

![Export Markdown - Step 2](media/export/02-content-only.png "Click on the \"Lab Metadata: IDL Content Only\" radio button and then click \"OK\" to export your lab contents in markdown format")

### Importing Markdown content into Lab on Demand

![Edit lab profile](media/import/01-edit-lab.png "Click on \"Edit\" to edit your lab profile")

![Enable IDL support](media/import/02-enable-idl.png "Check the \"Has IDL Content\" check box to turn on IDL support for your lab profile")

![Import Markdown - Step 1](media/import/03-import.png "Click on \"Import\" to import your markdown content")

![Import Markdown - Step 2](media/import/04-select-idl-content.png "Click on the \"IDL Content\" radio button and then click \"OK\" to continue")

![Import Markdown - Step 3](media/import/05-choose-file.png "Click on \"Choose file\" to browse to the archive that contains your lab contents in markdown format")

![Import Markdown - Step 4](media/import/06-browse-to-archive-file.png "Browse to a zip file that contains your lab contents in markdown format (markdown file and screenshots/videos) and click on \"Open\" to select that file for import")

![Import Markdown - Step 5](media/import/07-click-import.png "Click on \"Import\" to import the lab contents into Lab on Demand")

![View the lab manual](media/import/08-view-lab-manual-to-verify.png "Click on \"Lab Manual\" to view the updated lab manual and verify the contents were imported correctly")

