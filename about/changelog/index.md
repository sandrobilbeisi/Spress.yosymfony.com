---
layout: page-about
header: { title: Change log, sub: Release history }
title: Changelog
id_content: changelog 
---

More information about the [releases](https://github.com/yosymfony/Spress/releases).

## V1.1.0-beta.2 {#1-1-0-beta-2}
Date: 2014-11-21

* <span class="label label-success">New</span> Issue [#17](https://github.com/spress/Spress/issues/17): 
[Twig debug mode](/news/2014/10/28/new-in-spress-1-1-debug-mode/) through configuration.
* <span class="label label-success">New</span> Two new scaffolding commands: `new:post` and `new:plugin`.
* <span class="label label-success">New</span> Proposal [#22](https://github.com/spress/Spress/issues/22): Namespace "new" in commands for creating stuff.
* <span class="label label-danger">Deprecated</span> The command `site:new` has been declared deprecated and replaced by `new:site`.

## V1.1.0-beta.1 {#1-1-0-beta-1}
Date: 2014-10-19

* <span class="label label-success">New</span> [IO API](/news/2014/05/11/new-in-spress-1-1-io-api/) useful for interacting with the users.
* <span class="label label-success">New</span> Proposal [#9](https://github.com/spress/Spress/issues/9): Support for environment configuration files. New key `env` for `config.yml`.
* <span class="label label-success">New</span> PR [#12](https://github.com/spress/Spress/issues/12): Added ability to use multiple extensions on layouts.
* <span class="label label-success">New</span> Proposal [#15](https://github.com/spress/Spress/issues/15): Built-in server and watch for changes.
* <span class="label label-default">Fixed</span> Issue [#10](https://github.com/spress/Spress/issues/10): Classname with typo: EnviromentEvent. This class was replaced by EnvironmentEvent.
* <span class="label label-default">Fixed</span> PR [#14](https://github.com/spress/Spress/issues/14): Changed Frontmatter regex pattern to allow for CRLF line endings.
* <span class="label label-primary">Improved</span> Proposal [#13](https://github.com/spress/Spress/issues/13): Split Spress into Spress Core and its ecosystem.
* <span class="label label-primary">Improved</span> Replaces all uses of deprecated method mergeWith from ConfigServiceProvider by union method.
* <span class="label label-primary">Improved</span> Proposal [#11](https://github.com/spress/Spress/issues/11): Improve the plugins manager for writing plugins more easily.
* <span class="label label-primary">Improved</span> Decoupled options for Plugin Manager.
* <span class="label label-primary">Improved</span> PSR-4 for classloader.
* <span class="label label-primary">Improved</span> Symfony components >= 2.4 and < 3 in `composer.json`.
* <span class="label label-primary">Improved</span> The default value for `url` key at global configuration is empty-string.
* <span class="label label-primary">Improved</span> Documentation fixes.
* <span class="label label-danger">Deprecated</span> The configuration options: `baseurl` and `relative_permalinks` has been declared  deprecated.

## v1.0.3 {#1-0-3}
Date: 2014-05-22

* <span class="label label-default">Fixed</span> bug [#7](https://github.com/yosymfony/Spress/issues/7): Error with Site Build.
* <span class="label label-primary">Improved</span> Tested on PHP 5.6 (Travis CI).

## v1.0.2 {#1-0-2}
Date: 2014-03-30

* <span class="label label-default">Fixed</span> bug [#6](https://github.com/yosymfony/Spress/issues/6): Twig tags not rendered in posts located at variable `site.posts`.
* <span class="label label-default">Fixed</span> bug [#6](https://github.com/yosymfony/Spress/issues/6) with variables `site.categories` and `site.tags`.
* <span class="label label-primary">Improved</span> Variables site.categories and site.tags have page-identifier as index of array.
* <span class="label label-primary">Improved</span> Base implementation of ContentItemInterface created at ContentItem. The classes PageItem and PostItem extend from this.



## v1.0.1 {#1-0-1}
Date: 2014-03-08

* <span class="label label-success">New</span> events related with pagination phase (issue [#3](https://github.com/yosymfony/Spress/issues/3)): **spress.before_render_pagination** and **spress.after_render_pagination**.
* <span class="label label-primary">Improved</span> Payload argument of Render method (plugins TemplateManager) is optional.
* <span class="label label-primary">Improved</span> pagination phase of posts.
* <span class="label label-default">Fixed</span> bug [#4](https://github.com/yosymfony/Spress/issues/4): UrlGenerator always has ending slash.
* <span class="label label-default">Fixed</span> the class loader path when Spress is installed as package.

## v1.0.0
Date: 2014-02-05

* <span class="label label-success">New</span> Added template manager to the API plugins for rendering Twig templates (accessible from spress.start event).
* <span class="label label-primary">Improved</span> the class loader of the site plugins.
* <span class="label label-default">Fixed</span> documentation

## v1.0.0-rc.3
Date: 2014-01-12

* <span class="label label-success">New</span> Support to composer for spress site plugins.
* <span class="label label-success">New</span> Install themes with Composer.
* <span class="label label-success">New</span> Generate composer.json in a blank site.
* <span class="label label-primary">Improved</span> the search of folders that starting with underscore.
* <span class="label label-default">Fixed</span> the documentation.
* <span class="label label-danger">Deleted</span> Spresso theme. Now is a package.
