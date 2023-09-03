Change Log
----------
## 2023.2.3 (2023-09-04)
### Added
- Query builder can now specify the operation type (scan, query, or auto for automatic selection of the appropriate operation)
- Query builder can now specify the index name (or use 'auto' for automatic selection of the appropriate index)
- Query builder can now specify the sort order when using a range key
### Changed
- Improved syntax for the `begins_with` and `contains` functions in the query builder
### Fixed
- Fixed the usage of the `IN` operator in the query builder

## 2023.2.2 (2023-08-23)
### Added
- The ability to save queries
- Display of saved queries in the query history popup
- Display of saved requests in the request history popup
- [\#38](https://github.com/AntonShuvaev/intellij-dynamodb/issues/38) Open Edit Item dialog by double-clicking on the row number or by ctrl + double-clicking on the row
- [\#35](https://github.com/AntonShuvaev/intellij-dynamodb/issues/35) Copy items to another table
### Changed
- Tables can be opened in Data Browser or REST Console
- Favorite requests, queries and consoles are now displayed within the cluster node
- Store request history and connection details separately
### Fixed
- [\#34](https://github.com/AntonShuvaev/intellij-dynamodb/issues/34) Submitting error report doesn't work
- [\#39](https://github.com/AntonShuvaev/intellij-dynamodb/issues/39) Dragging columns should be preserved if you refresh query
- [\#40](https://github.com/AntonShuvaev/intellij-dynamodb/issues/40) Expanding edit window doesn't expand textarea
- Table cell popup editor turns green when searching
- "IllegalStateException: Do not change documents during undo as it will break undo sequence" might occur in some cases
- Various minor fixes

## 2023.2.1 (2023-07-12)
### Fixed
- "IllegalArgumentException: Wrong offsets" might occur in some cases
- Other minor fixes

## 2023.2.0 (2023-05-15)
### Added
- The query builder now automatically updates to display the generated query when a `scan` or `query` request is executed.
- When switching between requests, the response view automatically updates to show the cached response.
- Query builder now supports `null` values.
- Added the ability to zoom in the result table.
- You can now move multi-level columns in the result table.
- Structure view (`Cmd+7`) for DynamoDB tables with the ability to navigate to a column and hide/show columns.
- A link to the User Experience Survey has been added to the help action group.
### Fixed
- The query builder now is not hidden when query is not valid.

## 2023.1.5 (2023-04-20)
### Fixed
- [\#32](https://github.com/AntonShuvaev/intellij-dynamodb/issues/32) Not working with YDB Documents tables

## 2023.1.4 (2023-04-11)
### Fixed
- [\#31](https://github.com/AntonShuvaev/intellij-dynamodb/issues/31) Datagrip cannot successfully restart with plugin installed
### Changed
- Do not automatically execute queries from opened files after IDE restart

## 2023.1.3 (2023-04-10)
### Fixed
- [\#30](https://github.com/AntonShuvaev/intellij-dynamodb/issues/30) Ability to trust self-signed certificates
- Credentials might be lost after IDE restart on Windows

## 2023.1.2 (2023-04-07)
### Added
- [\#30](https://github.com/AntonShuvaev/intellij-dynamodb/issues/30) Ability to trust self-signed certificates
- Action to change default page size
- Ability to create DynamoDB file from project view context menu

## 2023.1.1 (2023-04-03)
### Fixed
- [\#29](https://github.com/AntonShuvaev/intellij-dynamodb/issues/29) Failed to refresh process-based credentials

## 2023.1.0 (2023-03-16)
### Added
- [\#28](https://github.com/AntonShuvaev/intellij-dynamodb/issues/28) Support for proxy
- Recent DynamoDB files are stored and can be opened from the "Recent Files"
- Support for 2023.1 IDEs
### Changed
- DynamoDB toolwindow icon changed to the monochrome version
### Fixed
- DynamoDB files are not correctly shown in "Recent Files" list
- [\#22](https://github.com/AntonShuvaev/intellij-dynamodb/issues/22) JSON import fails to read file with single null value 
- [\#23](https://github.com/AntonShuvaev/intellij-dynamodb/issues/23) Bad conversion of JSON null field to binary

## 2022.3.5
### Fixed
- "JsonParseException: Unexpected character" error occurs in some cases
### Added
- [\#24](https://github.com/AntonShuvaev/intellij-dynamodb/issues/24) Support for assume role with MFA

## 2022.3.4
### Fixed
- "java.lang.VerifyError" error occurs when using "Move statement" action
- [\#19](https://github.com/AntonShuvaev/intellij-dynamodb/issues/19) Support operator "!=" in PartiQL and filter expression

## 2022.3.3
### Fixed
- Regression: Add to favorites dialog is not working

## 2022.3.2
### Fixed
- [\#20](https://github.com/AntonShuvaev/intellij-dynamodb/issues/20) Tables are not shown if you have no permissions for some of them
- [\#21](https://github.com/AntonShuvaev/intellij-dynamodb/issues/21) Support ScyllaDB
- TraceableDisposable$DisposalException thrown in some cases


## 2022.3.1
### Fixed
- [\#18](https://github.com/AntonShuvaev/intellij-dynamodb/issues/18) Fixed error when creating item with unicode symbol

### Added
- Added operations DescribeImport, ListImports, ImportTable
- Added ability to choose custom color for connection
- Added aws regions me-central-1, eu-central-2
- Added help action group

### Changed
- Updated DynamoDB documentation

## 2022.3.0
### Fixed
- [\#17](https://github.com/AntonShuvaev/intellij-dynamodb/issues/17) DynamoDB language injection doesn't handle ? parameter placements
- Table row numbers are incorrect when switch between different requests
- NullPointerException when applying "Wrap with double quotes" quick fix
- TraceableDisposable$DisposalException might be thrown in some cases

### Added
- Show consumed capacity in the result table
- Show in history search only matching requests
- Support for 2022.3

## 2022.2.3
### Fixed
- "IllegalArgumentException: Illegal base64 character" might occur in some cases

## 2022.2.2
### Fixed
- "IllegalArgumentException: Illegal base64 character" might occur on Windows and cause the loss of state

## 2022.2.1
### Added
- [\#13](https://github.com/AntonShuvaev/intellij-dynamodb/issues/13) Added ability to specify .aws/config file along with .aws/credentials file

### Fixed
- NullPointerException might occur in import dialog

## 2022.2.0
### Added
- Show list of consoles in the explorer
- Compatibility with IntelliJ Platform 2022.2

### Changed
- [\#9](https://github.com/AntonShuvaev/intellij-dynamodb/issues/9) Favorites moved to the explorer

### Fixed
- [\#10](https://github.com/AntonShuvaev/intellij-dynamodb/issues/10) Filter resets every time I run a query

## 2022.1.9
### Fixed
- com.intellij.diagnostic.PluginException might occur
- Field name mapping in export does not work correctly

### Added
- Ability to send error reports to the developer

## 2022.1.8
### Fixed
- java.lang.ExceptionInInitializerError might occur
- When editing item message about key changed might appear incorrectly

## 2022.1.7
### Added
- Filter tables by name pattern and tags
- Editing Favorites from editor

## 2022.1.6
### Fixed
- \#3 Query for attributes containing '-' fails
- The error might occur when not default theme is used

## 2022.1.5
### Fixed
- Fixed memory leak

## 2022.1.4
### Added
- Support PartiQL queries with autocompletion
- Cache fields from previous requests to use them in autocompletion 
- Show backups in the explorer tree
- \#2 AWS SSO Support (Requires sso login with AWS CLI)

### Fixed
- \#1 only shows the first 50 tables
- Export to Dump file might generate incorrect Create table request

## 2022.1.3
### Added
- Gzipping export files
- Import from CSV, JSON, DynamoDB JSON and Dump files (or gzipped files)
- Copying tables

### Changed
- Favorite requests moved to Bookmarks tool window

### Fixed
- Fixed exporting all items

## 2022.1.2
### Fixed
- Tables may not be refreshed in database explorer tree

### Added
- Adding, editing and deleting rows in tables
- Multilevel table header

## 2022.1.0
### Added
- Connect to local or cloud DynamoDB
- Browse data in Table, JSON ot DynamoDB JSON view, with paginating and filtering fields
- Autocompletion for API operations
- Documentation for API operations
- Easily scan or query your data with simple expression DSL
- Keep your favorite requests in project or scratch files
- Create, Update or Delete items
- Export items to CSV, JSON, DynamoDB JSON
- Requests history
- Saving favorite requests