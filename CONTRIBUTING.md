# Contributing to phlowers

At this time we **do not accept contributions from outside the organization** as we are waiting for a clear governance. Still, people outside the organization are of course welcome to use the libraries we will develop in this project.

This document describes how organization members can contribute.

## English convention
The convention for phlowers code and documents, is to use American English. A list of spelling differences between British and American English can be found [here](https://www.britishcouncilfoundation.id/en/english/articles/british-and-american-english).

## License
Phlowers is an open source project in which each repository is licensed under the [Mozilla Public License 2.0](https://www.mozilla.org/en-US/MPL/2.0/). By contributing to phlowers, you accept and agree to the terms and conditions for your present and future contributions submitted to phlowers.

## Contributing to the code or the documentation
Before contributing to the project, please be sure to have read and understood the [license](#license) paragraph.

Please also make sure that you fully understand the [DCO mechanism](#dco) and the [contributing process](#contributing-process) described below.

### DCO

The project uses a mechanism known as a [Developer Certificate of Origin (DCO)](https://developercertificate.org/) to manage the process of ensuring that we are legally allowed to distribute all the code and assets for the project. A DCO is a legally binding statement that asserts that you are the author of your contribution, and that you wish to allow phlowers to use your work.

Contributors sign off on these requirements by adding a `Signed-off-by` line to commit messages. All commits from all repositories of the phlowers community have to be signed-off in this way:

```
This is my commit message.

Signed-off-by: Jay Doe <jay.doe@server.com>
```

You can write it manually, but Git even has a -s command line option to automatically append it to your commit message:

```
$ git commit -s -m 'This is my commit message'
```

Please make sure to configure your .gitconfig file beforehand with your name and email address:

[user]
	name = Jay Doe
	email = jay.doe@server.com

Most IDEs can also be configured in order to automatically add a `Signed-off-by` line at the end of the commit message.

Note that, during continuous integration, a check is performed to see if all commits in a pull request contain a valid `Signed-off-by' line.

### Contributing process

Once the development is done, you have to create a [pull request](https://help.github.com/en/articles/about-pull-requests):
- Make sure you have updated the documentation: no Pull Request shall be merged without the associated documentation;
- Fill all the relevant sections of the template to give context to the reviewer;
- Assign one or more reviewer;
- Verify that all [status checks](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-status-checks) are OK, especially the Sonar analysis.

The reviewer will review your proposal and:
- Approves your changes: your contribution fits the project guidelines and will be merged;
- Comments: the reviewer suggests to make some improvements;
- Requests a change: your proposal cannot be merged as such. You need to fix it with respect to the different comments made by the reviewer.

**Please note that, after a first review has been done, no force-push should be done on the Pull Request.** A force-push makes it more difficult for reviewers to follow the changes following their reviews.
