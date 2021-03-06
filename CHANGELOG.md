Changes
=======

# 0.8.0 / 2016-03-01

* [FEATURE] Add success/failure metric [#75][] [@jhulten][]
* [FEATURE] Retry tags submission when host is not yet present on DD [#80][] [@olivielpeau][]
* [OPTIMIZE] Ensure tags always returns an array [#78][] [@rlaveycal][]
* [OPTIMIZE] More robust failed chef run checking [#69][] [@bigbam505][]

# 0.7.0 / 2015-10-22

* [FEATURE] Support passing `DATADOG_PROXY` env var to control `dogapi` behavior, [#65][] [@datwiz][]
* [OPTIMIZE] Only map `tags` if non-nil, [#66][] [@owen][]
* [MISC] Style updates, [#60][] [@miketheman][]
* [MISC] Update test matrix to handle latest released major versions, [#59][] [@miketheman][]

# 0.6.0 / 2014-09-17

* [FEATURE] Submit Chef-related tags to Datadog for Events, [#52][] [@miketheman][]

# 0.5.0 / 2014-08-21

* [FEATURE] Place recent updated resources above stacktrace on failure, [#46][] [@miketheman][]
* [BUGFIX] Handle cases where Chef fails during compile phase, [#51][] [@miketheman][]
* [FEATURE] Allow credentials to be passed as string keys vs symbols, [#50][] [@dwradcliffe][]
* [MISC] Testing framework updates, [@miketheman][]
* [MISC] Doc updates

# 0.4.0 / 2014-05-08

* [FEATURE] Allow specification of a `:hostname` to config to override `node.name`, [#41][] [@miketheman][]
* [FEATURE] Allow passing an array of handles in config to alert when Chef fails, [#29][] [@miketheman][]
* [OPTIMIZE] Use new version of `dogapi` lib to submit tags for Chef only, [#28][] [@miketheman][]
* [MISC] Updated versions of Chef tested
* [MISC] Style update for source file name, parens

# 0.3.0 / 2014-01-23

* [MISC] **Breaking Change**: Chef 0.9.x is no longer supported. Extra code implemented for 0.9 versions has been removed. [@miketheman][]
* [BUGFIX] Report correct response when failing to submit tags, [#39][] [@miketheman][]
* [OPTIMIZE] Refactor hostname resolution to its own method, simplify `report` method. [@miketheman][]
* [OPTIMIZE] Refactor metrics reporting to its own method, simplify `report` method. [@miketheman][]
* [OPTIMIZE] Refactor tagging get/set to own methods, simplify `report` method. [@miketheman][]
* [MISC] Converted `opts` to an instance variable of `config` to reduce the amount of instance variables passing around. [@miketheman][]
* [OPTIMIZE] Don't try to tag node when Application Key isn't provided, [#31][] [@miketheman][]
* [OPTIMIZE] Only load in the parts of the Chef gem that are used. [@miketheman][]
* [OPTIMIZE] Change order in which event_data is constructed, to not lose the full backtrace, [#37][] [@miketheman][]

Testing suite: [#18][], [@miketheman][]
* Removed Tailor testing in favor of Rubocop
* Added Appraisals with specific Chef versions to be tested
* Added RSpec testing via VCR and Webmock

# 0.2.0 / 2013-10-31

* [BUGFIX] moved Chef gem dependency to development, [#34][] [@miketheman][]
* [BUGFIX] redis python client check was not properly checking the default version, [@remh][]
* [MISC] tailor 1.3.1 caught some cosmetic issue, [@alq][]
* [MISC] fixed a few repo & build issues, [@miketheman][]

# 0.1.2 / 2013-04-03

And all other versions were prior to this. See git history for more.

<!--- The following link definition list is generated by PimpMyChangelog --->
[#18]: https://github.com/DataDog/chef-handler-datadog/issues/18
[#28]: https://github.com/DataDog/chef-handler-datadog/issues/28
[#29]: https://github.com/DataDog/chef-handler-datadog/issues/29
[#31]: https://github.com/DataDog/chef-handler-datadog/issues/31
[#34]: https://github.com/DataDog/chef-handler-datadog/issues/34
[#37]: https://github.com/DataDog/chef-handler-datadog/issues/37
[#39]: https://github.com/DataDog/chef-handler-datadog/issues/39
[#41]: https://github.com/DataDog/chef-handler-datadog/issues/41
[#46]: https://github.com/DataDog/chef-handler-datadog/issues/46
[#50]: https://github.com/DataDog/chef-handler-datadog/issues/50
[#51]: https://github.com/DataDog/chef-handler-datadog/issues/51
[#52]: https://github.com/DataDog/chef-handler-datadog/issues/52
[#59]: https://github.com/DataDog/chef-handler-datadog/issues/59
[#60]: https://github.com/DataDog/chef-handler-datadog/issues/60
[#65]: https://github.com/DataDog/chef-handler-datadog/issues/65
[#66]: https://github.com/DataDog/chef-handler-datadog/issues/66
[#69]: https://github.com/DataDog/chef-handler-datadog/issues/69
[#75]: https://github.com/DataDog/chef-handler-datadog/issues/75
[#78]: https://github.com/DataDog/chef-handler-datadog/issues/78
[#80]: https://github.com/DataDog/chef-handler-datadog/issues/80
[@alq]: https://github.com/alq
[@bigbam505]: https://github.com/bigbam505
[@datwiz]: https://github.com/datwiz
[@dwradcliffe]: https://github.com/dwradcliffe
[@jhulten]: https://github.com/jhulten
[@miketheman]: https://github.com/miketheman
[@olivielpeau]: https://github.com/olivielpeau
[@owen]: https://github.com/owen
[@remh]: https://github.com/remh
[@rlaveycal]: https://github.com/rlaveycal