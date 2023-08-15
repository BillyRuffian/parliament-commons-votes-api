# parliament_commons_votes

ParliamentCommonsVotes - the Ruby gem for the Commons Votes API

An API that allows querying of Commons Votes data.

This SDK is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: v1
- Package version: 1.0.0
- Build package: org.openapitools.codegen.languages.RubyClientCodegen
For more information, please visit [https://www.parliament.uk/](https://www.parliament.uk/)

## Installation

### Build a gem

To build the Ruby code into a gem:

```shell
gem build parliament_commons_votes.gemspec
```

Then either install the gem locally:

```shell
gem install ./parliament_commons_votes-1.0.0.gem
```

(for development, run `gem install --dev ./parliament_commons_votes-1.0.0.gem` to install the development dependencies)

or publish the gem to a gem hosting service, e.g. [RubyGems](https://rubygems.org/).

Finally add this to the Gemfile:

    gem 'parliament_commons_votes', '~> 1.0.0'

### Install from Git

If the Ruby gem is hosted at a git repository: https://github.com/GIT_USER_ID/GIT_REPO_ID, then add the following in the Gemfile:

    gem 'parliament_commons_votes', :git => 'https://github.com/GIT_USER_ID/GIT_REPO_ID.git'

### Include the Ruby code directly

Include the Ruby code directly using `-I` as follows:

```shell
ruby -Ilib script.rb
```

## Getting Started

Please follow the [installation](#installation) procedure and then run the following code:

```ruby
# Load the gem
require 'parliament_commons_votes'

api_instance = ParliamentCommonsVotes::DivisionsApi.new
division_id = 56 # Integer | Id number of a Division whose records are to be returned
format = 'format_example' # String | xml or json

begin
  #Return a Division
  result = api_instance.divisions_get_division_by_id(division_id, format)
  p result
rescue ParliamentCommonsVotes::ApiError => e
  puts "Exception when calling DivisionsApi->divisions_get_division_by_id: #{e}"
end

```

## Documentation for API Endpoints

All URIs are relative to *http://commonsvotes-api.parliament.uk*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ParliamentCommonsVotes::DivisionsApi* | [**divisions_get_division_by_id**](docs/DivisionsApi.md#divisions_get_division_by_id) | **GET** /data/division/{divisionId}.{format} | Return a Division
*ParliamentCommonsVotes::DivisionsApi* | [**divisions_get_divisions_groups_by_party**](docs/DivisionsApi.md#divisions_get_divisions_groups_by_party) | **GET** /data/divisions.{format}/groupedbyparty | Return Divisions results grouped by party
*ParliamentCommonsVotes::DivisionsApi* | [**divisions_get_voting_records_for_member**](docs/DivisionsApi.md#divisions_get_voting_records_for_member) | **GET** /data/divisions.{format}/membervoting | Return voting records for a Member
*ParliamentCommonsVotes::DivisionsApi* | [**divisions_search_divisions**](docs/DivisionsApi.md#divisions_search_divisions) | **GET** /data/divisions.{format}/search | Return a list of Divisions
*ParliamentCommonsVotes::DivisionsApi* | [**divisions_search_total_results**](docs/DivisionsApi.md#divisions_search_total_results) | **GET** /data/divisions.{format}/searchTotalResults | Return total results count


## Documentation for Models

 - [ParliamentCommonsVotes::DivisionGroupedByParty](docs/DivisionGroupedByParty.md)
 - [ParliamentCommonsVotes::MemberSearchQueryParameters](docs/MemberSearchQueryParameters.md)
 - [ParliamentCommonsVotes::MemberVotingRecord](docs/MemberVotingRecord.md)
 - [ParliamentCommonsVotes::PartyVoteResult](docs/PartyVoteResult.md)
 - [ParliamentCommonsVotes::PublishedDivision](docs/PublishedDivision.md)
 - [ParliamentCommonsVotes::QueryParameters](docs/QueryParameters.md)
 - [ParliamentCommonsVotes::RecordedMember](docs/RecordedMember.md)
 - [ParliamentCommonsVotes::SearchQueryParameters](docs/SearchQueryParameters.md)


## Documentation for Authorization

Endpoints do not require authorization.

# parliament-commons-votes-api
