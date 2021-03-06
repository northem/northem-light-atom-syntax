<p align="center"><img src="https://cdn.rawgit.com/arcticicestudio/northem-light-atom-syntax/develop/assets/northem-light-atom-syntax-banner.svg"/></p>

<p align="center"><img src="https://assets-cdn.github.com/favicon.ico" width=24 height=24/> <a href="https://github.com/arcticicestudio/northem-light-atom-syntax/releases/latest"><img src="https://img.shields.io/github/release/arcticicestudio/northem-light-atom-syntax.svg"/></a> <a href="https://github.com/arcticicestudio/northem-light/releases/tag/v2.0.1"><img src="https://img.shields.io/badge/Northem_Light-v2.0.1-6FBAD0.svg"/></a> <img src="https://atom.io/favicon.ico" width=24 height=24/> <a href="https://github.com/atom/atom/releases/tag/v1.13.0"><img src="https://img.shields.io/badge/Atom->=v1.13.0-green.svg"/></a> <a href="https://atom.io/themes/northem-light-atom-syntax"><img src="https://img.shields.io/apm/v/northem-light-atom-syntax.svg"/></a> <a href="https://atom.io/themes/northem-light-atom-syntax"><img src="https://img.shields.io/apm/dm/northem-light-atom-syntax.svg"/></a></p>

---

# 2.1.0
*2017-03-05*
**Please note that the minimal version for this theme is now >=1.13.0 due to the Atom theme API change!**

## Features
### Languages
❯ The namespace tag entity color now differs from markup/HTML tags which are also now colored correctly.  
*Character Data* blocks tags `<![CDATA[` `]]>` are now formated bold and, including the surrounded text, using the comment color. (@arcticicestudio, #13, fd455260)

<p align="center"><img src="https://raw.githubusercontent.com/arcticicestudio/northem-light-atom-syntax/develop/assets/scrot-lang-xml.png"/></p>

<p align="center"><strong>CDATA</strong><br><img src="https://cloud.githubusercontent.com/assets/7836623/23581982/8ea1c6b8-0120-11e7-817f-1614cb61a934.png"/></p>
<p align="center"><strong>Markup/HTML Entities</strong><br><img src="https://cloud.githubusercontent.com/assets/7836623/23581985/b7232d70-0120-11e7-871f-a28c88810b6b.png"/></p>
<p align="center"><strong>Namespace tags</strong><br><img src="https://cloud.githubusercontent.com/assets/7836623/23581987/bd2c9b70-0120-11e7-9d1b-2da7e974c273.png"/></p>

❯ Implemented optimized <img src="http://elixir-lang.org/favicon.ico" width=16 height=16/> [Elixir](http://elixir-lang.org) styles for the community package <img src="https://avatars0.githubusercontent.com/u/1481354" width=16 height=16/>  [`language-elixir`](https://atom.io/packages/language-elixir). (@arcticicestudio, #14, 429a321f)

<p align="center"><img src="https://cloud.githubusercontent.com/assets/7836623/23582009/ecaed4d0-0120-11e7-9cc4-00a6fd106313.png"/></p>

## Improvements
❯ Migrated to the new Atom theme API.  
Starting from Atom version 1.13, the contents of `atom-text-editor` [elements are no longer encapsulated within a shadow DOM boundary](http://blog.atom.io/2016/11/14/removing-shadow-dom-boundary-from-text-editor-elements.html).  
This means the `:host` and `::shadow` pseudo-selectors should be completely removed and all syntax selectors should be prepended with `syntax--`.
To prevent breakage with existing style sheets, Atom will automatically upgrade selectors for versions less or equal to 1.12. (@arcticicestudio, #15, d915b739)

<p align="center"><img src="http://blog.atom.io/img/posts/shadow-dom.png"/></p>

# 2.0.0
*2016-11-10*
**The whole project has been cleaned up and rewritten to adapt the codebase of the [Nord Atom Syntax](https://github.com/arcticicestudio/nord-atom-syntax) project!**
*This closes the milestone [Version 2.0.0](https://github.com/arcticicestudio/northem-light-atom-syntax/milestone/2) and the associated backlog ticket #8.*

## Features
Detailed information about new features can be found in the [README](https://github.com/arcticicestudio/northem-light-atom-syntax/blob/develop/README.md#features) and the [Nord Atom Syntax](https://github.com/arcticicestudio/nord-atom-syntax#features) documentation!

### Color Palette
This major update has been migrated to the new Northem Light color palette version [`2.0.0`](https://github.com/arcticicestudio/northem-light/releases/tag/v2.0.0). (@arcticicestudio, #9, 7d3d5ca5)

### Design
The old design was uncomfortable, unconsistent and has not been updated to the latest Atom version which resulted in unpredictable bugs and glitch due to changes of the Atom Core.
Northem Light Atom Syntax has adapted the Nord Atom Syntax design which provides a clean, elegant and up-to-date syntax highlighting. (@arcticicestudio, #9, 7d3d5ca5)

### Language Support
All previous supported language packages have been migrated to the new codebase and packages currently supported by Nord Atom Syntax have been added. (@arcticicestudio, #9, 7d3d5ca5)

### Documentation
All project documentations adapted the new project setup and styles and new branding assets have been added. (@arcticicestudio, #10, 1c9fa404)

# 0.20.0
*2016-08-11*
## Features
### Language Support
❯ Implemented language support for <img src="https://golang.org/favicon.ico" width=16 height=16/> [Go](https://atom.io/packages/language-go) (@arcticicestudio, [GHI #5][ghi-5])
  - Implemented language support for <img src="https://www.gnu.org/favicon.ico" width=16 height=16/> [Make](https://atom.io/packages/language-make) (@arcticicestudio, [GHI #5][ghi-5])
  - Implemented language support for [Nunjucks](https://atom.io/packages/language-nunjucks) (@arcticicestudio, [GHI #5][ghi-5])
  - Implemented language support for <img src="http://www.scala-lang.org/favicon.ico" width=16 height=16/> [Scala](https://atom.io/packages/language-scala) (@arcticicestudio, [GHI #7][ghi-7]) :email:

## [backlog][backlog-language-library-framework-support]
This version closes the backlog item
  - [x] <img src="https://golang.org/favicon.ico" width=16 height=16/> [Go](https://atom.io/packages/language-go) (@arcticicestudio, [GHI #5][ghi-5])
  - [x] <img src="https://www.gnu.org/favicon.ico" width=16 height=16/> [Make](https://atom.io/packages/language-make) (@arcticicestudio, [GHI #5][ghi-5])
  - [x] [Nunjucks](https://atom.io/packages/language-nunjucks) (@arcticicestudio, [GHI #5][ghi-5])
  - [x] <img src="http://www.scala-lang.org/favicon.ico" width=16 height=16/> [Scala](https://atom.io/packages/language-make) (@arcticicestudio, [GHI #7][ghi-7]) :email:

## Improvements
### Language Support
**JavaScript**  
❯ Removed a explicit keyword selector to allow syntax highlighting for all keywords

### Documentation
❯ Removed unnecessary comment-doc overhead like index numbering, section delimitation etc.  
❯ The documentations have been modernized and the `README` now includes a "Getting started" section

# 0.19.1
*2016-05-06*
## Bug Fixes
### Dependencies
❯ Updated to [`northem-light@1.0.1`](https://github.com/arcticicestudio/northem-light/releases/tag/v1.0.1) to fix an exception on package loading caused by an unrecognized input in the `northem-light.less` stylesheet (@zhrkevin, [GHI #6][ghi-6])

# 0.19.0
*2016-05-04*
## Features
### Language Support
❯ Implemented language support for [LaTeX](https://atom.io/packages/language-latex) (@arcticicestudio, [GHI #6][ghi-6])

## [backlog][backlog-language-library-framework-support]
This version completes the backlog item
  - [x] <img src="http://www.latex-project.org/favicon.ico" width=16 height=16/> [LaTeX](https://atom.io/packages/language-latex) (@arcticicestudio, [GHI #6][ghi-6])

# 0.18.0
*2016-04-11*
## Features
### Language Support
❯ Implemented language support for the [React JSX](https://atom.io/packages/react) syntax extension (@Pszek, [GHI #3][ghi-3])

### Package Support
❯ Implemented package support for the <img src="https://avatars3.githubusercontent.com/u/7209979" width=16 height=16/> [minimap-git-diff](https://atom.io/packages/minimap-git-diff) package (@Pszek, [GHI #4][ghi-4])

## [backlog][backlog-language-library-framework-support]
This version completes the backlog items
  - [x] <img src="https://facebook.github.io/react/favicon.ico" width=16 height=16/> [React.js](https://atom.io/packages/react) (@Pszek, [GHI #3][ghi-3])

# 0.17.0
*2016-04-10*
The project repository has been reconstructed and reinitialized for a clean migration to [gitflow](http://nvie.com/posts/a-successful-git-branching-model).  
This is only relevant for the git history and does **NOT** impact the source code!

## Maintenance
### Dependencies
**Development**
*Skeletons*
❯ Migrated to [`glacier-git@0.21.0`](https://github.com/arcticicestudio/glacier-git)

# 0.16.0
*2016-03-05*
## Features
### Language Support
❯ Implemented language support for [Java Properties](https://atom.io/packages/language-java). This also includes `.properties` files like `build.properties` for [Apache Ant](http://ant.apache.org) or `ivy.properties` for [Apache Ivy](http://ant.apache.org/ivy) since these files are interpreted as [Java Properties](https://atom.io/packages/language-java).

# 0.15.0
*2016-03-01*
## Improvements
### Language Support
**HTML** (`language-html`)  
❯ [[#3](https://github.com/arcticicestudio/northem-light-atom-syntax/issues/3)] Improved the readability:
  - Attribute names are now underlined for a better emphasis
  - Attribute values are now colored `light-blue` for a better differentiation between attribute names and values and to differ from normal text

### Gutter
❯ Line numbers in the gutter are now left-aligned

# 0.14.0
*2016-02-15*
## Features
### Language Support
❯ Implemented language support for the [HTML](https://atom.io/packages/language-html) responsive-email preprocessor [MJML](https://atom.io/packages/language-mjml) (@caseymhunt, [GHI #2][ghi-northem-light-atom-syntax-2])

# 0.13.0
*2016-02-04*
## Refactoring
❯ Refactored all package files for performance by removing redundancy and improving nesting (~`10ms`/`11ms` to ~ `9ms`/`8ms` startup time)

## Bug Fixes
❯ Fixed all file modes/permissions (linux *umask*)

## Improvements
### Documentation
❯ Edited license file to valid markdown

## Maintenance
### Dependencies
❯ Updated to [`northem-light@1.0.2`](https://github.com/arcticicestudio/northem-light)

*Specifications*  
❯ Updated to [`arcver@0.8.0`](https://github.com/arcticicestudio/arcver)

**Development**
*Skeletons*  
❯ Migrated to [`glacier-git@0.8.0`](https://github.com/arcticicestudio/glacier-git)

# 0.12.0
*2016-01-27*
## Features
### Language Support
❯ Implemented language support for [SQL](https://atom.io/packages/language-sql)

# 0.11.0
*2016-01-24*
## Features
### Language Support
❯ Implemented language support for [C++](https://atom.io/packages/language-c) (@rkhunter, [GHI #2][ghi-2])

# 0.10.2
*2015-10-04*
## Bug Fixes
### Package Support
❯ Fixed the background color for the `markdown-preview` package codeblocks

# 0.10.1
*2015-10-01*
## Bug Fixes
### Package Support
❯ Fixed a deprecation warning for the outdated `.editor` class

# 0.10.0
*2015-09-27*
## Features
### Package Support
❯ Implemented support for the [color-picker](https://atom.io/packages/color-picker) package

## Improvements
### Package Support
❯ Code elements are now colored `light-blue` in the preview of the [markdown-preview](https://atom.io/packages/markdown-preview) package

### Documentation
❯ Added a list of supported packages and the corresponding version range

## Bug Fixes
### Package Support
❯ Fixed the background color for code blocks of the [markdown-preview](https://atom.io/packages/markdown-preview) package

# 0.9.1
*2015-09-24*
## Bug Fixes
❯ Fixed multiple basic color variable names caused a crash on theme loading  
❯ Fixed misplaced basic color variables caused by the reorded `colors.less` file

# 0.9.0
*2015-09-24*
## Features
### Language Support
❯ Implemented language support for [Generic Config (dotfiles)](https://atom.io/packages/language-generic-config), provides syntax highlighting for all files containing comments and/or non-comments without a particular structure like
  - `.gitignore`
  - `.env`

❯ Implemented language support for [git](https://atom.io/packages/language-git), includes
  - Git Commit Messages (`COMMIT_EDITMSG`,`MERGE_MSG`)
  - Git Configuration `.gitconfig`,`.gitmodules`,`.git/config`,`/etc/gitconfig`)
  - Git Rebase Messages

❯ Implemented language support for [PropertyList](https://atom.io/packages/language-property-list), includes the formats
  - ASCII (Old-Style)
  - XML

## Improvements
### Language Support
**Jade** (`language-jade`)  
❯ Better differentiation for `HTML` tags:
  - Control keywords (`if`, `each`, `unless` etc.) now highlighted in `dark-blue` instead of `blue`  
  - Embedded JavaScript block- and line indicators (`- var`, `script.` etc.) now highlighted in `dark-blue` instead of `blue`  
  - Inline tags and control flows (`#[]`, `#{}`) now highlighted in `dark-blue` instead of `blue`  
  - Preprocessor keywords (`block`, `append`, `prepend`, `include` etc.) now highlighted in bolded `dark-blue` instead of `blue`

# 0.8.0
*2015-08-29*
## Features
### Language Support
❯ Implemented language support for [`C`](https://atom.io/packages/language-c)  
❯ Implemented language support for [`Clojure`](https://atom.io/packages/language-clojure)  
❯ Implemented language support for [`C#`](https://atom.io/packages/language-csharp) (CS,CSharp)

## Improvements
### Language Support
**Haskell** (`language-haskell`)
❯ Improved highlighting for tags and the `runhaskell`-shebang

# 0.7.0
*2015-08-16*
## Features
### Language Support
❯ Implemented language support for [`D`](https://atom.io/packages/language-d)

# 0.6.0
*2015-08-16*
## Features
### Language Support
❯ Implemented language support for [`GLSL`](https://atom.io/packages/language-glsl)  
❯ Implemented language support for [R](https://atom.io/packages/language-r)

# 0.5.0
*2015-08-12*
## Features
### Language Support
❯ Implemented language support for [`HAML`](https://atom.io/packages/language-haml)

# 0.4.1
*2015-08-10*
## Bug Fixes
❯ Fixed color variable name for Java caused a crash on theme loading (@paulidealiste, [GHI #1][ghi-1])

# 0.4.0
*2015-08-08*
## Features
### Language Support
❯ Implemented language support for [`Java`](https://atom.io/packages/language-java)

# 0.3.0
*2015-08-02*
## Features
### Language Support
❯ Implemented language support for [Haskell](https://atom.io/packages/language-haskell)

## Bug Fixes
### Documentation
❯ Fixed favicon sizes in `README.md`  
❯ Fixed missing notice for the [`file-icons`](https://atom.io/packages/file-icons) package in [`README.md`](README.md)

# 0.2.0
*2015-06-05*
## Features
### Language Support
❯ Implemented language support for [Julia](https://atom.io/packages/language-julia)  
❯ Implemented language support for [ShellScript](https://atom.io/packages/language-shellscript)

# 0.1.0
*2016-04-19*
**Project Reconstruction**

# 0.0.0
*2016-04-10*
**Repository Reinitialization**

[backlog-language-library-framework-support]: https://github.com/arcticicestudio/northem-light-atom-syntax/issues/5

[ghi-1]: https://github.com/arcticicestudio/northem-light-atom-syntax/issues/1
[ghi-2]: https://github.com/arcticicestudio/northem-light-atom-syntax/issues/2
[ghi-3]: https://github.com/arcticicestudio/northem-light-atom-syntax/issues/3
[ghi-4]: https://github.com/arcticicestudio/northem-light-atom-syntax/issues/4
[ghi-6]: https://github.com/arcticicestudio/northem-light-atom-syntax/issues/6
[ghi-7]: https://github.com/arcticicestudio/northem-light-atom-syntax/issues/7

[ghi-northem-light-atom-syntax-2]: https://github.com/arcticicestudio/northem-light-atom-syntax/issues/2
