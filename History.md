
v0.6.0 / 2016-09-13
==================

  * Merge pull request #29 from @xsve / pairrates
    * Implemented rate calculation for any pair of currencies via base currency
  * Update travis ruby list
  * Fix usage of URI.join instead of File.join

v0.5.0 / 2016-08-12
===================

  * Changed base api url
  * Fix rubocop to 0.41.2 for Ruby 1.9 support
  * Update rake to 11 and rubocop to 0.41
  * README add Installation
  * Update rubocop to 0.38
  * Always use raise to signal exceptions
  * Use last rubinius binary on travis
  * Update year
  * Update README badges
  * Update jruby to 9.0.4.0
  * Update rubocop and add frozen_string_literal
  * Add Ruby 2.3 and rbx-2 to CI
  * Remove inch from dev tools for ruby 1.9
  * Update money deps
  * Update deps and freeze strings constants

v0.4.1 / 2015-12-06
===================

  * Add more test for latest and historical urls
  * used the correct URL for secure historical

v0.4.0 / 2015-09-28
===================

  * Add webmock helpers for tests
  * No need for TEST_APP_ID with webmock
  * Add ChangeLog
  * Support historical data endpoint with date
  * move version into a module not depending on money
  * Remove encodings headers
  * Better secure_connection tests
  * Better temp_cache_path and read_from_url use on tests
  * Update inch to 0.7
  * Add Money::Bank::OpenExchangeRatesBank::VERSION
  * Update minitest and timecop
  * Use inch for doc suggest
  * Improve doc for #valid_rates?
  * Added jruby-9.0.0.0 to travis
  * Rakefile: add --display-style-guide option to rubocop
  * Improve code documentation
  * Update money gem to 6.6
  * Added license badge
  * Improve code documentation
  * Remove useless doc attr_reader
  * Improve code documentation
  * Improve documentation of OpenExchangeRatesBank class
  * Run rubocop on default rake
  * Added rake rubocop task
  * Added inch documentation badge
  * Rename README.markdown to README.md
  * Update README
  * Add jruby-head to travis
  * Add travis notifications config
  * Make rubocop happy

v0.3.1 / 2015-06-17
===================

  * Fix secure oer url (see #22)
  * Test fail for #22; https
  * More clear spec for ttl (see #17)
  * Add minitest-line for debug
  * Update license date
  * Update license date

v0.3.0 / 2015-06-14
===================

  * add ruby-head to travis.yml
  * gem: syntax check
  * test: syntax check
  * Syntax fix with rubocop
  * Use tr instead of gsub
  * update monetize to 1.3
  * Tests for the secure_connection option
  * Updated README to include secure_connection example
  * Added the secure_connection option to enable HTTPS connections to OER
  * travis: added 2.2.0 version

v0.2.3 / 2014-12-21
===================

  * Bump to 0.2.3
  * Upgrade money to 6.5.0 and monetize to 1.1.0
  * update not present exchange rate and know exchange
  * Update latest.json
  * Doc save_rates and code cleanup
  * adjust tests to intentionally remove AED from data file and test conversions to AED
  * setup reverse rates (ie. XYZ -> USD)
  * travis: cache bundler
  * README: added badges [ci skip]

v0.2.0 / 2014-09-12
===================

  * update contributors and authors
  * travis: remove jruby-head
  * use exchange_with and get_rate from VariableExchange
  * tests: unify raise testing
  * tests: @bank to subject
  * Revert "travis: cache bundle remove 1.9.3,jruby"
  * travis: cache bundle remove 1.9.3,jruby
  * README: update
  * update money gem to 6.2.1
  * travis: added config

v0.1.7 / 2014-04-15
===================

  * Bump to 0.1.7
  * test: expire_rates implementation testing
  * Remove useless boolean return for expire_rates
  * Added pry gem for debug
  * Add the ability to expire rates after a fixed amount of time
  * test: use const for get rate
  * update case description in spec
  * getting rate implementation moved from #exchange_with to own method
  * test: remove deprecation warning about money 6.1.0
  * test: Remove RR deprecation warning
  * Added license on gemspec
  * README: typo

v0.1.5 / 2013-07-11
===================

  * Added Rakefile for tests
  * Merge pull request #10 from weynsee/remove_multi_json
  * use vanilla json instead of multi_json
  * require at least ruby 1.9.2
  * fix failing tests
  * use https protocol for rubygems.org to avoid warnings

v0.1.1 / 2012-10-01
===================

  * Bump to v0.1.1
  * Some cleanup in tests.
  * Use TEST_APP_ID_PATH.
  * Update README for tests and app_id.
  * Refactoring to cope with Proc for cache, allowing greater flexibility
  * Tidy up formatting
  * Added app_id necessary for ongoing usage of OER API

v0.0.7 / 2012-07-23
===================

  * Bump to v0.0.7
  * Added contributors.
  * Update documentation - update_rates must be called prior to attempting a currency conversation
  * Raise unknown rate format if can't find an exchange rate (rather than FloatDomainError)

v0.0.6 / 2012-05-08
===================

  * Added invalid json case for save_rates.
  * Use cache for exchange test and use same_currency?
  * Update spec for money 5.0.0 version.
  * Make sure cache file isn't overwritten if json returns an error
  * Don't error out when exchanging from a currency to itself even if there are no rates
  * Restructure to prevent writing empty cache file, and add spec

v0.0.5 / 2012-03-29
===================

  * Better tests.
  * Fix over issue over integer type rate.
  * overwrite cache file in a block to make sure it's closed after writing
  * add failing test when calling update_rates after save_rates
  * Remove warning: already initialized constant STRINGIFIED_KEYS
  * make tests pass for money 4.0.2
  * round numbers correctly to make tests pass in 1.8.7-p358

v0.0.4 / 2011-12-11
===================

  * Skip exchange unknown by Money and fix tests.
  * Sync latest openexchangerates.

v0.0.3 / 2011-10-19
===================

  * Dont check file exist for a cache...

v0.0.2 / 2011-10-19
===================

  * [bugfix] check file exist on filesystem.
  * Initial commit.
