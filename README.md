# A document catalog, or a filing system

This is work in progress, and may remain so forever, do not take this seriously.

## Goals

### What not to do

* Not tied to a particular tool, except...
* Use only linux filesystem and userland tools
* All configuration and metadata in user readable (as opposed to dev readable
  format. No special characters, no json, plain text files with as little 
  mental interpretation as possible.
* No server processes required, only tools

### Features
* Design a filing system as a folder structure in advance. Yes folders are
  limited but they are ubiquitous. Let's see how far we can go with just using
  what linux already provides.

* Allow tools to maintain and refactor the folder structure, again these
  could be based simply on linux tools.

* Automated filing of new files, based on rules which work on filename, file
  metadata and/or file contents.

* Check with user before filing something. Assisted filing or manual filing
  should work as well.

# Filing

Allow a tool to create an initial folder structure for filing. Nested, heirar-
-chical, it has disadvantages, but let's start with it.

## Sample folder structure

```text
~/docs
	self
		memos-to-self
		blog
		notes
		creative
			fiction
				short
				medium
				long
			nonfiction
				critique
				psychology
				political
				philosopy
				other
		ideas
		uncategorized
	papers
		cs
		math
		swengg
		chem
		phy
			astronomy
			optics
		bio
		photography
		psychology
		philosophy
		uncategorized
	articles
		cs
		math
		swengg
		chem
		phy
			astronomy
			optics
		bio
		photography
		psychology
		philosophy
		uncategorized
	finance
		company-reports
			<company-name>
				annual
				quarterly
				half-yearly
				other
		company-info
			<company-name>
				data
				articles
				notes
		portfolio
		taxes
	personal
		scanned-ids
		sensitive
```

## Tools to create and maintain the folder structure

### catog create
### catog update
### catog remove (only remove config not the folder structure)


