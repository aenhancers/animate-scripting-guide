# Animate Scripting Guide

This repo hosts the Animate Scripting Guide RST docs, linked into a http://readthedocs.io system hosted at https://an-scripting.docsforadobe.dev/

---

## Contribution

Contributors are welcome and encouraged to suggest fixes, adjustments, notes/warnings, and anything else that may help the project.

---

## Internal References

Anchors should be defined at each page setting relative to the root folder; the anchor for the "Application" page within the JS Object Reference should be:

	.. _intro/Application

And the anchor for a child item (property, method or example):

	.. _intro/Application.open

Then, to link to these items from other pages, we use:

	:ref:`intro/Application`

or:

	:ref:`intro/Application.open`

If you want different text than the title the anchor points to:

	:ref:`Check this out! <intro/Application.open>`

---

## External Links

These should follow the following structure:

	`Link Text <http://www.aenhancers.com>`__

---

## Tables

Function parameter tables should have following order:

|   Parameter   | Type |         Description         |
| ------------- | ---- | --------------------------- |
| ``parameter`` | Type | What does the parameter do? |


Use [Table Formatter](https://marketplace.visualstudio.com/items?itemName=shuworks.vscode-table-formatter) for VSCode for easier table formating.

---

## Admonitions Usage

Currently, the following [admonitions](http://docutils.sourceforge.net/docs/ref/rst/directives.html#admonitions) are in use in this project. Try to keep one piece of data per note, for easier parsing.

	.. note::
		Notes detail version added, and/or relevant pieces of information.

	.. tip::
		Tips supply helpful suggestions on usage or behaviours.

	.. warning::
		Warnings convey negative behaviours, or when something won't work the way you'd expect.

---

## Adding undocumented attributes or methods

If you find attributes or methods that are not mentioned in this documentation, and they are not publically announced by Adobe, please add this warning to attribute/method so the user knows to use it at their own risk.

	.. warning::
	  	This method/property is officially undocumented and was found via research. The information here may be inaccurate, and this whole method/property may disappear or stop working some point. Please contribute if you have more information on it!

---

## Build HTML Locally

You may want to build the HTML locally before pushing, in order to ensure that the result is what you'd expect. These files aren't included in the git repo, nor are they used online; this is solely to create a local, offline version of the online docs.

- Install ``Python``
- Install ``pip``
- Navigate to the project directory and use the command ``pip install -r requirements.txt``
- Build the docs using ``make html``

---

## Licensing & Ownership

This project exists for educational purposes only.

All content is copyright Adobe Systems Incorporated.
